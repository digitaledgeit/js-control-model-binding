# control-binding

[![Circle CI](https://circleci.com/gh/digitaledgeit/js-control-model-binding.svg?style=svg)](https://circleci.com/gh/digitaledgeit/js-control-model-binding)

A plugin that binds a model to a [control](https://github.com/nib-health-funds/control).

## Usage

	control.use(plugin({
		model:      model,
		property    'firstName'
	}));

Now, when the control is validated the model will be updated, and, when the model is changed the control will be updated.

## Options

 - `model` - The model e.g. [anthonyshort/observable](https://github.com/anthonyshort/observable)
 - `property` - The model property
 - `mapper` - Methods to map the value between the model and control
 - `event` - The control event(s) to bind to e.g. `validate` or `change`

## Known Issues

 - On most observables you cannot set properties to be instances of a class because of the way the properties of objects are set