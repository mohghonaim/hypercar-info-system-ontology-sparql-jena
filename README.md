# hypercar-info-system-ontology-sparql-jena

Background


Hypercar Information System is used as a registry for hypercars, storing information about hypercars including engine spec, performance spec, transmission, model type and manufacturer. It also helps us find common specs between the various hypercar models.


The reason we register this information using ontology is because there are relations between models.


Hypercar manufacturers (i.e. Bugatti) do not make new models frequently. What they do is, they put out one base model (i.e. Bugatti Chiron) every 10-12 years. And during this gap they produce special editions and variants based on this model.


These variants can be track-only versions of the base model, downforce (track-focused lightweight) model, low drag (top-speed focused), one-off (coach-built, unique) model, or roadster version. These variants share specs with each other and with the base model while differing in other specs.


For example, the models can share the same engine (number of cylinders, layout, capacity, ..) and share the transmission spec (same number of gears, same transmission type) but differ in performance specs.


Description


Manufacturer makes at least 1 Model.


Models are divided into:


	Base Model (from which variants are made),


	Downforce Model (high-downforce track-focused sports model),


	Low Drag Model (top-speed-focused model),


	One-Off Model (unique model of which only 1 car is made)


	Roadster Model (model with removable/convertible roof)


	Track Only Model (track model illegal on road)


Model has exactly 1 Bodystyle (model bodystyle is coupe or roadster).


Model has exactly one Performance Spec (power, torque, drivetrain).


Model has max 1 Retractable Wing (wing width, wing adjustment type, angle of attack).


Model has exactly 1 Transmission Spec.


Model has exactly 1 Engine Spec (cylinders, capacity, layout, aspiration).


Model has exactly 1 Wheel Type (material, spokes, bolting).


Downforce Model, Track Only Model has exactly 1 Fixed Wing.


Roadster Model has exactly one Roadster (bodystyle).


Downforce Model, Low Drag Model, One Off Model, Roadster Model, Track Only Model have exactly 1 Base Model.


Transmission Spec is divided into A/T, Dual Clutch, Manual, Multi Clutch, Single Speed Direct Drive.


Wheel is divided into Carbon Wheel, Alloy Wheel, CenterLockWheel, LugNutWheel.


Carbon Wheel and Alloy Wheel are disjoint.


Center Lock Wheel and Lug Nut Wheel are disjoint.


A Wheel can be of type Carbon Wheel and Center Lock Wheel for example.


(For more info, refer to .pdf file ih the repo)
