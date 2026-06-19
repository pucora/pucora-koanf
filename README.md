# Pucora koanf

A config parser for the [Pucora](http://pucora.io/) framework

## How to use it

Import the package

	import "github.com/pucora/pucora-koanf"

And you are ready for building a parser and get the config from json / yaml / toml files.

	parser := koanf.New()
	serviceConfig, err := parser.Parse(*configFile)
	if err != nil {
		log.Fatal("ERROR:", err.Error())
	}
