# rx-js-notes


Observable methods
	next
	error
	complete

Observer can 
	.subscribe (
		next
		error
		complete
)

	.unsubscribe
————————————————————————
fromEvent: create observable for event
from: create observable for json/ values
————————————————————————
Hot Observable
	observer gets all previous events.
	.share on observable
————————————————————————

?Observables can call next in create call only.
with subjects next can be called anywhere
Observer able to emit values, its both observable and observer at the same time
Receives values only after .subscribe

Subjects

BehaviorSubject
	new observer can receive one event before its creations	

ReplaySubject
	new observer can receive number of events specified, before its creations	

AsyncSubject
	values only sent when complete is called upon subject.
————————————————————————

Operators

Modify observable return one

Static
	create obervable
Instance
	applied on observable instances

Examples
	merge : merges two observables
	map : map values 
	pluck : to pick some values


