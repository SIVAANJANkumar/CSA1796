hypothesis(has_fever) :- symptom(high_temperature).
hypothesis(has_cough) :- symptom(cough).
hypothesis(has_rash) :- symptom(skin_rash).

symptom(high_temperature).
symptom(cough).
symptom(skin_rash).

forward_chain :-
    hypothesis(Hypothesis),
    writeln('Patient may have: '),
    writeln(Hypothesis),
    retract(symptom(Hypothesis)),
    fail.
forward_chain.
