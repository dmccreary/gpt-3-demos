# OpenAI API Key Setup

## You can get your keys here:

https://beta.openai.com/account/api-keys

## UNIX Environment Variable Method
You can set the environment variable 

```sh
export OPENAI_API_KEY=<API-KEY>
```

In your .bash_profile or similar shell startup.

Verify by typing:

```sh
echo $OPENAI_API_KEY
```

### Test your key
After you install the openapi conda environment you should then have an openai command in your path:

```sh
$ which openai
```

Using the lowest cost engine: ada
```sh
openai api completions.create -e ada -p "The quick brown fox" -M 5 --stream
```

Which returned this for me:

```sh
The quick brown fox made many choices that we(gpt)
```

Error: No API key provided. (HINT: set your API key using in code using "openai.api_key = <API-KEY>", or you can set the environment variable OPENAI_API_KEY=<API-KEY>). You can generate API keys in the OpenAI web interface. See https://onboard.openai.com for details, or email support@openai.com if you have any questions.

openai api completions.create -e ada -p "This is a test" -M 5 --stream