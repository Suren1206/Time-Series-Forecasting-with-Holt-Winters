On Choice made - Dataset & Scope

(1) Why choose didactic dataset like AirPassengers ?
    • Adversarial dataset → is needed when we reach a need to challenge and break models. I felt AirPassengers is excellent for learning
    • Goal of this project is to see and understand how the chosen models works; I intend to choose an Adversarial data set in my next project to review if my understanding is real.

(2) The Scope of the project is only to see and a get a feel of model functionality & high level understanding of how parameter choices impact the model & a glance of sensitivity analysis. The exploration ended with a clarity that Depth in Detailing need not translate to Real Value

Key Insights :

(A) Model Structure vs Model Performance

        ◦ In Holt–Winters, accuracy is a constraint; structure is the objective. A healthy model distributes responsibility across components correctly
        ◦ Optimization finds numbers. Parameter reasoning decides whether you should trust them.
        ◦ Model correctness answers “can this model represent the process at all?”; Data sufficiency answers “has the model seen enough data to stabilize its internal states?”
        ◦ Never justify model rejection by listing missing components. Justify it by showing how missing components distort existing ones.
        
(B) Parameters, States, and Dynamics

    • Alpha alone is inadequate to explain structured variation; it only fine-tunes the baseline once structure is accounted for. β weights the new observed slope from data against the previously estimated trend.
    • The level answers: “Where is the series right now?” Both:Trend (direction of movement), and Seasonality (oscillation around baseline) are defined relative to the level. No amount of correct trend or seasonality can fix a wrong level
    • α answers: “Did the whole series shift up or down?”; β answers: “Did the rate of increase itself change?”
    • In classical exponential smoothing, parameters are fixed; only states evolve.
        ◦ States have units. Parameters have no units.
        ◦ States evolve. Parameters control how fast they evolve.
