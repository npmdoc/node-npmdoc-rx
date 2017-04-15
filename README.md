# api documentation for  [rx (v4.1.0)](https://github.com/Reactive-Extensions/RxJS)  [![npm package](https://img.shields.io/npm/v/npmdoc-rx.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-rx) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-rx.svg)](https://travis-ci.org/npmdoc/node-npmdoc-rx)
#### Library for composing asynchronous and event-based operations in JavaScript

[![NPM](https://nodei.co/npm/rx.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/rx)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rx/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rx/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-rx/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-rx/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Cloud Programmability Team",
        "url": "https://github.com/Reactive-Extensions/RxJS/blob/master/authors.txt"
    },
    "browser": {
        "index.js": "./dist/rx.all.js"
    },
    "bugs": {
        "url": "https://github.com/Reactive-Extensions/RxJS/issues"
    },
    "dependencies": {},
    "description": "Library for composing asynchronous and event-based operations in JavaScript",
    "devDependencies": {
        "benchmark": "*",
        "grunt": "*",
        "grunt-cli": "*",
        "grunt-contrib-concat": "*",
        "grunt-contrib-connect": "*",
        "grunt-contrib-copy": "*",
        "grunt-contrib-jshint": "*",
        "grunt-contrib-qunit": "*",
        "grunt-contrib-uglify": "*",
        "grunt-contrib-watch": "*",
        "grunt-jscs": "*",
        "grunt-saucelabs": "*",
        "load-grunt-tasks": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "a5f13ff79ef3b740fe30aa803fb09f98805d4782",
        "tarball": "https://registry.npmjs.org/rx/-/rx-4.1.0.tgz"
    },
    "gitHead": "11cd57f5d66dd2a4bc3ed8140bfac48093e59197",
    "homepage": "https://github.com/Reactive-Extensions/RxJS",
    "jam": {
        "main": "dist/rx.all.js"
    },
    "keywords": [
        "LINQ",
        "FRP",
        "Reactive",
        "Events",
        "Rx",
        "RxJS"
    ],
    "license": "Apache-2.0",
    "main": "index.js",
    "maintainers": [
        {
            "name": "vvilhonen"
        },
        {
            "name": "mattpodwysocki"
        }
    ],
    "name": "rx",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Reactive-Extensions/RxJS.git"
    },
    "scripts": {
        "test": "grunt"
    },
    "title": "Reactive Extensions for JavaScript (RxJS)",
    "version": "4.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module rx](#apidoc.module.rx)
1.  [function <span class="apidocSignatureSpan">rx.</span>AnonymousObservable (subscribe, parent)](#apidoc.element.rx.AnonymousObservable)
1.  [function <span class="apidocSignatureSpan">rx.</span>AnonymousObserver (onNext, onError, onCompleted)](#apidoc.element.rx.AnonymousObserver)
1.  [function <span class="apidocSignatureSpan">rx.</span>AnonymousSubject (observer, observable)](#apidoc.element.rx.AnonymousSubject)
1.  [function <span class="apidocSignatureSpan">rx.</span>ArgumentOutOfRangeError ()](#apidoc.element.rx.ArgumentOutOfRangeError)
1.  [function <span class="apidocSignatureSpan">rx.</span>AsyncSubject ()](#apidoc.element.rx.AsyncSubject)
1.  [function <span class="apidocSignatureSpan">rx.</span>BehaviorSubject (value)](#apidoc.element.rx.BehaviorSubject)
1.  [function <span class="apidocSignatureSpan">rx.</span>BinaryDisposable (first, second)](#apidoc.element.rx.BinaryDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>CompositeDisposable ()](#apidoc.element.rx.CompositeDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>CompositeError (errors)](#apidoc.element.rx.CompositeError)
1.  [function <span class="apidocSignatureSpan">rx.</span>ConnectableObservable (source, subject)](#apidoc.element.rx.ConnectableObservable)
1.  [function <span class="apidocSignatureSpan">rx.</span>Disposable (action)](#apidoc.element.rx.Disposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>EmptyError ()](#apidoc.element.rx.EmptyError)
1.  [function <span class="apidocSignatureSpan">rx.</span>FlatMapObservable (source, selector, resultSelector, thisArg)](#apidoc.element.rx.FlatMapObservable)
1.  [function <span class="apidocSignatureSpan">rx.</span>HistoricalScheduler (initialClock, comparer)](#apidoc.element.rx.HistoricalScheduler)
1.  [function <span class="apidocSignatureSpan">rx.</span>MockDisposable (scheduler)](#apidoc.element.rx.MockDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>NAryDisposable (disposables)](#apidoc.element.rx.NAryDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>NotImplementedError (message)](#apidoc.element.rx.NotImplementedError)
1.  [function <span class="apidocSignatureSpan">rx.</span>NotSupportedError (message)](#apidoc.element.rx.NotSupportedError)
1.  [function <span class="apidocSignatureSpan">rx.</span>Notification ()](#apidoc.element.rx.Notification)
1.  [function <span class="apidocSignatureSpan">rx.</span>ObjectDisposedError ()](#apidoc.element.rx.ObjectDisposedError)
1.  [function <span class="apidocSignatureSpan">rx.</span>Observable ()](#apidoc.element.rx.Observable)
1.  [function <span class="apidocSignatureSpan">rx.</span>ObservableBase ()](#apidoc.element.rx.ObservableBase)
1.  [function <span class="apidocSignatureSpan">rx.</span>Observer ()](#apidoc.element.rx.Observer)
1.  [function <span class="apidocSignatureSpan">rx.</span>Pauser ()](#apidoc.element.rx.Pauser)
1.  [function <span class="apidocSignatureSpan">rx.</span>Recorded (time, value, comparer)](#apidoc.element.rx.Recorded)
1.  [function <span class="apidocSignatureSpan">rx.</span>RefCountDisposable (disposable)](#apidoc.element.rx.RefCountDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>ReplaySubject (bufferSize, windowSize, scheduler)](#apidoc.element.rx.ReplaySubject)
1.  [function <span class="apidocSignatureSpan">rx.</span>Scheduler ()](#apidoc.element.rx.Scheduler)
1.  [function <span class="apidocSignatureSpan">rx.</span>SerialDisposable ()](#apidoc.element.rx.SerialDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>SingleAssignmentDisposable ()](#apidoc.element.rx.SingleAssignmentDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>Subject ()](#apidoc.element.rx.Subject)
1.  [function <span class="apidocSignatureSpan">rx.</span>Subscription (start, end)](#apidoc.element.rx.Subscription)
1.  [function <span class="apidocSignatureSpan">rx.</span>TestScheduler ()](#apidoc.element.rx.TestScheduler)
1.  [function <span class="apidocSignatureSpan">rx.</span>TimeoutError (message)](#apidoc.element.rx.TimeoutError)
1.  [function <span class="apidocSignatureSpan">rx.</span>VirtualTimeScheduler (initialClock, comparer)](#apidoc.element.rx.VirtualTimeScheduler)
1.  [function <span class="apidocSignatureSpan">rx.</span>internals.AbstractObserver ()](#apidoc.element.rx.internals.AbstractObserver)
1.  [function <span class="apidocSignatureSpan">rx.</span>internals.Enumerable ()](#apidoc.element.rx.internals.Enumerable)
1.  [function <span class="apidocSignatureSpan">rx.</span>internals.PriorityQueue (capacity)](#apidoc.element.rx.internals.PriorityQueue)
1.  [function <span class="apidocSignatureSpan">rx.</span>internals.SchedulePeriodicRecursive (scheduler, state, period, action)](#apidoc.element.rx.internals.SchedulePeriodicRecursive)
1.  [function <span class="apidocSignatureSpan">rx.</span>internals.ScheduledItem (scheduler, state, action, dueTime, comparer)](#apidoc.element.rx.internals.ScheduledItem)
1.  [function <span class="apidocSignatureSpan">rx.</span>internals.ScheduledObserver (scheduler, observer)](#apidoc.element.rx.internals.ScheduledObserver)
1.  object <span class="apidocSignatureSpan">rx.</span>AnonymousObservable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>AnonymousObserver.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>AnonymousSubject.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>AsyncSubject.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>BehaviorSubject.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>BinaryDisposable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>CompositeDisposable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>ConnectableObservable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>Disposable.empty
1.  object <span class="apidocSignatureSpan">rx.</span>Disposable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>FlatMapObservable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>HistoricalScheduler.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>MockDisposable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>NAryDisposable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>Notification.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>Observable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>ObservableBase.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>Observer.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>Pauser.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>ReactiveTest
1.  object <span class="apidocSignatureSpan">rx.</span>Recorded.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>RefCountDisposable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>ReplaySubject.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>Rx
1.  object <span class="apidocSignatureSpan">rx.</span>Scheduler.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>SerialDisposable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>SingleAssignmentDisposable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>Subject.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>Subscription.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>TestScheduler.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>VirtualTimeScheduler.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>config
1.  object <span class="apidocSignatureSpan">rx.</span>doneEnumerator
1.  object <span class="apidocSignatureSpan">rx.</span>helpers
1.  object <span class="apidocSignatureSpan">rx.</span>internals
1.  object <span class="apidocSignatureSpan">rx.</span>internals.AbstractObserver.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>internals.Enumerable.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>internals.PriorityQueue.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>internals.SchedulePeriodicRecursive.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>internals.ScheduledItem.prototype
1.  object <span class="apidocSignatureSpan">rx.</span>internals.ScheduledObserver.prototype

#### [module rx.AnonymousObservable](#apidoc.module.rx.AnonymousObservable)
1.  [function <span class="apidocSignatureSpan">rx.</span>AnonymousObservable (subscribe, parent)](#apidoc.element.rx.AnonymousObservable.AnonymousObservable)

#### [module rx.AnonymousObservable.prototype](#apidoc.module.rx.AnonymousObservable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousObservable.prototype.</span>_subscribe (o)](#apidoc.element.rx.AnonymousObservable.prototype._subscribe)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousObservable.prototype.</span>constructor (subscribe, parent)](#apidoc.element.rx.AnonymousObservable.prototype.constructor)

#### [module rx.AnonymousObserver](#apidoc.module.rx.AnonymousObserver)
1.  [function <span class="apidocSignatureSpan">rx.</span>AnonymousObserver (onNext, onError, onCompleted)](#apidoc.element.rx.AnonymousObserver.AnonymousObserver)

#### [module rx.AnonymousObserver.prototype](#apidoc.module.rx.AnonymousObserver.prototype)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousObserver.prototype.</span>completed ()](#apidoc.element.rx.AnonymousObserver.prototype.completed)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousObserver.prototype.</span>constructor (onNext, onError, onCompleted)](#apidoc.element.rx.AnonymousObserver.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousObserver.prototype.</span>error (error)](#apidoc.element.rx.AnonymousObserver.prototype.error)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousObserver.prototype.</span>next (value)](#apidoc.element.rx.AnonymousObserver.prototype.next)

#### [module rx.AnonymousSubject](#apidoc.module.rx.AnonymousSubject)
1.  [function <span class="apidocSignatureSpan">rx.</span>AnonymousSubject (observer, observable)](#apidoc.element.rx.AnonymousSubject.AnonymousSubject)

#### [module rx.AnonymousSubject.prototype](#apidoc.module.rx.AnonymousSubject.prototype)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>_subscribe (o)](#apidoc.element.rx.AnonymousSubject.prototype._subscribe)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>asObserver ()](#apidoc.element.rx.AnonymousSubject.prototype.asObserver)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>checked ()](#apidoc.element.rx.AnonymousSubject.prototype.checked)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>constructor (observer, observable)](#apidoc.element.rx.AnonymousSubject.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.AnonymousSubject.prototype.makeSafe)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.AnonymousSubject.prototype.notifyOn)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>onCompleted ()](#apidoc.element.rx.AnonymousSubject.prototype.onCompleted)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>onError (error)](#apidoc.element.rx.AnonymousSubject.prototype.onError)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>onNext (value)](#apidoc.element.rx.AnonymousSubject.prototype.onNext)
1.  [function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>toNotifier ()](#apidoc.element.rx.AnonymousSubject.prototype.toNotifier)

#### [module rx.AsyncSubject](#apidoc.module.rx.AsyncSubject)
1.  [function <span class="apidocSignatureSpan">rx.</span>AsyncSubject ()](#apidoc.element.rx.AsyncSubject.AsyncSubject)

#### [module rx.AsyncSubject.prototype](#apidoc.module.rx.AsyncSubject.prototype)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>_subscribe (o)](#apidoc.element.rx.AsyncSubject.prototype._subscribe)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>asObserver ()](#apidoc.element.rx.AsyncSubject.prototype.asObserver)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>checked ()](#apidoc.element.rx.AsyncSubject.prototype.checked)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>constructor ()](#apidoc.element.rx.AsyncSubject.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>dispose ()](#apidoc.element.rx.AsyncSubject.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>hasObservers ()](#apidoc.element.rx.AsyncSubject.prototype.hasObservers)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.AsyncSubject.prototype.makeSafe)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.AsyncSubject.prototype.notifyOn)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>onCompleted ()](#apidoc.element.rx.AsyncSubject.prototype.onCompleted)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>onError (error)](#apidoc.element.rx.AsyncSubject.prototype.onError)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>onNext (value)](#apidoc.element.rx.AsyncSubject.prototype.onNext)
1.  [function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>toNotifier ()](#apidoc.element.rx.AsyncSubject.prototype.toNotifier)

#### [module rx.BehaviorSubject](#apidoc.module.rx.BehaviorSubject)
1.  [function <span class="apidocSignatureSpan">rx.</span>BehaviorSubject (value)](#apidoc.element.rx.BehaviorSubject.BehaviorSubject)

#### [module rx.BehaviorSubject.prototype](#apidoc.module.rx.BehaviorSubject.prototype)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>_subscribe (o)](#apidoc.element.rx.BehaviorSubject.prototype._subscribe)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>asObserver ()](#apidoc.element.rx.BehaviorSubject.prototype.asObserver)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>checked ()](#apidoc.element.rx.BehaviorSubject.prototype.checked)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>constructor (value)](#apidoc.element.rx.BehaviorSubject.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>dispose ()](#apidoc.element.rx.BehaviorSubject.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>getValue ()](#apidoc.element.rx.BehaviorSubject.prototype.getValue)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>hasObservers ()](#apidoc.element.rx.BehaviorSubject.prototype.hasObservers)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.BehaviorSubject.prototype.makeSafe)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.BehaviorSubject.prototype.notifyOn)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>onCompleted ()](#apidoc.element.rx.BehaviorSubject.prototype.onCompleted)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>onError (error)](#apidoc.element.rx.BehaviorSubject.prototype.onError)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>onNext (value)](#apidoc.element.rx.BehaviorSubject.prototype.onNext)
1.  [function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>toNotifier ()](#apidoc.element.rx.BehaviorSubject.prototype.toNotifier)

#### [module rx.BinaryDisposable](#apidoc.module.rx.BinaryDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>BinaryDisposable (first, second)](#apidoc.element.rx.BinaryDisposable.BinaryDisposable)

#### [module rx.BinaryDisposable.prototype](#apidoc.module.rx.BinaryDisposable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.BinaryDisposable.prototype.</span>dispose ()](#apidoc.element.rx.BinaryDisposable.prototype.dispose)

#### [module rx.CompositeDisposable](#apidoc.module.rx.CompositeDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>CompositeDisposable ()](#apidoc.element.rx.CompositeDisposable.CompositeDisposable)

#### [module rx.CompositeDisposable.prototype](#apidoc.module.rx.CompositeDisposable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.CompositeDisposable.prototype.</span>add (item)](#apidoc.element.rx.CompositeDisposable.prototype.add)
1.  [function <span class="apidocSignatureSpan">rx.CompositeDisposable.prototype.</span>dispose ()](#apidoc.element.rx.CompositeDisposable.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">rx.CompositeDisposable.prototype.</span>remove (item)](#apidoc.element.rx.CompositeDisposable.prototype.remove)

#### [module rx.ConnectableObservable](#apidoc.module.rx.ConnectableObservable)
1.  [function <span class="apidocSignatureSpan">rx.</span>ConnectableObservable (source, subject)](#apidoc.element.rx.ConnectableObservable.ConnectableObservable)

#### [module rx.ConnectableObservable.prototype](#apidoc.module.rx.ConnectableObservable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.ConnectableObservable.prototype.</span>_subscribe (o)](#apidoc.element.rx.ConnectableObservable.prototype._subscribe)
1.  [function <span class="apidocSignatureSpan">rx.ConnectableObservable.prototype.</span>connect ()](#apidoc.element.rx.ConnectableObservable.prototype.connect)
1.  [function <span class="apidocSignatureSpan">rx.ConnectableObservable.prototype.</span>constructor (source, subject)](#apidoc.element.rx.ConnectableObservable.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.ConnectableObservable.prototype.</span>refCount ()](#apidoc.element.rx.ConnectableObservable.prototype.refCount)

#### [module rx.Disposable](#apidoc.module.rx.Disposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>Disposable (action)](#apidoc.element.rx.Disposable.Disposable)
1.  [function <span class="apidocSignatureSpan">rx.Disposable.</span>_fixup (result)](#apidoc.element.rx.Disposable._fixup)
1.  [function <span class="apidocSignatureSpan">rx.Disposable.</span>checkDisposed (disposable)](#apidoc.element.rx.Disposable.checkDisposed)
1.  [function <span class="apidocSignatureSpan">rx.Disposable.</span>create (action)](#apidoc.element.rx.Disposable.create)
1.  [function <span class="apidocSignatureSpan">rx.Disposable.</span>isDisposable (d)](#apidoc.element.rx.Disposable.isDisposable)
1.  object <span class="apidocSignatureSpan">rx.Disposable.</span>empty

#### [module rx.Disposable.empty](#apidoc.module.rx.Disposable.empty)
1.  [function <span class="apidocSignatureSpan">rx.Disposable.empty.</span>dispose ()](#apidoc.element.rx.Disposable.empty.dispose)

#### [module rx.Disposable.prototype](#apidoc.module.rx.Disposable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.Disposable.prototype.</span>dispose ()](#apidoc.element.rx.Disposable.prototype.dispose)

#### [module rx.FlatMapObservable](#apidoc.module.rx.FlatMapObservable)
1.  [function <span class="apidocSignatureSpan">rx.</span>FlatMapObservable (source, selector, resultSelector, thisArg)](#apidoc.element.rx.FlatMapObservable.FlatMapObservable)

#### [module rx.FlatMapObservable.prototype](#apidoc.module.rx.FlatMapObservable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.FlatMapObservable.prototype.</span>constructor (source, selector, resultSelector, thisArg)](#apidoc.element.rx.FlatMapObservable.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.FlatMapObservable.prototype.</span>subscribeCore (o)](#apidoc.element.rx.FlatMapObservable.prototype.subscribeCore)

#### [module rx.HistoricalScheduler](#apidoc.module.rx.HistoricalScheduler)
1.  [function <span class="apidocSignatureSpan">rx.</span>HistoricalScheduler (initialClock, comparer)](#apidoc.element.rx.HistoricalScheduler.HistoricalScheduler)

#### [module rx.HistoricalScheduler.prototype](#apidoc.module.rx.HistoricalScheduler.prototype)
1.  [function <span class="apidocSignatureSpan">rx.HistoricalScheduler.prototype.</span>add (absolute, relative)](#apidoc.element.rx.HistoricalScheduler.prototype.add)
1.  [function <span class="apidocSignatureSpan">rx.HistoricalScheduler.prototype.</span>constructor (initialClock, comparer)](#apidoc.element.rx.HistoricalScheduler.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.HistoricalScheduler.prototype.</span>toAbsoluteTime (absolute)](#apidoc.element.rx.HistoricalScheduler.prototype.toAbsoluteTime)
1.  [function <span class="apidocSignatureSpan">rx.HistoricalScheduler.prototype.</span>toRelativeTime (timeSpan)](#apidoc.element.rx.HistoricalScheduler.prototype.toRelativeTime)

#### [module rx.MockDisposable](#apidoc.module.rx.MockDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>MockDisposable (scheduler)](#apidoc.element.rx.MockDisposable.MockDisposable)

#### [module rx.MockDisposable.prototype](#apidoc.module.rx.MockDisposable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.MockDisposable.prototype.</span>dispose ()](#apidoc.element.rx.MockDisposable.prototype.dispose)

#### [module rx.NAryDisposable](#apidoc.module.rx.NAryDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>NAryDisposable (disposables)](#apidoc.element.rx.NAryDisposable.NAryDisposable)

#### [module rx.NAryDisposable.prototype](#apidoc.module.rx.NAryDisposable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.NAryDisposable.prototype.</span>dispose ()](#apidoc.element.rx.NAryDisposable.prototype.dispose)

#### [module rx.Notification](#apidoc.module.rx.Notification)
1.  [function <span class="apidocSignatureSpan">rx.</span>Notification ()](#apidoc.element.rx.Notification.Notification)
1.  [function <span class="apidocSignatureSpan">rx.Notification.</span>createOnCompleted ()](#apidoc.element.rx.Notification.createOnCompleted)
1.  [function <span class="apidocSignatureSpan">rx.Notification.</span>createOnError (error)](#apidoc.element.rx.Notification.createOnError)
1.  [function <span class="apidocSignatureSpan">rx.Notification.</span>createOnNext (value)](#apidoc.element.rx.Notification.createOnNext)

#### [module rx.Notification.prototype](#apidoc.module.rx.Notification.prototype)
1.  [function <span class="apidocSignatureSpan">rx.Notification.prototype.</span>_accept (onNext, onError, onCompleted)](#apidoc.element.rx.Notification.prototype._accept)
1.  [function <span class="apidocSignatureSpan">rx.Notification.prototype.</span>_acceptObserver (onNext, onError, onCompleted)](#apidoc.element.rx.Notification.prototype._acceptObserver)
1.  [function <span class="apidocSignatureSpan">rx.Notification.prototype.</span>accept (observerOrOnNext, onError, onCompleted)](#apidoc.element.rx.Notification.prototype.accept)
1.  [function <span class="apidocSignatureSpan">rx.Notification.prototype.</span>toObservable (scheduler)](#apidoc.element.rx.Notification.prototype.toObservable)

#### [module rx.Observable](#apidoc.module.rx.Observable)
1.  [function <span class="apidocSignatureSpan">rx.</span>Observable ()](#apidoc.element.rx.Observable.Observable)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>amb ()](#apidoc.element.rx.Observable.amb)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>case (selector, sources, defaultSourceOrScheduler)](#apidoc.element.rx.Observable.case)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>catch ()](#apidoc.element.rx.Observable.catch)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>combineLatest ()](#apidoc.element.rx.Observable.combineLatest)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>concat ()](#apidoc.element.rx.Observable.concat)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>create (subscribe, parent)](#apidoc.element.rx.Observable.create)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>defer (observableFactory)](#apidoc.element.rx.Observable.defer)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>empty (scheduler)](#apidoc.element.rx.Observable.empty)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>for (sources, resultSelector, thisArg)](#apidoc.element.rx.Observable.for)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>forIn (sources, resultSelector, thisArg)](#apidoc.element.rx.Observable.forIn)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>forkJoin ()](#apidoc.element.rx.Observable.forkJoin)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>from (iterable, mapFn, thisArg, scheduler)](#apidoc.element.rx.Observable.from)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>fromArray (array, scheduler)](#apidoc.element.rx.Observable.fromArray)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>fromCallback (fn, ctx, selector)](#apidoc.element.rx.Observable.fromCallback)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>fromEvent (element, eventName, selector)](#apidoc.element.rx.Observable.fromEvent)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>fromEventPattern (addHandler, removeHandler, selector)](#apidoc.element.rx.Observable.fromEventPattern)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>fromNodeCallback (fn, ctx, selector)](#apidoc.element.rx.Observable.fromNodeCallback)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>fromPromise (promise, scheduler)](#apidoc.element.rx.Observable.fromPromise)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>generate (initialState, condition, iterate, resultSelector, scheduler)](#apidoc.element.rx.Observable.generate)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>generateWithAbsoluteTime (initialState, condition, iterate, resultSelector, timeSelector, scheduler)](#apidoc.element.rx.Observable.generateWithAbsoluteTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>generateWithRelativeTime (initialState, condition, iterate, resultSelector, timeSelector, scheduler)](#apidoc.element.rx.Observable.generateWithRelativeTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>if (condition, thenSource, elseSourceOrScheduler)](#apidoc.element.rx.Observable.if)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>interval (period, scheduler)](#apidoc.element.rx.Observable.interval)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>isObservable (o)](#apidoc.element.rx.Observable.isObservable)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>just (value, scheduler)](#apidoc.element.rx.Observable.just)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>merge ()](#apidoc.element.rx.Observable.merge)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>mergeDelayError ()](#apidoc.element.rx.Observable.mergeDelayError)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>never ()](#apidoc.element.rx.Observable.never)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>of ()](#apidoc.element.rx.Observable.of)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>ofWithScheduler (scheduler)](#apidoc.element.rx.Observable.ofWithScheduler)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>onErrorResumeNext ()](#apidoc.element.rx.Observable.onErrorResumeNext)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>pairs (obj, scheduler)](#apidoc.element.rx.Observable.pairs)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>range (start, count, scheduler)](#apidoc.element.rx.Observable.range)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>repeat (value, repeatCount, scheduler)](#apidoc.element.rx.Observable.repeat)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>return (value, scheduler)](#apidoc.element.rx.Observable.return)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>spawn ()](#apidoc.element.rx.Observable.spawn)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>start (func, context, scheduler)](#apidoc.element.rx.Observable.start)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>startAsync (functionAsync)](#apidoc.element.rx.Observable.startAsync)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>throw (error, scheduler)](#apidoc.element.rx.Observable.throw)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>timer (dueTime, periodOrScheduler, scheduler)](#apidoc.element.rx.Observable.timer)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>toAsync (func, context, scheduler)](#apidoc.element.rx.Observable.toAsync)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>using (resourceFactory, observableFactory)](#apidoc.element.rx.Observable.using)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>when ()](#apidoc.element.rx.Observable.when)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>while (condition, source)](#apidoc.element.rx.Observable.while)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>whileDo (condition, source)](#apidoc.element.rx.Observable.whileDo)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>wrap (fn)](#apidoc.element.rx.Observable.wrap)
1.  [function <span class="apidocSignatureSpan">rx.Observable.</span>zip ()](#apidoc.element.rx.Observable.zip)

#### [module rx.Observable.prototype](#apidoc.module.rx.Observable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>amb (rightSource)](#apidoc.element.rx.Observable.prototype.amb)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>and (right)](#apidoc.element.rx.Observable.prototype.and)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>asObservable ()](#apidoc.element.rx.Observable.prototype.asObservable)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>average (keySelector, thisArg)](#apidoc.element.rx.Observable.prototype.average)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>buffer ()](#apidoc.element.rx.Observable.prototype.buffer)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferCount (count, skip)](#apidoc.element.rx.Observable.prototype.bufferCount)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferTime (timeSpan, timeShiftOrScheduler, scheduler)](#apidoc.element.rx.Observable.prototype.bufferTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferTimeOrCount (timeSpan, count, scheduler)](#apidoc.element.rx.Observable.prototype.bufferTimeOrCount)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferWithCount (count, skip)](#apidoc.element.rx.Observable.prototype.bufferWithCount)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferWithTime (timeSpan, timeShiftOrScheduler, scheduler)](#apidoc.element.rx.Observable.prototype.bufferWithTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferWithTimeOrCount (timeSpan, count, scheduler)](#apidoc.element.rx.Observable.prototype.bufferWithTimeOrCount)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>catch (handlerOrSecond)](#apidoc.element.rx.Observable.prototype.catch)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>combineLatest ()](#apidoc.element.rx.Observable.prototype.combineLatest)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>concat ()](#apidoc.element.rx.Observable.prototype.concat)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>concatAll ()](#apidoc.element.rx.Observable.prototype.concatAll)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>concatMap (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.concatMap)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>concatMapObserver (onNext, onError, onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.concatMapObserver)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>controlled (enableQueue, scheduler)](#apidoc.element.rx.Observable.prototype.controlled)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>count (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.count)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>debounce ()](#apidoc.element.rx.Observable.prototype.debounce)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>defaultIfEmpty (defaultValue)](#apidoc.element.rx.Observable.prototype.defaultIfEmpty)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>delay ()](#apidoc.element.rx.Observable.prototype.delay)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>delaySubscription (dueTime, scheduler)](#apidoc.element.rx.Observable.prototype.delaySubscription)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>dematerialize ()](#apidoc.element.rx.Observable.prototype.dematerialize)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>distinct (keySelector, comparer)](#apidoc.element.rx.Observable.prototype.distinct)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>distinctUntilChanged (keyFn, comparer)](#apidoc.element.rx.Observable.prototype.distinctUntilChanged)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>do (observerOrOnNext, onError, onCompleted)](#apidoc.element.rx.Observable.prototype.do)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>doAction (observerOrOnNext, onError, onCompleted)](#apidoc.element.rx.Observable.prototype.doAction)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>doOnCompleted (onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.doOnCompleted)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>doOnError (onError, thisArg)](#apidoc.element.rx.Observable.prototype.doOnError)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>doOnNext (onNext, thisArg)](#apidoc.element.rx.Observable.prototype.doOnNext)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>doWhile (condition)](#apidoc.element.rx.Observable.prototype.doWhile)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>elementAt (index, defaultValue)](#apidoc.element.rx.Observable.prototype.elementAt)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>every (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.every)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>exhaustMap (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.exhaustMap)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>expand (selector, scheduler)](#apidoc.element.rx.Observable.prototype.expand)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>extend (selector, scheduler)](#apidoc.element.rx.Observable.prototype.extend)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>filter (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.filter)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>finally (action, thisArg)](#apidoc.element.rx.Observable.prototype.finally)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>find (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.find)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>findIndex (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.findIndex)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>first ()](#apidoc.element.rx.Observable.prototype.first)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMap (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMap)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapConcat (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapConcat)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapFirst (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapFirst)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapLatest (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapLatest)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapMaxConcurrent (limit, selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapMaxConcurrent)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapObserver (onNext, onError, onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapObserver)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapWithMaxConcurrent (limit, selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapWithMaxConcurrent)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>forEach (oOrOnNext, onError, onCompleted)](#apidoc.element.rx.Observable.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>forkJoin ()](#apidoc.element.rx.Observable.prototype.forkJoin)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>groupBy (keySelector, elementSelector)](#apidoc.element.rx.Observable.prototype.groupBy)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>groupByUntil (keySelector, elementSelector, durationSelector)](#apidoc.element.rx.Observable.prototype.groupByUntil)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>groupJoin (right, leftDurationSelector, rightDurationSelector, resultSelector)](#apidoc.element.rx.Observable.prototype.groupJoin)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>ignoreElements ()](#apidoc.element.rx.Observable.prototype.ignoreElements)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>includes (searchElement, fromIndex)](#apidoc.element.rx.Observable.prototype.includes)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>indexOf (searchElement, fromIndex)](#apidoc.element.rx.Observable.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>isEmpty ()](#apidoc.element.rx.Observable.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>join (right, leftDurationSelector, rightDurationSelector, resultSelector)](#apidoc.element.rx.Observable.prototype.join)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>jortSort ()](#apidoc.element.rx.Observable.prototype.jortSort)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>jortSortUntil (other)](#apidoc.element.rx.Observable.prototype.jortSortUntil)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>last ()](#apidoc.element.rx.Observable.prototype.last)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>lastIndexOf (searchElement, fromIndex)](#apidoc.element.rx.Observable.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>let (func)](#apidoc.element.rx.Observable.prototype.let)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>letBind (func)](#apidoc.element.rx.Observable.prototype.letBind)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>manySelect (selector, scheduler)](#apidoc.element.rx.Observable.prototype.manySelect)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>map (selector, thisArg)](#apidoc.element.rx.Observable.prototype.map)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>materialize ()](#apidoc.element.rx.Observable.prototype.materialize)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>max (comparer)](#apidoc.element.rx.Observable.prototype.max)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>maxBy (keySelector, comparer)](#apidoc.element.rx.Observable.prototype.maxBy)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>merge (maxConcurrentOrOther)](#apidoc.element.rx.Observable.prototype.merge)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>mergeAll ()](#apidoc.element.rx.Observable.prototype.mergeAll)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>mergeMap (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.mergeMap)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>min (comparer)](#apidoc.element.rx.Observable.prototype.min)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>minBy (keySelector, comparer)](#apidoc.element.rx.Observable.prototype.minBy)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>multicast (subjectOrSubjectSelector, selector)](#apidoc.element.rx.Observable.prototype.multicast)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>observeOn (scheduler)](#apidoc.element.rx.Observable.prototype.observeOn)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>onErrorResumeNext (second)](#apidoc.element.rx.Observable.prototype.onErrorResumeNext)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>pairwise ()](#apidoc.element.rx.Observable.prototype.pairwise)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>partition (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.partition)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>pausable (pauser)](#apidoc.element.rx.Observable.prototype.pausable)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>pausableBuffered (pauser)](#apidoc.element.rx.Observable.prototype.pausableBuffered)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>pipe (dest)](#apidoc.element.rx.Observable.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>pluck ()](#apidoc.element.rx.Observable.prototype.pluck)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>publish (selector)](#apidoc.element.rx.Observable.prototype.publish)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>publishLast (selector)](#apidoc.element.rx.Observable.prototype.publishLast)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>publishValue (initialValueOrSelector, initialValue)](#apidoc.element.rx.Observable.prototype.publishValue)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>reduce ()](#apidoc.element.rx.Observable.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>repeat (repeatCount)](#apidoc.element.rx.Observable.prototype.repeat)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>repeatWhen (notifier)](#apidoc.element.rx.Observable.prototype.repeatWhen)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>replay (selector, bufferSize, windowSize, scheduler)](#apidoc.element.rx.Observable.prototype.replay)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>retry (retryCount)](#apidoc.element.rx.Observable.prototype.retry)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>retryWhen (notifier)](#apidoc.element.rx.Observable.prototype.retryWhen)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>sample (intervalOrSampler, scheduler)](#apidoc.element.rx.Observable.prototype.sample)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>scan ()](#apidoc.element.rx.Observable.prototype.scan)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>select (selector, thisArg)](#apidoc.element.rx.Observable.prototype.select)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>selectConcatObserver (onNext, onError, onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.selectConcatObserver)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>selectMany (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.selectMany)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>selectManyObserver (onNext, onError, onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.selectManyObserver)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>sequenceEqual (second, comparer)](#apidoc.element.rx.Observable.prototype.sequenceEqual)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>share ()](#apidoc.element.rx.Observable.prototype.share)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>shareReplay (bufferSize, windowSize, scheduler)](#apidoc.element.rx.Observable.prototype.shareReplay)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>shareValue (initialValue)](#apidoc.element.rx.Observable.prototype.shareValue)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>single (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.single)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>singleInstance ()](#apidoc.element.rx.Observable.prototype.singleInstance)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skip (count)](#apidoc.element.rx.Observable.prototype.skip)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipLast (count)](#apidoc.element.rx.Observable.prototype.skipLast)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipLastWithTime (duration, scheduler)](#apidoc.element.rx.Observable.prototype.skipLastWithTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipUntil (other)](#apidoc.element.rx.Observable.prototype.skipUntil)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipUntilWithTime (startTime, scheduler)](#apidoc.element.rx.Observable.prototype.skipUntilWithTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipWhile (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.skipWhile)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipWithTime (duration, scheduler)](#apidoc.element.rx.Observable.prototype.skipWithTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>slice (begin, end)](#apidoc.element.rx.Observable.prototype.slice)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>some (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.some)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>startWith ()](#apidoc.element.rx.Observable.prototype.startWith)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>subscribe (oOrOnNext, onError, onCompleted)](#apidoc.element.rx.Observable.prototype.subscribe)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>subscribeOn (scheduler)](#apidoc.element.rx.Observable.prototype.subscribeOn)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>subscribeOnCompleted (onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.subscribeOnCompleted)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>subscribeOnError (onError, thisArg)](#apidoc.element.rx.Observable.prototype.subscribeOnError)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>subscribeOnNext (onNext, thisArg)](#apidoc.element.rx.Observable.prototype.subscribeOnNext)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>sum (keySelector, thisArg)](#apidoc.element.rx.Observable.prototype.sum)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>switch ()](#apidoc.element.rx.Observable.prototype.switch)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>switchFirst ()](#apidoc.element.rx.Observable.prototype.switchFirst)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>switchLatest ()](#apidoc.element.rx.Observable.prototype.switchLatest)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>switchMap (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.switchMap)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>take (count, scheduler)](#apidoc.element.rx.Observable.prototype.take)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeLast (count)](#apidoc.element.rx.Observable.prototype.takeLast)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeLastBuffer (count)](#apidoc.element.rx.Observable.prototype.takeLastBuffer)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeLastBufferWithTime (duration, scheduler)](#apidoc.element.rx.Observable.prototype.takeLastBufferWithTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeLastWithTime (duration, scheduler)](#apidoc.element.rx.Observable.prototype.takeLastWithTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeUntil (other)](#apidoc.element.rx.Observable.prototype.takeUntil)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeUntilWithTime (endTime, scheduler)](#apidoc.element.rx.Observable.prototype.takeUntilWithTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeWhile (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.takeWhile)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeWithTime (duration, scheduler)](#apidoc.element.rx.Observable.prototype.takeWithTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>tap (observerOrOnNext, onError, onCompleted)](#apidoc.element.rx.Observable.prototype.tap)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>tapOnCompleted (onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.tapOnCompleted)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>tapOnError (onError, thisArg)](#apidoc.element.rx.Observable.prototype.tapOnError)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>tapOnNext (onNext, thisArg)](#apidoc.element.rx.Observable.prototype.tapOnNext)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>thenDo (selector)](#apidoc.element.rx.Observable.prototype.thenDo)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>throttle (windowDuration, scheduler)](#apidoc.element.rx.Observable.prototype.throttle)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>timeInterval (scheduler)](#apidoc.element.rx.Observable.prototype.timeInterval)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>timeout ()](#apidoc.element.rx.Observable.prototype.timeout)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>timestamp (scheduler)](#apidoc.element.rx.Observable.prototype.timestamp)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>toArray ()](#apidoc.element.rx.Observable.prototype.toArray)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>toMap (keySelector, elementSelector)](#apidoc.element.rx.Observable.prototype.toMap)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>toPromise (promiseCtor)](#apidoc.element.rx.Observable.prototype.toPromise)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>toSet ()](#apidoc.element.rx.Observable.prototype.toSet)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>transduce (transducer)](#apidoc.element.rx.Observable.prototype.transduce)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>where (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.where)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>window (windowOpeningsOrClosingSelector, windowClosingSelector)](#apidoc.element.rx.Observable.prototype.window)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowCount (count, skip)](#apidoc.element.rx.Observable.prototype.windowCount)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowTime (timeSpan, timeShiftOrScheduler, scheduler)](#apidoc.element.rx.Observable.prototype.windowTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowTimeOrCount (timeSpan, count, scheduler)](#apidoc.element.rx.Observable.prototype.windowTimeOrCount)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowWithCount (count, skip)](#apidoc.element.rx.Observable.prototype.windowWithCount)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowWithTime (timeSpan, timeShiftOrScheduler, scheduler)](#apidoc.element.rx.Observable.prototype.windowWithTime)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowWithTimeOrCount (timeSpan, count, scheduler)](#apidoc.element.rx.Observable.prototype.windowWithTimeOrCount)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>withLatestFrom ()](#apidoc.element.rx.Observable.prototype.withLatestFrom)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>zip ()](#apidoc.element.rx.Observable.prototype.zip)
1.  [function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>zipIterable ()](#apidoc.element.rx.Observable.prototype.zipIterable)

#### [module rx.ObservableBase](#apidoc.module.rx.ObservableBase)
1.  [function <span class="apidocSignatureSpan">rx.</span>ObservableBase ()](#apidoc.element.rx.ObservableBase.ObservableBase)

#### [module rx.ObservableBase.prototype](#apidoc.module.rx.ObservableBase.prototype)
1.  [function <span class="apidocSignatureSpan">rx.ObservableBase.prototype.</span>_subscribe (o)](#apidoc.element.rx.ObservableBase.prototype._subscribe)
1.  [function <span class="apidocSignatureSpan">rx.ObservableBase.prototype.</span>constructor ()](#apidoc.element.rx.ObservableBase.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.ObservableBase.prototype.</span>subscribeCore ()](#apidoc.element.rx.ObservableBase.prototype.subscribeCore)

#### [module rx.Observer](#apidoc.module.rx.Observer)
1.  [function <span class="apidocSignatureSpan">rx.</span>Observer ()](#apidoc.element.rx.Observer.Observer)
1.  [function <span class="apidocSignatureSpan">rx.Observer.</span>create (onNext, onError, onCompleted)](#apidoc.element.rx.Observer.create)
1.  [function <span class="apidocSignatureSpan">rx.Observer.</span>fromNotifier (handler, thisArg)](#apidoc.element.rx.Observer.fromNotifier)

#### [module rx.Observer.prototype](#apidoc.module.rx.Observer.prototype)
1.  [function <span class="apidocSignatureSpan">rx.Observer.prototype.</span>asObserver ()](#apidoc.element.rx.Observer.prototype.asObserver)
1.  [function <span class="apidocSignatureSpan">rx.Observer.prototype.</span>checked ()](#apidoc.element.rx.Observer.prototype.checked)
1.  [function <span class="apidocSignatureSpan">rx.Observer.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.Observer.prototype.makeSafe)
1.  [function <span class="apidocSignatureSpan">rx.Observer.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.Observer.prototype.notifyOn)
1.  [function <span class="apidocSignatureSpan">rx.Observer.prototype.</span>toNotifier ()](#apidoc.element.rx.Observer.prototype.toNotifier)

#### [module rx.Pauser](#apidoc.module.rx.Pauser)
1.  [function <span class="apidocSignatureSpan">rx.</span>Pauser ()](#apidoc.element.rx.Pauser.Pauser)

#### [module rx.Pauser.prototype](#apidoc.module.rx.Pauser.prototype)
1.  [function <span class="apidocSignatureSpan">rx.Pauser.prototype.</span>constructor ()](#apidoc.element.rx.Pauser.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.Pauser.prototype.</span>pause ()](#apidoc.element.rx.Pauser.prototype.pause)
1.  [function <span class="apidocSignatureSpan">rx.Pauser.prototype.</span>resume ()](#apidoc.element.rx.Pauser.prototype.resume)

#### [module rx.ReactiveTest](#apidoc.module.rx.ReactiveTest)
1.  [function <span class="apidocSignatureSpan">rx.ReactiveTest.</span>onCompleted (ticks)](#apidoc.element.rx.ReactiveTest.onCompleted)
1.  [function <span class="apidocSignatureSpan">rx.ReactiveTest.</span>onError (ticks, error)](#apidoc.element.rx.ReactiveTest.onError)
1.  [function <span class="apidocSignatureSpan">rx.ReactiveTest.</span>onNext (ticks, value)](#apidoc.element.rx.ReactiveTest.onNext)
1.  [function <span class="apidocSignatureSpan">rx.ReactiveTest.</span>subscribe (start, end)](#apidoc.element.rx.ReactiveTest.subscribe)
1.  number <span class="apidocSignatureSpan">rx.ReactiveTest.</span>created
1.  number <span class="apidocSignatureSpan">rx.ReactiveTest.</span>disposed
1.  number <span class="apidocSignatureSpan">rx.ReactiveTest.</span>subscribed

#### [module rx.Recorded](#apidoc.module.rx.Recorded)
1.  [function <span class="apidocSignatureSpan">rx.</span>Recorded (time, value, comparer)](#apidoc.element.rx.Recorded.Recorded)

#### [module rx.Recorded.prototype](#apidoc.module.rx.Recorded.prototype)
1.  [function <span class="apidocSignatureSpan">rx.Recorded.prototype.</span>equals (other)](#apidoc.element.rx.Recorded.prototype.equals)
1.  [function <span class="apidocSignatureSpan">rx.Recorded.prototype.</span>toString ()](#apidoc.element.rx.Recorded.prototype.toString)

#### [module rx.RefCountDisposable](#apidoc.module.rx.RefCountDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>RefCountDisposable (disposable)](#apidoc.element.rx.RefCountDisposable.RefCountDisposable)

#### [module rx.RefCountDisposable.prototype](#apidoc.module.rx.RefCountDisposable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.RefCountDisposable.prototype.</span>dispose ()](#apidoc.element.rx.RefCountDisposable.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">rx.RefCountDisposable.prototype.</span>getDisposable ()](#apidoc.element.rx.RefCountDisposable.prototype.getDisposable)

#### [module rx.ReplaySubject](#apidoc.module.rx.ReplaySubject)
1.  [function <span class="apidocSignatureSpan">rx.</span>ReplaySubject (bufferSize, windowSize, scheduler)](#apidoc.element.rx.ReplaySubject.ReplaySubject)

#### [module rx.ReplaySubject.prototype](#apidoc.module.rx.ReplaySubject.prototype)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>_subscribe (o)](#apidoc.element.rx.ReplaySubject.prototype._subscribe)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>_trim (now)](#apidoc.element.rx.ReplaySubject.prototype._trim)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>asObserver ()](#apidoc.element.rx.ReplaySubject.prototype.asObserver)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>checked ()](#apidoc.element.rx.ReplaySubject.prototype.checked)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>constructor (bufferSize, windowSize, scheduler)](#apidoc.element.rx.ReplaySubject.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>dispose ()](#apidoc.element.rx.ReplaySubject.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>hasObservers ()](#apidoc.element.rx.ReplaySubject.prototype.hasObservers)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.ReplaySubject.prototype.makeSafe)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.ReplaySubject.prototype.notifyOn)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>onCompleted ()](#apidoc.element.rx.ReplaySubject.prototype.onCompleted)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>onError (error)](#apidoc.element.rx.ReplaySubject.prototype.onError)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>onNext (value)](#apidoc.element.rx.ReplaySubject.prototype.onNext)
1.  [function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>toNotifier ()](#apidoc.element.rx.ReplaySubject.prototype.toNotifier)

#### [module rx.Rx](#apidoc.module.rx.Rx)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>AnonymousObservable (subscribe, parent)](#apidoc.element.rx.Rx.AnonymousObservable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>AnonymousObserver (onNext, onError, onCompleted)](#apidoc.element.rx.Rx.AnonymousObserver)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>AnonymousSubject (observer, observable)](#apidoc.element.rx.Rx.AnonymousSubject)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>ArgumentOutOfRangeError ()](#apidoc.element.rx.Rx.ArgumentOutOfRangeError)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>AsyncSubject ()](#apidoc.element.rx.Rx.AsyncSubject)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>BehaviorSubject (value)](#apidoc.element.rx.Rx.BehaviorSubject)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>BinaryDisposable (first, second)](#apidoc.element.rx.Rx.BinaryDisposable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>CompositeDisposable ()](#apidoc.element.rx.Rx.CompositeDisposable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>CompositeError (errors)](#apidoc.element.rx.Rx.CompositeError)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>ConnectableObservable (source, subject)](#apidoc.element.rx.Rx.ConnectableObservable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>Disposable (action)](#apidoc.element.rx.Rx.Disposable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>EmptyError ()](#apidoc.element.rx.Rx.EmptyError)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>FlatMapObservable (source, selector, resultSelector, thisArg)](#apidoc.element.rx.Rx.FlatMapObservable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>HistoricalScheduler (initialClock, comparer)](#apidoc.element.rx.Rx.HistoricalScheduler)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>MockDisposable (scheduler)](#apidoc.element.rx.Rx.MockDisposable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>NAryDisposable (disposables)](#apidoc.element.rx.Rx.NAryDisposable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>NotImplementedError (message)](#apidoc.element.rx.Rx.NotImplementedError)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>NotSupportedError (message)](#apidoc.element.rx.Rx.NotSupportedError)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>Notification ()](#apidoc.element.rx.Rx.Notification)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>ObjectDisposedError ()](#apidoc.element.rx.Rx.ObjectDisposedError)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>Observable ()](#apidoc.element.rx.Rx.Observable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>ObservableBase ()](#apidoc.element.rx.Rx.ObservableBase)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>Observer ()](#apidoc.element.rx.Rx.Observer)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>Pauser ()](#apidoc.element.rx.Rx.Pauser)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>Recorded (time, value, comparer)](#apidoc.element.rx.Rx.Recorded)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>RefCountDisposable (disposable)](#apidoc.element.rx.Rx.RefCountDisposable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>ReplaySubject (bufferSize, windowSize, scheduler)](#apidoc.element.rx.Rx.ReplaySubject)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>Scheduler ()](#apidoc.element.rx.Rx.Scheduler)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>SerialDisposable ()](#apidoc.element.rx.Rx.SerialDisposable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>SingleAssignmentDisposable ()](#apidoc.element.rx.Rx.SingleAssignmentDisposable)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>Subject ()](#apidoc.element.rx.Rx.Subject)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>Subscription (start, end)](#apidoc.element.rx.Rx.Subscription)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>TestScheduler ()](#apidoc.element.rx.Rx.TestScheduler)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>TimeoutError (message)](#apidoc.element.rx.Rx.TimeoutError)
1.  [function <span class="apidocSignatureSpan">rx.Rx.</span>VirtualTimeScheduler (initialClock, comparer)](#apidoc.element.rx.Rx.VirtualTimeScheduler)
1.  object <span class="apidocSignatureSpan">rx.</span>Rx
1.  object <span class="apidocSignatureSpan">rx.Rx.</span>ReactiveTest
1.  object <span class="apidocSignatureSpan">rx.Rx.</span>config
1.  object <span class="apidocSignatureSpan">rx.Rx.</span>doneEnumerator
1.  object <span class="apidocSignatureSpan">rx.Rx.</span>helpers
1.  object <span class="apidocSignatureSpan">rx.Rx.</span>internals

#### [module rx.Scheduler](#apidoc.module.rx.Scheduler)
1.  [function <span class="apidocSignatureSpan">rx.</span>Scheduler ()](#apidoc.element.rx.Scheduler.Scheduler)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.</span>isScheduler (s)](#apidoc.element.rx.Scheduler.isScheduler)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.</span>normalize (timeSpan)](#apidoc.element.rx.Scheduler.normalize)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.</span>now ()](#apidoc.element.rx.Scheduler.now)
1.  object <span class="apidocSignatureSpan">rx.Scheduler.</span>async
1.  object <span class="apidocSignatureSpan">rx.Scheduler.</span>currentThread
1.  object <span class="apidocSignatureSpan">rx.Scheduler.</span>default
1.  object <span class="apidocSignatureSpan">rx.Scheduler.</span>immediate

#### [module rx.Scheduler.prototype](#apidoc.module.rx.Scheduler.prototype)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>_scheduleFuture (state, dueTime, action)](#apidoc.element.rx.Scheduler.prototype._scheduleFuture)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>catch (handler)](#apidoc.element.rx.Scheduler.prototype.catch)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>catchError (handler)](#apidoc.element.rx.Scheduler.prototype.catchError)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>now ()](#apidoc.element.rx.Scheduler.prototype.now)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>schedule (state, action)](#apidoc.element.rx.Scheduler.prototype.schedule)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>scheduleFuture (state, dueTime, action)](#apidoc.element.rx.Scheduler.prototype.scheduleFuture)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>schedulePeriodic (state, period, action)](#apidoc.element.rx.Scheduler.prototype.schedulePeriodic)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>scheduleRecursive (state, action)](#apidoc.element.rx.Scheduler.prototype.scheduleRecursive)
1.  [function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>scheduleRecursiveFuture (state, dueTime, action)](#apidoc.element.rx.Scheduler.prototype.scheduleRecursiveFuture)

#### [module rx.SerialDisposable](#apidoc.module.rx.SerialDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>SerialDisposable ()](#apidoc.element.rx.SerialDisposable.SerialDisposable)

#### [module rx.SerialDisposable.prototype](#apidoc.module.rx.SerialDisposable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.SerialDisposable.prototype.</span>dispose ()](#apidoc.element.rx.SerialDisposable.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">rx.SerialDisposable.prototype.</span>getDisposable ()](#apidoc.element.rx.SerialDisposable.prototype.getDisposable)
1.  [function <span class="apidocSignatureSpan">rx.SerialDisposable.prototype.</span>setDisposable (value)](#apidoc.element.rx.SerialDisposable.prototype.setDisposable)

#### [module rx.SingleAssignmentDisposable](#apidoc.module.rx.SingleAssignmentDisposable)
1.  [function <span class="apidocSignatureSpan">rx.</span>SingleAssignmentDisposable ()](#apidoc.element.rx.SingleAssignmentDisposable.SingleAssignmentDisposable)

#### [module rx.SingleAssignmentDisposable.prototype](#apidoc.module.rx.SingleAssignmentDisposable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.SingleAssignmentDisposable.prototype.</span>dispose ()](#apidoc.element.rx.SingleAssignmentDisposable.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">rx.SingleAssignmentDisposable.prototype.</span>getDisposable ()](#apidoc.element.rx.SingleAssignmentDisposable.prototype.getDisposable)
1.  [function <span class="apidocSignatureSpan">rx.SingleAssignmentDisposable.prototype.</span>setDisposable (value)](#apidoc.element.rx.SingleAssignmentDisposable.prototype.setDisposable)

#### [module rx.Subject](#apidoc.module.rx.Subject)
1.  [function <span class="apidocSignatureSpan">rx.</span>Subject ()](#apidoc.element.rx.Subject.Subject)
1.  [function <span class="apidocSignatureSpan">rx.Subject.</span>create (observer, observable)](#apidoc.element.rx.Subject.create)

#### [module rx.Subject.prototype](#apidoc.module.rx.Subject.prototype)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>_subscribe (o)](#apidoc.element.rx.Subject.prototype._subscribe)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>asObserver ()](#apidoc.element.rx.Subject.prototype.asObserver)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>checked ()](#apidoc.element.rx.Subject.prototype.checked)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>constructor ()](#apidoc.element.rx.Subject.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>dispose ()](#apidoc.element.rx.Subject.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>hasObservers ()](#apidoc.element.rx.Subject.prototype.hasObservers)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.Subject.prototype.makeSafe)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.Subject.prototype.notifyOn)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>onCompleted ()](#apidoc.element.rx.Subject.prototype.onCompleted)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>onError (error)](#apidoc.element.rx.Subject.prototype.onError)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>onNext (value)](#apidoc.element.rx.Subject.prototype.onNext)
1.  [function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>toNotifier ()](#apidoc.element.rx.Subject.prototype.toNotifier)

#### [module rx.Subscription](#apidoc.module.rx.Subscription)
1.  [function <span class="apidocSignatureSpan">rx.</span>Subscription (start, end)](#apidoc.element.rx.Subscription.Subscription)

#### [module rx.Subscription.prototype](#apidoc.module.rx.Subscription.prototype)
1.  [function <span class="apidocSignatureSpan">rx.Subscription.prototype.</span>equals (other)](#apidoc.element.rx.Subscription.prototype.equals)
1.  [function <span class="apidocSignatureSpan">rx.Subscription.prototype.</span>toString ()](#apidoc.element.rx.Subscription.prototype.toString)

#### [module rx.TestScheduler](#apidoc.module.rx.TestScheduler)
1.  [function <span class="apidocSignatureSpan">rx.</span>TestScheduler ()](#apidoc.element.rx.TestScheduler.TestScheduler)

#### [module rx.TestScheduler.prototype](#apidoc.module.rx.TestScheduler.prototype)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>add (absolute, relative)](#apidoc.element.rx.TestScheduler.prototype.add)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>constructor ()](#apidoc.element.rx.TestScheduler.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>createColdObservable ()](#apidoc.element.rx.TestScheduler.prototype.createColdObservable)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>createHotObservable ()](#apidoc.element.rx.TestScheduler.prototype.createHotObservable)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>createObserver ()](#apidoc.element.rx.TestScheduler.prototype.createObserver)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>createRejectedPromise (ticks, reason)](#apidoc.element.rx.TestScheduler.prototype.createRejectedPromise)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>createResolvedPromise (ticks, value)](#apidoc.element.rx.TestScheduler.prototype.createResolvedPromise)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>scheduleAbsolute (state, dueTime, action)](#apidoc.element.rx.TestScheduler.prototype.scheduleAbsolute)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>startScheduler (createFn, settings)](#apidoc.element.rx.TestScheduler.prototype.startScheduler)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>toAbsoluteTime (absolute)](#apidoc.element.rx.TestScheduler.prototype.toAbsoluteTime)
1.  [function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>toRelativeTime (timeSpan)](#apidoc.element.rx.TestScheduler.prototype.toRelativeTime)

#### [module rx.VirtualTimeScheduler](#apidoc.module.rx.VirtualTimeScheduler)
1.  [function <span class="apidocSignatureSpan">rx.</span>VirtualTimeScheduler (initialClock, comparer)](#apidoc.element.rx.VirtualTimeScheduler.VirtualTimeScheduler)

#### [module rx.VirtualTimeScheduler.prototype](#apidoc.module.rx.VirtualTimeScheduler.prototype)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>add ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.add)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>advanceBy (time)](#apidoc.element.rx.VirtualTimeScheduler.prototype.advanceBy)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>advanceTo (time)](#apidoc.element.rx.VirtualTimeScheduler.prototype.advanceTo)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>constructor (initialClock, comparer)](#apidoc.element.rx.VirtualTimeScheduler.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>getNext ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.getNext)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>now ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.now)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>schedule (state, action)](#apidoc.element.rx.VirtualTimeScheduler.prototype.schedule)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>scheduleAbsolute (state, dueTime, action)](#apidoc.element.rx.VirtualTimeScheduler.prototype.scheduleAbsolute)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>scheduleFuture (state, dueTime, action)](#apidoc.element.rx.VirtualTimeScheduler.prototype.scheduleFuture)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>schedulePeriodic (state, period, action)](#apidoc.element.rx.VirtualTimeScheduler.prototype.schedulePeriodic)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>scheduleRelative (state, dueTime, action)](#apidoc.element.rx.VirtualTimeScheduler.prototype.scheduleRelative)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>sleep (time)](#apidoc.element.rx.VirtualTimeScheduler.prototype.sleep)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>start ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.start)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>stop ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.stop)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>toAbsoluteTime ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.toAbsoluteTime)
1.  [function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>toRelativeTime ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.toRelativeTime)

#### [module rx.config](#apidoc.module.rx.config)
1.  boolean <span class="apidocSignatureSpan">rx.config.</span>longStackSupport
1.  boolean <span class="apidocSignatureSpan">rx.config.</span>useNativeEvents
1.  [function <span class="apidocSignatureSpan">rx.config.</span>Promise ()](#apidoc.element.rx.config.Promise)

#### [module rx.helpers](#apidoc.module.rx.helpers)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>defaultComparer (x, y)](#apidoc.element.rx.helpers.defaultComparer)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>defaultError (err)](#apidoc.element.rx.helpers.defaultError)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>defaultKeySerializer (x)](#apidoc.element.rx.helpers.defaultKeySerializer)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>defaultNow ()](#apidoc.element.rx.helpers.defaultNow)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>defaultSubComparer (x, y)](#apidoc.element.rx.helpers.defaultSubComparer)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>identity (x)](#apidoc.element.rx.helpers.identity)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>isArrayLike (o)](#apidoc.element.rx.helpers.isArrayLike)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>isFunction (value)](#apidoc.element.rx.helpers.isFunction)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>isIterable (o)](#apidoc.element.rx.helpers.isIterable)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>isPromise (p)](#apidoc.element.rx.helpers.isPromise)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>noop ()](#apidoc.element.rx.helpers.noop)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>notImplemented ()](#apidoc.element.rx.helpers.notImplemented)
1.  [function <span class="apidocSignatureSpan">rx.helpers.</span>notSupported ()](#apidoc.element.rx.helpers.notSupported)
1.  symbol <span class="apidocSignatureSpan">rx.helpers.</span>iterator

#### [module rx.internals](#apidoc.module.rx.internals)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>AbstractObserver ()](#apidoc.element.rx.internals.AbstractObserver)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>Enumerable ()](#apidoc.element.rx.internals.Enumerable)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>PriorityQueue (capacity)](#apidoc.element.rx.internals.PriorityQueue)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>SchedulePeriodicRecursive (scheduler, state, period, action)](#apidoc.element.rx.internals.SchedulePeriodicRecursive)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>ScheduledItem (scheduler, state, action, dueTime, comparer)](#apidoc.element.rx.internals.ScheduledItem)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>ScheduledObserver (scheduler, observer)](#apidoc.element.rx.internals.ScheduledObserver)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>addProperties (obj)](#apidoc.element.rx.internals.addProperties)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>addRef (xs, r)](#apidoc.element.rx.internals.addRef)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>bindCallback (func, thisArg, argCount)](#apidoc.element.rx.internals.bindCallback)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>inherits (child, parent)](#apidoc.element.rx.internals.inherits)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>isEqual (value, other)](#apidoc.element.rx.internals.isEqual)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>isObject (value)](#apidoc.element.rx.internals.isObject)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>tryCatch (fn)](#apidoc.element.rx.internals.tryCatch)

#### [module rx.internals.AbstractObserver](#apidoc.module.rx.internals.AbstractObserver)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>AbstractObserver ()](#apidoc.element.rx.internals.AbstractObserver.AbstractObserver)

#### [module rx.internals.AbstractObserver.prototype](#apidoc.module.rx.internals.AbstractObserver.prototype)
1.  [function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>completed ()](#apidoc.element.rx.internals.AbstractObserver.prototype.completed)
1.  [function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>constructor ()](#apidoc.element.rx.internals.AbstractObserver.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>dispose ()](#apidoc.element.rx.internals.AbstractObserver.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>error ()](#apidoc.element.rx.internals.AbstractObserver.prototype.error)
1.  [function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>fail (e)](#apidoc.element.rx.internals.AbstractObserver.prototype.fail)
1.  [function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>next ()](#apidoc.element.rx.internals.AbstractObserver.prototype.next)
1.  [function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>onCompleted ()](#apidoc.element.rx.internals.AbstractObserver.prototype.onCompleted)
1.  [function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>onError (error)](#apidoc.element.rx.internals.AbstractObserver.prototype.onError)
1.  [function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>onNext (value)](#apidoc.element.rx.internals.AbstractObserver.prototype.onNext)

#### [module rx.internals.Enumerable](#apidoc.module.rx.internals.Enumerable)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>Enumerable ()](#apidoc.element.rx.internals.Enumerable.Enumerable)
1.  [function <span class="apidocSignatureSpan">rx.internals.Enumerable.</span>of (source, selector, thisArg)](#apidoc.element.rx.internals.Enumerable.of)
1.  [function <span class="apidocSignatureSpan">rx.internals.Enumerable.</span>repeat (value, repeatCount)](#apidoc.element.rx.internals.Enumerable.repeat)

#### [module rx.internals.Enumerable.prototype](#apidoc.module.rx.internals.Enumerable.prototype)
1.  [function <span class="apidocSignatureSpan">rx.internals.Enumerable.prototype.</span>catchError ()](#apidoc.element.rx.internals.Enumerable.prototype.catchError)
1.  [function <span class="apidocSignatureSpan">rx.internals.Enumerable.prototype.</span>concat ()](#apidoc.element.rx.internals.Enumerable.prototype.concat)

#### [module rx.internals.PriorityQueue](#apidoc.module.rx.internals.PriorityQueue)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>PriorityQueue (capacity)](#apidoc.element.rx.internals.PriorityQueue.PriorityQueue)
1.  number <span class="apidocSignatureSpan">rx.internals.PriorityQueue.</span>count

#### [module rx.internals.PriorityQueue.prototype](#apidoc.module.rx.internals.PriorityQueue.prototype)
1.  [function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>dequeue ()](#apidoc.element.rx.internals.PriorityQueue.prototype.dequeue)
1.  [function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>enqueue (item)](#apidoc.element.rx.internals.PriorityQueue.prototype.enqueue)
1.  [function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>heapify (index)](#apidoc.element.rx.internals.PriorityQueue.prototype.heapify)
1.  [function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>isHigherPriority (left, right)](#apidoc.element.rx.internals.PriorityQueue.prototype.isHigherPriority)
1.  [function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>peek ()](#apidoc.element.rx.internals.PriorityQueue.prototype.peek)
1.  [function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>percolate (index)](#apidoc.element.rx.internals.PriorityQueue.prototype.percolate)
1.  [function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>remove (item)](#apidoc.element.rx.internals.PriorityQueue.prototype.remove)
1.  [function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>removeAt (index)](#apidoc.element.rx.internals.PriorityQueue.prototype.removeAt)

#### [module rx.internals.SchedulePeriodicRecursive](#apidoc.module.rx.internals.SchedulePeriodicRecursive)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>SchedulePeriodicRecursive (scheduler, state, period, action)](#apidoc.element.rx.internals.SchedulePeriodicRecursive.SchedulePeriodicRecursive)

#### [module rx.internals.SchedulePeriodicRecursive.prototype](#apidoc.module.rx.internals.SchedulePeriodicRecursive.prototype)
1.  [function <span class="apidocSignatureSpan">rx.internals.SchedulePeriodicRecursive.prototype.</span>start ()](#apidoc.element.rx.internals.SchedulePeriodicRecursive.prototype.start)

#### [module rx.internals.ScheduledItem](#apidoc.module.rx.internals.ScheduledItem)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>ScheduledItem (scheduler, state, action, dueTime, comparer)](#apidoc.element.rx.internals.ScheduledItem.ScheduledItem)

#### [module rx.internals.ScheduledItem.prototype](#apidoc.module.rx.internals.ScheduledItem.prototype)
1.  [function <span class="apidocSignatureSpan">rx.internals.ScheduledItem.prototype.</span>compareTo (other)](#apidoc.element.rx.internals.ScheduledItem.prototype.compareTo)
1.  [function <span class="apidocSignatureSpan">rx.internals.ScheduledItem.prototype.</span>invoke ()](#apidoc.element.rx.internals.ScheduledItem.prototype.invoke)
1.  [function <span class="apidocSignatureSpan">rx.internals.ScheduledItem.prototype.</span>invokeCore ()](#apidoc.element.rx.internals.ScheduledItem.prototype.invokeCore)
1.  [function <span class="apidocSignatureSpan">rx.internals.ScheduledItem.prototype.</span>isCancelled ()](#apidoc.element.rx.internals.ScheduledItem.prototype.isCancelled)

#### [module rx.internals.ScheduledObserver](#apidoc.module.rx.internals.ScheduledObserver)
1.  [function <span class="apidocSignatureSpan">rx.internals.</span>ScheduledObserver (scheduler, observer)](#apidoc.element.rx.internals.ScheduledObserver.ScheduledObserver)

#### [module rx.internals.ScheduledObserver.prototype](#apidoc.module.rx.internals.ScheduledObserver.prototype)
1.  [function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>completed ()](#apidoc.element.rx.internals.ScheduledObserver.prototype.completed)
1.  [function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>constructor (scheduler, observer)](#apidoc.element.rx.internals.ScheduledObserver.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>dispose ()](#apidoc.element.rx.internals.ScheduledObserver.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>ensureActive ()](#apidoc.element.rx.internals.ScheduledObserver.prototype.ensureActive)
1.  [function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>error (e)](#apidoc.element.rx.internals.ScheduledObserver.prototype.error)
1.  [function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>next (x)](#apidoc.element.rx.internals.ScheduledObserver.prototype.next)



# <a name="apidoc.module.rx"></a>[module rx](#apidoc.module.rx)

#### <a name="apidoc.element.rx.AnonymousObservable"></a>[function <span class="apidocSignatureSpan">rx.</span>AnonymousObservable (subscribe, parent)](#apidoc.element.rx.AnonymousObservable)
- description and source-code
```javascript
function AnonymousObservable(subscribe, parent) {
  this.source = parent;
  this.__subscribe = subscribe;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousObserver"></a>[function <span class="apidocSignatureSpan">rx.</span>AnonymousObserver (onNext, onError, onCompleted)](#apidoc.element.rx.AnonymousObserver)
- description and source-code
```javascript
function AnonymousObserver(onNext, onError, onCompleted) {
  __super__.call(this);
  this._onNext = onNext;
  this._onError = onError;
  this._onCompleted = onCompleted;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousSubject"></a>[function <span class="apidocSignatureSpan">rx.</span>AnonymousSubject (observer, observable)](#apidoc.element.rx.AnonymousSubject)
- description and source-code
```javascript
function AnonymousSubject(observer, observable) {
  this.observer = observer;
  this.observable = observable;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ArgumentOutOfRangeError"></a>[function <span class="apidocSignatureSpan">rx.</span>ArgumentOutOfRangeError ()](#apidoc.element.rx.ArgumentOutOfRangeError)
- description and source-code
```javascript
ArgumentOutOfRangeError = function () {
  this.message = 'Argument out of range';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject"></a>[function <span class="apidocSignatureSpan">rx.</span>AsyncSubject ()](#apidoc.element.rx.AsyncSubject)
- description and source-code
```javascript
function AsyncSubject() {
  __super__.call(this);
  this.isDisposed = false;
  this.isStopped = false;
  this.hasValue = false;
  this.observers = [];
  this.hasError = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject"></a>[function <span class="apidocSignatureSpan">rx.</span>BehaviorSubject (value)](#apidoc.element.rx.BehaviorSubject)
- description and source-code
```javascript
function BehaviorSubject(value) {
  __super__.call(this);
  this.value = value;
  this.observers = [];
  this.isDisposed = false;
  this.isStopped = false;
  this.hasError = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BinaryDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>BinaryDisposable (first, second)](#apidoc.element.rx.BinaryDisposable)
- description and source-code
```javascript
BinaryDisposable = function (first, second) {
  this._first = first;
  this._second = second;
  this.isDisposed = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.CompositeDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>CompositeDisposable ()](#apidoc.element.rx.CompositeDisposable)
- description and source-code
```javascript
CompositeDisposable = function () {
  var args = [], i, len;
  if (Array.isArray(arguments[0])) {
    args = arguments[0];
  } else {
    len = arguments.length;
    args = new Array(len);
    for(i = 0; i < len; i++) { args[i] = arguments[i]; }
  }
  this.disposables = args;
  this.isDisposed = false;
  this.length = args.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.CompositeError"></a>[function <span class="apidocSignatureSpan">rx.</span>CompositeError (errors)](#apidoc.element.rx.CompositeError)
- description and source-code
```javascript
CompositeError = function (errors) {
  this.innerErrors = errors;
  this.message = 'This contains multiple errors. Check the innerErrors';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ConnectableObservable"></a>[function <span class="apidocSignatureSpan">rx.</span>ConnectableObservable (source, subject)](#apidoc.element.rx.ConnectableObservable)
- description and source-code
```javascript
function ConnectableObservable(source, subject) {
  this.source = source;
  this._connection = null;
  this._source = source.asObservable();
  this._subject = subject;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Disposable"></a>[function <span class="apidocSignatureSpan">rx.</span>Disposable (action)](#apidoc.element.rx.Disposable)
- description and source-code
```javascript
Disposable = function (action) {
  this.isDisposed = false;
  this.action = action || noop;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.EmptyError"></a>[function <span class="apidocSignatureSpan">rx.</span>EmptyError ()](#apidoc.element.rx.EmptyError)
- description and source-code
```javascript
EmptyError = function () {
  this.message = 'Sequence contains no elements.';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.FlatMapObservable"></a>[function <span class="apidocSignatureSpan">rx.</span>FlatMapObservable (source, selector, resultSelector, thisArg)](#apidoc.element.rx.FlatMapObservable)
- description and source-code
```javascript
function FlatMapObservable(source, selector, resultSelector, thisArg) {
  this.resultSelector = isFunction(resultSelector) ? resultSelector : null;
  this.selector = bindCallback(isFunction(selector) ? selector : function() { return selector; }, thisArg, 3);
  this.source = source;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.HistoricalScheduler"></a>[function <span class="apidocSignatureSpan">rx.</span>HistoricalScheduler (initialClock, comparer)](#apidoc.element.rx.HistoricalScheduler)
- description and source-code
```javascript
function HistoricalScheduler(initialClock, comparer) {
  var clock = initialClock == null ? 0 : initialClock;
  var cmp = comparer || defaultSubComparer;
  __super__.call(this, clock, cmp);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.MockDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>MockDisposable (scheduler)](#apidoc.element.rx.MockDisposable)
- description and source-code
```javascript
MockDisposable = function (scheduler) {
  this.scheduler = scheduler;
  this.disposes = [];
  this.disposes.push(this.scheduler.clock);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.NAryDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>NAryDisposable (disposables)](#apidoc.element.rx.NAryDisposable)
- description and source-code
```javascript
NAryDisposable = function (disposables) {
  this._disposables = disposables;
  this.isDisposed = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.NotImplementedError"></a>[function <span class="apidocSignatureSpan">rx.</span>NotImplementedError (message)](#apidoc.element.rx.NotImplementedError)
- description and source-code
```javascript
NotImplementedError = function (message) {
  this.message = message || 'This operation is not implemented';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.NotSupportedError"></a>[function <span class="apidocSignatureSpan">rx.</span>NotSupportedError (message)](#apidoc.element.rx.NotSupportedError)
- description and source-code
```javascript
NotSupportedError = function (message) {
  this.message = message || 'This operation is not supported';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Notification"></a>[function <span class="apidocSignatureSpan">rx.</span>Notification ()](#apidoc.element.rx.Notification)
- description and source-code
```javascript
function Notification() {

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ObjectDisposedError"></a>[function <span class="apidocSignatureSpan">rx.</span>ObjectDisposedError ()](#apidoc.element.rx.ObjectDisposedError)
- description and source-code
```javascript
ObjectDisposedError = function () {
  this.message = 'Object has been disposed';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable"></a>[function <span class="apidocSignatureSpan">rx.</span>Observable ()](#apidoc.element.rx.Observable)
- description and source-code
```javascript
function Observable() {
  if (Rx.config.longStackSupport && hasStacks) {
    var oldSubscribe = this._subscribe;
    var e = tryCatch(thrower)(new Error()).e;
    this.stack = e.stack.substring(e.stack.indexOf('\n') + 1);
    this._subscribe = makeSubscribe(this, oldSubscribe);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ObservableBase"></a>[function <span class="apidocSignatureSpan">rx.</span>ObservableBase ()](#apidoc.element.rx.ObservableBase)
- description and source-code
```javascript
function ObservableBase() {
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observer"></a>[function <span class="apidocSignatureSpan">rx.</span>Observer ()](#apidoc.element.rx.Observer)
- description and source-code
```javascript
Observer = function () { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Pauser"></a>[function <span class="apidocSignatureSpan">rx.</span>Pauser ()](#apidoc.element.rx.Pauser)
- description and source-code
```javascript
function Pauser() {
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Recorded"></a>[function <span class="apidocSignatureSpan">rx.</span>Recorded (time, value, comparer)](#apidoc.element.rx.Recorded)
- description and source-code
```javascript
Recorded = function (time, value, comparer) {
  this.time = time;
  this.value = value;
  this.comparer = comparer || defaultComparer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.RefCountDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>RefCountDisposable (disposable)](#apidoc.element.rx.RefCountDisposable)
- description and source-code
```javascript
function RefCountDisposable(disposable) {
  this.underlyingDisposable = disposable;
  this.isDisposed = false;
  this.isPrimaryDisposed = false;
  this.count = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject"></a>[function <span class="apidocSignatureSpan">rx.</span>ReplaySubject (bufferSize, windowSize, scheduler)](#apidoc.element.rx.ReplaySubject)
- description and source-code
```javascript
function ReplaySubject(bufferSize, windowSize, scheduler) {
  this.bufferSize = bufferSize == null ? maxSafeInteger : bufferSize;
  this.windowSize = windowSize == null ? maxSafeInteger : windowSize;
  this.scheduler = scheduler || currentThreadScheduler;
  this.q = [];
  this.observers = [];
  this.isStopped = false;
  this.isDisposed = false;
  this.hasError = false;
  this.error = null;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler"></a>[function <span class="apidocSignatureSpan">rx.</span>Scheduler ()](#apidoc.element.rx.Scheduler)
- description and source-code
```javascript
function Scheduler() { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.SerialDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>SerialDisposable ()](#apidoc.element.rx.SerialDisposable)
- description and source-code
```javascript
SerialDisposable = function () {
  this.isDisposed = false;
  this.current = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.SingleAssignmentDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>SingleAssignmentDisposable ()](#apidoc.element.rx.SingleAssignmentDisposable)
- description and source-code
```javascript
SingleAssignmentDisposable = function () {
  this.isDisposed = false;
  this.current = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject"></a>[function <span class="apidocSignatureSpan">rx.</span>Subject ()](#apidoc.element.rx.Subject)
- description and source-code
```javascript
function Subject() {
  __super__.call(this);
  this.isDisposed = false;
  this.isStopped = false;
  this.observers = [];
  this.hasError = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subscription"></a>[function <span class="apidocSignatureSpan">rx.</span>Subscription (start, end)](#apidoc.element.rx.Subscription)
- description and source-code
```javascript
Subscription = function (start, end) {
  this.subscribe = start;
  this.unsubscribe = end || Number.MAX_VALUE;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler"></a>[function <span class="apidocSignatureSpan">rx.</span>TestScheduler ()](#apidoc.element.rx.TestScheduler)
- description and source-code
```javascript
function TestScheduler() {
  __super__.call(this, 0, baseComparer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TimeoutError"></a>[function <span class="apidocSignatureSpan">rx.</span>TimeoutError (message)](#apidoc.element.rx.TimeoutError)
- description and source-code
```javascript
TimeoutError = function (message) {
  this.message = message || 'Timeout has occurred';
  this.name = 'TimeoutError';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler"></a>[function <span class="apidocSignatureSpan">rx.</span>VirtualTimeScheduler (initialClock, comparer)](#apidoc.element.rx.VirtualTimeScheduler)
- description and source-code
```javascript
function VirtualTimeScheduler(initialClock, comparer) {
  this.clock = initialClock;
  this.comparer = comparer;
  this.isEnabled = false;
  this.queue = new PriorityQueue(1024);
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.AbstractObserver"></a>[function <span class="apidocSignatureSpan">rx.</span>internals.AbstractObserver ()](#apidoc.element.rx.internals.AbstractObserver)
- description and source-code
```javascript
function AbstractObserver() {
  this.isStopped = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.Enumerable"></a>[function <span class="apidocSignatureSpan">rx.</span>internals.Enumerable ()](#apidoc.element.rx.internals.Enumerable)
- description and source-code
```javascript
internals.Enumerable = function () { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.PriorityQueue"></a>[function <span class="apidocSignatureSpan">rx.</span>internals.PriorityQueue (capacity)](#apidoc.element.rx.internals.PriorityQueue)
- description and source-code
```javascript
internals.PriorityQueue = function (capacity) {
  this.items = new Array(capacity);
  this.length = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.SchedulePeriodicRecursive"></a>[function <span class="apidocSignatureSpan">rx.</span>internals.SchedulePeriodicRecursive (scheduler, state, period, action)](#apidoc.element.rx.internals.SchedulePeriodicRecursive)
- description and source-code
```javascript
function SchedulePeriodicRecursive(scheduler, state, period, action) {
  this._scheduler = scheduler;
  this._state = state;
  this._period = period;
  this._action = action;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledItem"></a>[function <span class="apidocSignatureSpan">rx.</span>internals.ScheduledItem (scheduler, state, action, dueTime, comparer)](#apidoc.element.rx.internals.ScheduledItem)
- description and source-code
```javascript
internals.ScheduledItem = function (scheduler, state, action, dueTime, comparer) {
  this.scheduler = scheduler;
  this.state = state;
  this.action = action;
  this.dueTime = dueTime;
  this.comparer = comparer || defaultSubComparer;
  this.disposable = new SingleAssignmentDisposable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledObserver"></a>[function <span class="apidocSignatureSpan">rx.</span>internals.ScheduledObserver (scheduler, observer)](#apidoc.element.rx.internals.ScheduledObserver)
- description and source-code
```javascript
function ScheduledObserver(scheduler, observer) {
  __super__.call(this);
  this.scheduler = scheduler;
  this.observer = observer;
  this.isAcquired = false;
  this.hasFaulted = false;
  this.queue = [];
  this.disposable = new SerialDisposable();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.AnonymousObservable"></a>[module rx.AnonymousObservable](#apidoc.module.rx.AnonymousObservable)

#### <a name="apidoc.element.rx.AnonymousObservable.AnonymousObservable"></a>[function <span class="apidocSignatureSpan">rx.</span>AnonymousObservable (subscribe, parent)](#apidoc.element.rx.AnonymousObservable.AnonymousObservable)
- description and source-code
```javascript
function AnonymousObservable(subscribe, parent) {
  this.source = parent;
  this.__subscribe = subscribe;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.AnonymousObservable.prototype"></a>[module rx.AnonymousObservable.prototype](#apidoc.module.rx.AnonymousObservable.prototype)

#### <a name="apidoc.element.rx.AnonymousObservable.prototype._subscribe"></a>[function <span class="apidocSignatureSpan">rx.AnonymousObservable.prototype.</span>_subscribe (o)](#apidoc.element.rx.AnonymousObservable.prototype._subscribe)
- description and source-code
```javascript
_subscribe = function (o) {
  var ado = new AutoDetachObserver(o), state = [ado, this];

  if (currentThreadScheduler.scheduleRequired()) {
    currentThreadScheduler.schedule(state, setDisposable);
  } else {
    setDisposable(null, state);
  }
  return ado;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousObservable.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.AnonymousObservable.prototype.</span>constructor (subscribe, parent)](#apidoc.element.rx.AnonymousObservable.prototype.constructor)
- description and source-code
```javascript
function AnonymousObservable(subscribe, parent) {
  this.source = parent;
  this.__subscribe = subscribe;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.AnonymousObserver"></a>[module rx.AnonymousObserver](#apidoc.module.rx.AnonymousObserver)

#### <a name="apidoc.element.rx.AnonymousObserver.AnonymousObserver"></a>[function <span class="apidocSignatureSpan">rx.</span>AnonymousObserver (onNext, onError, onCompleted)](#apidoc.element.rx.AnonymousObserver.AnonymousObserver)
- description and source-code
```javascript
function AnonymousObserver(onNext, onError, onCompleted) {
  __super__.call(this);
  this._onNext = onNext;
  this._onError = onError;
  this._onCompleted = onCompleted;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.AnonymousObserver.prototype"></a>[module rx.AnonymousObserver.prototype](#apidoc.module.rx.AnonymousObserver.prototype)

#### <a name="apidoc.element.rx.AnonymousObserver.prototype.completed"></a>[function <span class="apidocSignatureSpan">rx.AnonymousObserver.prototype.</span>completed ()](#apidoc.element.rx.AnonymousObserver.prototype.completed)
- description and source-code
```javascript
completed = function () {
  this._onCompleted();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousObserver.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.AnonymousObserver.prototype.</span>constructor (onNext, onError, onCompleted)](#apidoc.element.rx.AnonymousObserver.prototype.constructor)
- description and source-code
```javascript
function AnonymousObserver(onNext, onError, onCompleted) {
  __super__.call(this);
  this._onNext = onNext;
  this._onError = onError;
  this._onCompleted = onCompleted;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousObserver.prototype.error"></a>[function <span class="apidocSignatureSpan">rx.AnonymousObserver.prototype.</span>error (error)](#apidoc.element.rx.AnonymousObserver.prototype.error)
- description and source-code
```javascript
error = function (error) {
  this._onError(error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousObserver.prototype.next"></a>[function <span class="apidocSignatureSpan">rx.AnonymousObserver.prototype.</span>next (value)](#apidoc.element.rx.AnonymousObserver.prototype.next)
- description and source-code
```javascript
next = function (value) {
  this._onNext(value);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.AnonymousSubject"></a>[module rx.AnonymousSubject](#apidoc.module.rx.AnonymousSubject)

#### <a name="apidoc.element.rx.AnonymousSubject.AnonymousSubject"></a>[function <span class="apidocSignatureSpan">rx.</span>AnonymousSubject (observer, observable)](#apidoc.element.rx.AnonymousSubject.AnonymousSubject)
- description and source-code
```javascript
function AnonymousSubject(observer, observable) {
  this.observer = observer;
  this.observable = observable;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.AnonymousSubject.prototype"></a>[module rx.AnonymousSubject.prototype](#apidoc.module.rx.AnonymousSubject.prototype)

#### <a name="apidoc.element.rx.AnonymousSubject.prototype._subscribe"></a>[function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>_subscribe (o)](#apidoc.element.rx.AnonymousSubject.prototype._subscribe)
- description and source-code
```javascript
_subscribe = function (o) {
  return this.observable.subscribe(o);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousSubject.prototype.asObserver"></a>[function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>asObserver ()](#apidoc.element.rx.AnonymousSubject.prototype.asObserver)
- description and source-code
```javascript
asObserver = function () {
  var self = this;
  return new AnonymousObserver(
    function (x) { self.onNext(x); },
    function (err) { self.onError(err); },
    function () { self.onCompleted(); });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousSubject.prototype.checked"></a>[function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>checked ()](#apidoc.element.rx.AnonymousSubject.prototype.checked)
- description and source-code
```javascript
checked = function () { return new CheckedObserver(this); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousSubject.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>constructor (observer, observable)](#apidoc.element.rx.AnonymousSubject.prototype.constructor)
- description and source-code
```javascript
function AnonymousSubject(observer, observable) {
  this.observer = observer;
  this.observable = observable;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousSubject.prototype.makeSafe"></a>[function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.AnonymousSubject.prototype.makeSafe)
- description and source-code
```javascript
makeSafe = function (disposable) {
  return new AnonymousSafeObserver(this._onNext, this._onError, this._onCompleted, disposable);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousSubject.prototype.notifyOn"></a>[function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.AnonymousSubject.prototype.notifyOn)
- description and source-code
```javascript
notifyOn = function (scheduler) {
  return new ObserveOnObserver(scheduler, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousSubject.prototype.onCompleted"></a>[function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>onCompleted ()](#apidoc.element.rx.AnonymousSubject.prototype.onCompleted)
- description and source-code
```javascript
onCompleted = function () {
  this.observer.onCompleted();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousSubject.prototype.onError"></a>[function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>onError (error)](#apidoc.element.rx.AnonymousSubject.prototype.onError)
- description and source-code
```javascript
onError = function (error) {
  this.observer.onError(error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousSubject.prototype.onNext"></a>[function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>onNext (value)](#apidoc.element.rx.AnonymousSubject.prototype.onNext)
- description and source-code
```javascript
onNext = function (value) {
  this.observer.onNext(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AnonymousSubject.prototype.toNotifier"></a>[function <span class="apidocSignatureSpan">rx.AnonymousSubject.prototype.</span>toNotifier ()](#apidoc.element.rx.AnonymousSubject.prototype.toNotifier)
- description and source-code
```javascript
toNotifier = function () {
  var observer = this;
  return function (n) { return n.accept(observer); };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.AsyncSubject"></a>[module rx.AsyncSubject](#apidoc.module.rx.AsyncSubject)

#### <a name="apidoc.element.rx.AsyncSubject.AsyncSubject"></a>[function <span class="apidocSignatureSpan">rx.</span>AsyncSubject ()](#apidoc.element.rx.AsyncSubject.AsyncSubject)
- description and source-code
```javascript
function AsyncSubject() {
  __super__.call(this);
  this.isDisposed = false;
  this.isStopped = false;
  this.hasValue = false;
  this.observers = [];
  this.hasError = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.AsyncSubject.prototype"></a>[module rx.AsyncSubject.prototype](#apidoc.module.rx.AsyncSubject.prototype)

#### <a name="apidoc.element.rx.AsyncSubject.prototype._subscribe"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>_subscribe (o)](#apidoc.element.rx.AsyncSubject.prototype._subscribe)
- description and source-code
```javascript
_subscribe = function (o) {
  checkDisposed(this);

  if (!this.isStopped) {
    this.observers.push(o);
    return new InnerSubscription(this, o);
  }

  if (this.hasError) {
    o.onError(this.error);
  } else if (this.hasValue) {
    o.onNext(this.value);
    o.onCompleted();
  } else {
    o.onCompleted();
  }

  return disposableEmpty;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.asObserver"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>asObserver ()](#apidoc.element.rx.AsyncSubject.prototype.asObserver)
- description and source-code
```javascript
asObserver = function () {
  var self = this;
  return new AnonymousObserver(
    function (x) { self.onNext(x); },
    function (err) { self.onError(err); },
    function () { self.onCompleted(); });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.checked"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>checked ()](#apidoc.element.rx.AsyncSubject.prototype.checked)
- description and source-code
```javascript
checked = function () { return new CheckedObserver(this); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>constructor ()](#apidoc.element.rx.AsyncSubject.prototype.constructor)
- description and source-code
```javascript
function AsyncSubject() {
  __super__.call(this);
  this.isDisposed = false;
  this.isStopped = false;
  this.hasValue = false;
  this.observers = [];
  this.hasError = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>dispose ()](#apidoc.element.rx.AsyncSubject.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  this.isDisposed = true;
  this.observers = null;
  this.error = null;
  this.value = null;
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.hasObservers"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>hasObservers ()](#apidoc.element.rx.AsyncSubject.prototype.hasObservers)
- description and source-code
```javascript
hasObservers = function () { checkDisposed(this); return this.observers.length > 0; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.makeSafe"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.AsyncSubject.prototype.makeSafe)
- description and source-code
```javascript
makeSafe = function (disposable) {
  return new AnonymousSafeObserver(this._onNext, this._onError, this._onCompleted, disposable);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.notifyOn"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.AsyncSubject.prototype.notifyOn)
- description and source-code
```javascript
notifyOn = function (scheduler) {
  return new ObserveOnObserver(scheduler, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.onCompleted"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>onCompleted ()](#apidoc.element.rx.AsyncSubject.prototype.onCompleted)
- description and source-code
```javascript
onCompleted = function () {
  var i, len;
  checkDisposed(this);
  if (!this.isStopped) {
    this.isStopped = true;
    var os = cloneArray(this.observers), len = os.length;

    if (this.hasValue) {
      for (i = 0; i < len; i++) {
        var o = os[i];
        o.onNext(this.value);
        o.onCompleted();
      }
    } else {
      for (i = 0; i < len; i++) {
        os[i].onCompleted();
      }
    }

    this.observers.length = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.onError"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>onError (error)](#apidoc.element.rx.AsyncSubject.prototype.onError)
- description and source-code
```javascript
onError = function (error) {
  checkDisposed(this);
  if (!this.isStopped) {
    this.isStopped = true;
    this.hasError = true;
    this.error = error;

    for (var i = 0, os = cloneArray(this.observers), len = os.length; i < len; i++) {
      os[i].onError(error);
    }

    this.observers.length = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.onNext"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>onNext (value)](#apidoc.element.rx.AsyncSubject.prototype.onNext)
- description and source-code
```javascript
onNext = function (value) {
  checkDisposed(this);
  if (this.isStopped) { return; }
  this.value = value;
  this.hasValue = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.AsyncSubject.prototype.toNotifier"></a>[function <span class="apidocSignatureSpan">rx.AsyncSubject.prototype.</span>toNotifier ()](#apidoc.element.rx.AsyncSubject.prototype.toNotifier)
- description and source-code
```javascript
toNotifier = function () {
  var observer = this;
  return function (n) { return n.accept(observer); };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.BehaviorSubject"></a>[module rx.BehaviorSubject](#apidoc.module.rx.BehaviorSubject)

#### <a name="apidoc.element.rx.BehaviorSubject.BehaviorSubject"></a>[function <span class="apidocSignatureSpan">rx.</span>BehaviorSubject (value)](#apidoc.element.rx.BehaviorSubject.BehaviorSubject)
- description and source-code
```javascript
function BehaviorSubject(value) {
  __super__.call(this);
  this.value = value;
  this.observers = [];
  this.isDisposed = false;
  this.isStopped = false;
  this.hasError = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.BehaviorSubject.prototype"></a>[module rx.BehaviorSubject.prototype](#apidoc.module.rx.BehaviorSubject.prototype)

#### <a name="apidoc.element.rx.BehaviorSubject.prototype._subscribe"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>_subscribe (o)](#apidoc.element.rx.BehaviorSubject.prototype._subscribe)
- description and source-code
```javascript
_subscribe = function (o) {
  checkDisposed(this);
  if (!this.isStopped) {
    this.observers.push(o);
    o.onNext(this.value);
    return new InnerSubscription(this, o);
  }
  if (this.hasError) {
    o.onError(this.error);
  } else {
    o.onCompleted();
  }
  return disposableEmpty;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.asObserver"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>asObserver ()](#apidoc.element.rx.BehaviorSubject.prototype.asObserver)
- description and source-code
```javascript
asObserver = function () {
  var self = this;
  return new AnonymousObserver(
    function (x) { self.onNext(x); },
    function (err) { self.onError(err); },
    function () { self.onCompleted(); });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.checked"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>checked ()](#apidoc.element.rx.BehaviorSubject.prototype.checked)
- description and source-code
```javascript
checked = function () { return new CheckedObserver(this); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>constructor (value)](#apidoc.element.rx.BehaviorSubject.prototype.constructor)
- description and source-code
```javascript
function BehaviorSubject(value) {
  __super__.call(this);
  this.value = value;
  this.observers = [];
  this.isDisposed = false;
  this.isStopped = false;
  this.hasError = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>dispose ()](#apidoc.element.rx.BehaviorSubject.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  this.isDisposed = true;
  this.observers = null;
  this.value = null;
  this.error = null;
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.getValue"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>getValue ()](#apidoc.element.rx.BehaviorSubject.prototype.getValue)
- description and source-code
```javascript
getValue = function () {
  checkDisposed(this);
  if (this.hasError) { thrower(this.error); }
  return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.hasObservers"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>hasObservers ()](#apidoc.element.rx.BehaviorSubject.prototype.hasObservers)
- description and source-code
```javascript
hasObservers = function () { checkDisposed(this); return this.observers.length > 0; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.makeSafe"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.BehaviorSubject.prototype.makeSafe)
- description and source-code
```javascript
makeSafe = function (disposable) {
  return new AnonymousSafeObserver(this._onNext, this._onError, this._onCompleted, disposable);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.notifyOn"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.BehaviorSubject.prototype.notifyOn)
- description and source-code
```javascript
notifyOn = function (scheduler) {
  return new ObserveOnObserver(scheduler, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.onCompleted"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>onCompleted ()](#apidoc.element.rx.BehaviorSubject.prototype.onCompleted)
- description and source-code
```javascript
onCompleted = function () {
  checkDisposed(this);
  if (this.isStopped) { return; }
  this.isStopped = true;
  for (var i = 0, os = cloneArray(this.observers), len = os.length; i < len; i++) {
    os[i].onCompleted();
  }

  this.observers.length = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.onError"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>onError (error)](#apidoc.element.rx.BehaviorSubject.prototype.onError)
- description and source-code
```javascript
onError = function (error) {
  checkDisposed(this);
  if (this.isStopped) { return; }
  this.isStopped = true;
  this.hasError = true;
  this.error = error;

  for (var i = 0, os = cloneArray(this.observers), len = os.length; i < len; i++) {
    os[i].onError(error);
  }

  this.observers.length = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.onNext"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>onNext (value)](#apidoc.element.rx.BehaviorSubject.prototype.onNext)
- description and source-code
```javascript
onNext = function (value) {
  checkDisposed(this);
  if (this.isStopped) { return; }
  this.value = value;
  for (var i = 0, os = cloneArray(this.observers), len = os.length; i < len; i++) {
    os[i].onNext(value);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.BehaviorSubject.prototype.toNotifier"></a>[function <span class="apidocSignatureSpan">rx.BehaviorSubject.prototype.</span>toNotifier ()](#apidoc.element.rx.BehaviorSubject.prototype.toNotifier)
- description and source-code
```javascript
toNotifier = function () {
  var observer = this;
  return function (n) { return n.accept(observer); };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.BinaryDisposable"></a>[module rx.BinaryDisposable](#apidoc.module.rx.BinaryDisposable)

#### <a name="apidoc.element.rx.BinaryDisposable.BinaryDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>BinaryDisposable (first, second)](#apidoc.element.rx.BinaryDisposable.BinaryDisposable)
- description and source-code
```javascript
BinaryDisposable = function (first, second) {
  this._first = first;
  this._second = second;
  this.isDisposed = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.BinaryDisposable.prototype"></a>[module rx.BinaryDisposable.prototype](#apidoc.module.rx.BinaryDisposable.prototype)

#### <a name="apidoc.element.rx.BinaryDisposable.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.BinaryDisposable.prototype.</span>dispose ()](#apidoc.element.rx.BinaryDisposable.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  if (!this.isDisposed) {
    this.isDisposed = true;
    var old1 = this._first;
    this._first = null;
    old1 && old1.dispose();
    var old2 = this._second;
    this._second = null;
    old2 && old2.dispose();
  }
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```



# <a name="apidoc.module.rx.CompositeDisposable"></a>[module rx.CompositeDisposable](#apidoc.module.rx.CompositeDisposable)

#### <a name="apidoc.element.rx.CompositeDisposable.CompositeDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>CompositeDisposable ()](#apidoc.element.rx.CompositeDisposable.CompositeDisposable)
- description and source-code
```javascript
CompositeDisposable = function () {
  var args = [], i, len;
  if (Array.isArray(arguments[0])) {
    args = arguments[0];
  } else {
    len = arguments.length;
    args = new Array(len);
    for(i = 0; i < len; i++) { args[i] = arguments[i]; }
  }
  this.disposables = args;
  this.isDisposed = false;
  this.length = args.length;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.CompositeDisposable.prototype"></a>[module rx.CompositeDisposable.prototype](#apidoc.module.rx.CompositeDisposable.prototype)

#### <a name="apidoc.element.rx.CompositeDisposable.prototype.add"></a>[function <span class="apidocSignatureSpan">rx.CompositeDisposable.prototype.</span>add (item)](#apidoc.element.rx.CompositeDisposable.prototype.add)
- description and source-code
```javascript
add = function (item) {
  if (this.isDisposed) {
    item.dispose();
  } else {
    this.disposables.push(item);
    this.length++;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.CompositeDisposable.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.CompositeDisposable.prototype.</span>dispose ()](#apidoc.element.rx.CompositeDisposable.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  if (!this.isDisposed) {
    this.isDisposed = true;
    var len = this.disposables.length, currentDisposables = new Array(len);
    for(var i = 0; i < len; i++) { currentDisposables[i] = this.disposables[i]; }
    this.disposables = [];
    this.length = 0;

    for (i = 0; i < len; i++) {
      currentDisposables[i].dispose();
    }
  }
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```

#### <a name="apidoc.element.rx.CompositeDisposable.prototype.remove"></a>[function <span class="apidocSignatureSpan">rx.CompositeDisposable.prototype.</span>remove (item)](#apidoc.element.rx.CompositeDisposable.prototype.remove)
- description and source-code
```javascript
remove = function (item) {
  var shouldDispose = false;
  if (!this.isDisposed) {
    var idx = this.disposables.indexOf(item);
    if (idx !== -1) {
      shouldDispose = true;
      this.disposables.splice(idx, 1);
      this.length--;
      item.dispose();
    }
  }
  return shouldDispose;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.ConnectableObservable"></a>[module rx.ConnectableObservable](#apidoc.module.rx.ConnectableObservable)

#### <a name="apidoc.element.rx.ConnectableObservable.ConnectableObservable"></a>[function <span class="apidocSignatureSpan">rx.</span>ConnectableObservable (source, subject)](#apidoc.element.rx.ConnectableObservable.ConnectableObservable)
- description and source-code
```javascript
function ConnectableObservable(source, subject) {
  this.source = source;
  this._connection = null;
  this._source = source.asObservable();
  this._subject = subject;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.ConnectableObservable.prototype"></a>[module rx.ConnectableObservable.prototype](#apidoc.module.rx.ConnectableObservable.prototype)

#### <a name="apidoc.element.rx.ConnectableObservable.prototype._subscribe"></a>[function <span class="apidocSignatureSpan">rx.ConnectableObservable.prototype.</span>_subscribe (o)](#apidoc.element.rx.ConnectableObservable.prototype._subscribe)
- description and source-code
```javascript
_subscribe = function (o) {
  return this._subject.subscribe(o);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ConnectableObservable.prototype.connect"></a>[function <span class="apidocSignatureSpan">rx.ConnectableObservable.prototype.</span>connect ()](#apidoc.element.rx.ConnectableObservable.prototype.connect)
- description and source-code
```javascript
connect = function () {
  if (!this._connection) {
    if (this._subject.isStopped) {
      return disposableEmpty;
    }
    var subscription = this._source.subscribe(this._subject);
    this._connection = new ConnectDisposable(this, subscription);
  }
  return this._connection;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ConnectableObservable.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.ConnectableObservable.prototype.</span>constructor (source, subject)](#apidoc.element.rx.ConnectableObservable.prototype.constructor)
- description and source-code
```javascript
function ConnectableObservable(source, subject) {
  this.source = source;
  this._connection = null;
  this._source = source.asObservable();
  this._subject = subject;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ConnectableObservable.prototype.refCount"></a>[function <span class="apidocSignatureSpan">rx.ConnectableObservable.prototype.</span>refCount ()](#apidoc.element.rx.ConnectableObservable.prototype.refCount)
- description and source-code
```javascript
refCount = function () {
  return new RefCountObservable(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Disposable"></a>[module rx.Disposable](#apidoc.module.rx.Disposable)

#### <a name="apidoc.element.rx.Disposable.Disposable"></a>[function <span class="apidocSignatureSpan">rx.</span>Disposable (action)](#apidoc.element.rx.Disposable.Disposable)
- description and source-code
```javascript
Disposable = function (action) {
  this.isDisposed = false;
  this.action = action || noop;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Disposable._fixup"></a>[function <span class="apidocSignatureSpan">rx.Disposable.</span>_fixup (result)](#apidoc.element.rx.Disposable._fixup)
- description and source-code
```javascript
_fixup = function (result) {
  return isDisposable(result) ? result : disposableEmpty;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Disposable.checkDisposed"></a>[function <span class="apidocSignatureSpan">rx.Disposable.</span>checkDisposed (disposable)](#apidoc.element.rx.Disposable.checkDisposed)
- description and source-code
```javascript
checkDisposed = function (disposable) {
  if (disposable.isDisposed) { throw new ObjectDisposedError(); }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Disposable.create"></a>[function <span class="apidocSignatureSpan">rx.Disposable.</span>create (action)](#apidoc.element.rx.Disposable.create)
- description and source-code
```javascript
create = function (action) { return new Disposable(action); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Disposable.isDisposable"></a>[function <span class="apidocSignatureSpan">rx.Disposable.</span>isDisposable (d)](#apidoc.element.rx.Disposable.isDisposable)
- description and source-code
```javascript
isDisposable = function (d) {
  return d && isFunction(d.dispose);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Disposable.empty"></a>[module rx.Disposable.empty](#apidoc.module.rx.Disposable.empty)

#### <a name="apidoc.element.rx.Disposable.empty.dispose"></a>[function <span class="apidocSignatureSpan">rx.Disposable.empty.</span>dispose ()](#apidoc.element.rx.Disposable.empty.dispose)
- description and source-code
```javascript
dispose = function () { }
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```



# <a name="apidoc.module.rx.Disposable.prototype"></a>[module rx.Disposable.prototype](#apidoc.module.rx.Disposable.prototype)

#### <a name="apidoc.element.rx.Disposable.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.Disposable.prototype.</span>dispose ()](#apidoc.element.rx.Disposable.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  if (!this.isDisposed) {
    this.action();
    this.isDisposed = true;
  }
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```



# <a name="apidoc.module.rx.FlatMapObservable"></a>[module rx.FlatMapObservable](#apidoc.module.rx.FlatMapObservable)

#### <a name="apidoc.element.rx.FlatMapObservable.FlatMapObservable"></a>[function <span class="apidocSignatureSpan">rx.</span>FlatMapObservable (source, selector, resultSelector, thisArg)](#apidoc.element.rx.FlatMapObservable.FlatMapObservable)
- description and source-code
```javascript
function FlatMapObservable(source, selector, resultSelector, thisArg) {
  this.resultSelector = isFunction(resultSelector) ? resultSelector : null;
  this.selector = bindCallback(isFunction(selector) ? selector : function() { return selector; }, thisArg, 3);
  this.source = source;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.FlatMapObservable.prototype"></a>[module rx.FlatMapObservable.prototype](#apidoc.module.rx.FlatMapObservable.prototype)

#### <a name="apidoc.element.rx.FlatMapObservable.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.FlatMapObservable.prototype.</span>constructor (source, selector, resultSelector, thisArg)](#apidoc.element.rx.FlatMapObservable.prototype.constructor)
- description and source-code
```javascript
function FlatMapObservable(source, selector, resultSelector, thisArg) {
  this.resultSelector = isFunction(resultSelector) ? resultSelector : null;
  this.selector = bindCallback(isFunction(selector) ? selector : function() { return selector; }, thisArg, 3);
  this.source = source;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.FlatMapObservable.prototype.subscribeCore"></a>[function <span class="apidocSignatureSpan">rx.FlatMapObservable.prototype.</span>subscribeCore (o)](#apidoc.element.rx.FlatMapObservable.prototype.subscribeCore)
- description and source-code
```javascript
subscribeCore = function (o) {
  return this.source.subscribe(new InnerObserver(o, this.selector, this.resultSelector, this));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.HistoricalScheduler"></a>[module rx.HistoricalScheduler](#apidoc.module.rx.HistoricalScheduler)

#### <a name="apidoc.element.rx.HistoricalScheduler.HistoricalScheduler"></a>[function <span class="apidocSignatureSpan">rx.</span>HistoricalScheduler (initialClock, comparer)](#apidoc.element.rx.HistoricalScheduler.HistoricalScheduler)
- description and source-code
```javascript
function HistoricalScheduler(initialClock, comparer) {
  var clock = initialClock == null ? 0 : initialClock;
  var cmp = comparer || defaultSubComparer;
  __super__.call(this, clock, cmp);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.HistoricalScheduler.prototype"></a>[module rx.HistoricalScheduler.prototype](#apidoc.module.rx.HistoricalScheduler.prototype)

#### <a name="apidoc.element.rx.HistoricalScheduler.prototype.add"></a>[function <span class="apidocSignatureSpan">rx.HistoricalScheduler.prototype.</span>add (absolute, relative)](#apidoc.element.rx.HistoricalScheduler.prototype.add)
- description and source-code
```javascript
add = function (absolute, relative) {
  return absolute + relative;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.HistoricalScheduler.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.HistoricalScheduler.prototype.</span>constructor (initialClock, comparer)](#apidoc.element.rx.HistoricalScheduler.prototype.constructor)
- description and source-code
```javascript
function HistoricalScheduler(initialClock, comparer) {
  var clock = initialClock == null ? 0 : initialClock;
  var cmp = comparer || defaultSubComparer;
  __super__.call(this, clock, cmp);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.HistoricalScheduler.prototype.toAbsoluteTime"></a>[function <span class="apidocSignatureSpan">rx.HistoricalScheduler.prototype.</span>toAbsoluteTime (absolute)](#apidoc.element.rx.HistoricalScheduler.prototype.toAbsoluteTime)
- description and source-code
```javascript
toAbsoluteTime = function (absolute) {
  return new Date(absolute).getTime();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.HistoricalScheduler.prototype.toRelativeTime"></a>[function <span class="apidocSignatureSpan">rx.HistoricalScheduler.prototype.</span>toRelativeTime (timeSpan)](#apidoc.element.rx.HistoricalScheduler.prototype.toRelativeTime)
- description and source-code
```javascript
toRelativeTime = function (timeSpan) {
  return timeSpan;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.MockDisposable"></a>[module rx.MockDisposable](#apidoc.module.rx.MockDisposable)

#### <a name="apidoc.element.rx.MockDisposable.MockDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>MockDisposable (scheduler)](#apidoc.element.rx.MockDisposable.MockDisposable)
- description and source-code
```javascript
MockDisposable = function (scheduler) {
  this.scheduler = scheduler;
  this.disposes = [];
  this.disposes.push(this.scheduler.clock);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.MockDisposable.prototype"></a>[module rx.MockDisposable.prototype](#apidoc.module.rx.MockDisposable.prototype)

#### <a name="apidoc.element.rx.MockDisposable.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.MockDisposable.prototype.</span>dispose ()](#apidoc.element.rx.MockDisposable.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  this.disposes.push(this.scheduler.clock);
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```



# <a name="apidoc.module.rx.NAryDisposable"></a>[module rx.NAryDisposable](#apidoc.module.rx.NAryDisposable)

#### <a name="apidoc.element.rx.NAryDisposable.NAryDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>NAryDisposable (disposables)](#apidoc.element.rx.NAryDisposable.NAryDisposable)
- description and source-code
```javascript
NAryDisposable = function (disposables) {
  this._disposables = disposables;
  this.isDisposed = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.NAryDisposable.prototype"></a>[module rx.NAryDisposable.prototype](#apidoc.module.rx.NAryDisposable.prototype)

#### <a name="apidoc.element.rx.NAryDisposable.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.NAryDisposable.prototype.</span>dispose ()](#apidoc.element.rx.NAryDisposable.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  if (!this.isDisposed) {
    this.isDisposed = true;
    for (var i = 0, len = this._disposables.length; i < len; i++) {
      this._disposables[i].dispose();
    }
    this._disposables.length = 0;
  }
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```



# <a name="apidoc.module.rx.Notification"></a>[module rx.Notification](#apidoc.module.rx.Notification)

#### <a name="apidoc.element.rx.Notification.Notification"></a>[function <span class="apidocSignatureSpan">rx.</span>Notification ()](#apidoc.element.rx.Notification.Notification)
- description and source-code
```javascript
function Notification() {

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Notification.createOnCompleted"></a>[function <span class="apidocSignatureSpan">rx.Notification.</span>createOnCompleted ()](#apidoc.element.rx.Notification.createOnCompleted)
- description and source-code
```javascript
createOnCompleted = function () {
  return new OnCompletedNotification();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Notification.createOnError"></a>[function <span class="apidocSignatureSpan">rx.Notification.</span>createOnError (error)](#apidoc.element.rx.Notification.createOnError)
- description and source-code
```javascript
createOnError = function (error) {
  return new OnErrorNotification(error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Notification.createOnNext"></a>[function <span class="apidocSignatureSpan">rx.Notification.</span>createOnNext (value)](#apidoc.element.rx.Notification.createOnNext)
- description and source-code
```javascript
createOnNext = function (value) {
  return new OnNextNotification(value);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Notification.prototype"></a>[module rx.Notification.prototype](#apidoc.module.rx.Notification.prototype)

#### <a name="apidoc.element.rx.Notification.prototype._accept"></a>[function <span class="apidocSignatureSpan">rx.Notification.prototype.</span>_accept (onNext, onError, onCompleted)](#apidoc.element.rx.Notification.prototype._accept)
- description and source-code
```javascript
_accept = function (onNext, onError, onCompleted) {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Notification.prototype._acceptObserver"></a>[function <span class="apidocSignatureSpan">rx.Notification.prototype.</span>_acceptObserver (onNext, onError, onCompleted)](#apidoc.element.rx.Notification.prototype._acceptObserver)
- description and source-code
```javascript
_acceptObserver = function (onNext, onError, onCompleted) {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Notification.prototype.accept"></a>[function <span class="apidocSignatureSpan">rx.Notification.prototype.</span>accept (observerOrOnNext, onError, onCompleted)](#apidoc.element.rx.Notification.prototype.accept)
- description and source-code
```javascript
accept = function (observerOrOnNext, onError, onCompleted) {
  return observerOrOnNext && typeof observerOrOnNext === 'object' ?
    this._acceptObserver(observerOrOnNext) :
    this._accept(observerOrOnNext, onError, onCompleted);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Notification.prototype.toObservable"></a>[function <span class="apidocSignatureSpan">rx.Notification.prototype.</span>toObservable (scheduler)](#apidoc.element.rx.Notification.prototype.toObservable)
- description and source-code
```javascript
toObservable = function (scheduler) {
  var self = this;
  isScheduler(scheduler) || (scheduler = immediateScheduler);
  return new AnonymousObservable(function (o) {
    return scheduler.schedule(self, function (_, notification) {
      notification._acceptObserver(o);
      notification.kind === 'N' && o.onCompleted();
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Observable"></a>[module rx.Observable](#apidoc.module.rx.Observable)

#### <a name="apidoc.element.rx.Observable.Observable"></a>[function <span class="apidocSignatureSpan">rx.</span>Observable ()](#apidoc.element.rx.Observable.Observable)
- description and source-code
```javascript
function Observable() {
  if (Rx.config.longStackSupport && hasStacks) {
    var oldSubscribe = this._subscribe;
    var e = tryCatch(thrower)(new Error()).e;
    this.stack = e.stack.substring(e.stack.indexOf('\n') + 1);
    this._subscribe = makeSubscribe(this, oldSubscribe);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.amb"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>amb ()](#apidoc.element.rx.Observable.amb)
- description and source-code
```javascript
amb = function () {
  var acc = observableNever(), items;
  if (Array.isArray(arguments[0])) {
    items = arguments[0];
  } else {
    var len = arguments.length;
    items = new Array(items);
    for(var i = 0; i < len; i++) { items[i] = arguments[i]; }
  }
  for (var i = 0, len = items.length; i < len; i++) {
    acc = amb(acc, items[i]);
  }
  return acc;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.case"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>case (selector, sources, defaultSourceOrScheduler)](#apidoc.element.rx.Observable.case)
- description and source-code
```javascript
case = function (selector, sources, defaultSourceOrScheduler) {
  return observableDefer(function () {
    isPromise(defaultSourceOrScheduler) && (defaultSourceOrScheduler = observableFromPromise(defaultSourceOrScheduler));
    defaultSourceOrScheduler || (defaultSourceOrScheduler = observableEmpty());

    isScheduler(defaultSourceOrScheduler) && (defaultSourceOrScheduler = observableEmpty(defaultSourceOrScheduler));

    var result = sources[selector()];
    isPromise(result) && (result = observableFromPromise(result));

    return result || defaultSourceOrScheduler;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.catch"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>catch ()](#apidoc.element.rx.Observable.catch)
- description and source-code
```javascript
catch = function () {
  var items;
  if (Array.isArray(arguments[0])) {
    items = arguments[0];
  } else {
    var len = arguments.length;
    items = new Array(len);
    for(var i = 0; i < len; i++) { items[i] = arguments[i]; }
  }
  return enumerableOf(items).catchError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.combineLatest"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>combineLatest ()](#apidoc.element.rx.Observable.combineLatest)
- description and source-code
```javascript
combineLatest = function () {
  var len = arguments.length, args = new Array(len);
  for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  var resultSelector = isFunction(args[len - 1]) ? args.pop() : argumentsToArray;
  Array.isArray(args[0]) && (args = args[0]);
  return new CombineLatestObservable(args, resultSelector);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.concat"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>concat ()](#apidoc.element.rx.Observable.concat)
- description and source-code
```javascript
concat = function () {
  var args;
  if (Array.isArray(arguments[0])) {
    args = arguments[0];
  } else {
    args = new Array(arguments.length);
    for(var i = 0, len = arguments.length; i < len; i++) { args[i] = arguments[i]; }
  }
  return new ConcatObservable(args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.create"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>create (subscribe, parent)](#apidoc.element.rx.Observable.create)
- description and source-code
```javascript
create = function (subscribe, parent) {
  return new AnonymousObservable(subscribe, parent);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.defer"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>defer (observableFactory)](#apidoc.element.rx.Observable.defer)
- description and source-code
```javascript
defer = function (observableFactory) {
  return new Defer(observableFactory);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.empty"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>empty (scheduler)](#apidoc.element.rx.Observable.empty)
- description and source-code
```javascript
empty = function (scheduler) {
  isScheduler(scheduler) || (scheduler = immediateScheduler);
  return scheduler === immediateScheduler ? EMPTY_OBSERVABLE : new EmptyObservable(scheduler);
}
```
- example usage
```shell
...

Finally, we call the 'subscribe' method on our observable sequence to start pulling data.

'''js
suggestions.subscribe(
data => {
  $results
    .empty()
    .append($.map(data[1], value =>  $('<li>').text(value)))
},
error=> {
  $results
    .empty()
    .append($('<li>'))
      .text('Error:' + error);
...
```

#### <a name="apidoc.element.rx.Observable.for"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>for (sources, resultSelector, thisArg)](#apidoc.element.rx.Observable.for)
- description and source-code
```javascript
for = function (sources, resultSelector, thisArg) {
  return enumerableOf(sources, resultSelector, thisArg).concat();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.forIn"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>forIn (sources, resultSelector, thisArg)](#apidoc.element.rx.Observable.forIn)
- description and source-code
```javascript
forIn = function (sources, resultSelector, thisArg) {
  return enumerableOf(sources, resultSelector, thisArg).concat();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.forkJoin"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>forkJoin ()](#apidoc.element.rx.Observable.forkJoin)
- description and source-code
```javascript
forkJoin = function () {
  var len = arguments.length, args = new Array(len);
  for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  var resultSelector = isFunction(args[len - 1]) ? args.pop() : argumentsToArray;
  Array.isArray(args[0]) && (args = args[0]);
  return new ForkJoinObservable(args, resultSelector);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.from"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>from (iterable, mapFn, thisArg, scheduler)](#apidoc.element.rx.Observable.from)
- description and source-code
```javascript
from = function (iterable, mapFn, thisArg, scheduler) {
  if (iterable == null) {
    throw new Error('iterable cannot be null.')
  }
  if (mapFn && !isFunction(mapFn)) {
    throw new Error('mapFn when provided must be a function');
  }
  if (mapFn) {
    var mapper = bindCallback(mapFn, thisArg, 2);
  }
  isScheduler(scheduler) || (scheduler = currentThreadScheduler);
  return new FromObservable(iterable, mapper, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.fromArray"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>fromArray (array, scheduler)](#apidoc.element.rx.Observable.fromArray)
- description and source-code
```javascript
fromArray = function (array, scheduler) {
  isScheduler(scheduler) || (scheduler = currentThreadScheduler);
  return new FromArrayObservable(array, scheduler)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.fromCallback"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>fromCallback (fn, ctx, selector)](#apidoc.element.rx.Observable.fromCallback)
- description and source-code
```javascript
fromCallback = function (fn, ctx, selector) {
  return function () {
    typeof ctx === 'undefined' && (ctx = this);

    var len = arguments.length, args = new Array(len)
    for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
    return createCbObservable(fn, ctx, selector, args);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.fromEvent"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>fromEvent (element, eventName, selector)](#apidoc.element.rx.Observable.fromEvent)
- description and source-code
```javascript
fromEvent = function (element, eventName, selector) {
  // Node.js specific
  if (element.addListener) {
    return fromEventPattern(
      function (h) { element.addListener(eventName, h); },
      function (h) { element.removeListener(eventName, h); },
      selector);
  }

  // Use only if non-native events are allowed
  if (!Rx.config.useNativeEvents) {
    // Handles jq, Angular.js, Zepto, Marionette, Ember.js
    if (typeof element.on === 'function' && typeof element.off === 'function') {
      return fromEventPattern(
        function (h) { element.on(eventName, h); },
        function (h) { element.off(eventName, h); },
        selector);
    }
  }

  return new EventObservable(element, eventName, selector).publish().refCount();
}
```
- example usage
```shell
...
Next, we'll get the user input from an input, listening to the keyup event by using the 'Rx.Observable.fromEvent' method.  This
will either use the event binding from [jQuery](http://jquery.com), [Zepto](http://zeptojs.com/), [AngularJS](https://angularjs.
org/), [Backbone.js](http://backbonejs.org/) and [Ember.js](http://emberjs.com/) if available, and if not, falls back to the native
 event binding.  This gives you consistent ways of thinking of events depending on your framework, so there are no surprises.

'''js
const $input = $('#input');
const $results = $('#results');

/* Only get the value from each key up */
var keyups = Rx.Observable.fromEvent($input, 'keyup')
.pluck('target', 'value')
.filter(text => text.length > 2 );

/* Now debounce the input for 500ms */
var debounced = keyups
.debounce(500 /* ms */);
...
```

#### <a name="apidoc.element.rx.Observable.fromEventPattern"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>fromEventPattern (addHandler, removeHandler, selector)](#apidoc.element.rx.Observable.fromEventPattern)
- description and source-code
```javascript
fromEventPattern = function (addHandler, removeHandler, selector) {
  return new EventPatternObservable(addHandler, removeHandler, selector).publish().refCount();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.fromNodeCallback"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>fromNodeCallback (fn, ctx, selector)](#apidoc.element.rx.Observable.fromNodeCallback)
- description and source-code
```javascript
fromNodeCallback = function (fn, ctx, selector) {
  return function () {
    typeof ctx === 'undefined' && (ctx = this);
    var len = arguments.length, args = new Array(len);
    for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
    return createNodeObservable(fn, ctx, selector, args);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.fromPromise"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>fromPromise (promise, scheduler)](#apidoc.element.rx.Observable.fromPromise)
- description and source-code
```javascript
fromPromise = function (promise, scheduler) {
  scheduler || (scheduler = defaultScheduler);
  return new FromPromiseObservable(promise, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.generate"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>generate (initialState, condition, iterate, resultSelector, scheduler)](#apidoc.element.rx.Observable.generate)
- description and source-code
```javascript
generate = function (initialState, condition, iterate, resultSelector, scheduler) {
  isScheduler(scheduler) || (scheduler = currentThreadScheduler);
  return new GenerateObservable(initialState, condition, iterate, resultSelector, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.generateWithAbsoluteTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>generateWithAbsoluteTime (initialState, condition, iterate, resultSelector, timeSelector, scheduler)](#apidoc.element.rx.Observable.generateWithAbsoluteTime)
- description and source-code
```javascript
generateWithAbsoluteTime = function (initialState, condition, iterate, resultSelector, timeSelector, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new GenerateAbsoluteObservable(initialState, condition, iterate, resultSelector, timeSelector, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.generateWithRelativeTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>generateWithRelativeTime (initialState, condition, iterate, resultSelector, timeSelector, scheduler)](#apidoc.element.rx.Observable.generateWithRelativeTime)
- description and source-code
```javascript
generateWithRelativeTime = function (initialState, condition, iterate, resultSelector, timeSelector, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new GenerateRelativeObservable(initialState, condition, iterate, resultSelector, timeSelector, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.if"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>if (condition, thenSource, elseSourceOrScheduler)](#apidoc.element.rx.Observable.if)
- description and source-code
```javascript
if = function (condition, thenSource, elseSourceOrScheduler) {
  return observableDefer(function () {
    elseSourceOrScheduler || (elseSourceOrScheduler = observableEmpty());

    isPromise(thenSource) && (thenSource = observableFromPromise(thenSource));
    isPromise(elseSourceOrScheduler) && (elseSourceOrScheduler = observableFromPromise(elseSourceOrScheduler));

    // Assume a scheduler for empty only
    typeof elseSourceOrScheduler.now === 'function' && (elseSourceOrScheduler = observableEmpty(elseSourceOrScheduler));
    return condition() ? thenSource : elseSourceOrScheduler;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.interval"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>interval (period, scheduler)](#apidoc.element.rx.Observable.interval)
- description and source-code
```javascript
interval = function (period, scheduler) {
  return observableTimerTimeSpanAndPeriod(period, period, isScheduler(scheduler) ? scheduler : defaultScheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.isObservable"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>isObservable (o)](#apidoc.element.rx.Observable.isObservable)
- description and source-code
```javascript
isObservable = function (o) {
  return o && isFunction(o.subscribe);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.just"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>just (value, scheduler)](#apidoc.element.rx.Observable.just)
- description and source-code
```javascript
just = function (value, scheduler) {
  isScheduler(scheduler) || (scheduler = immediateScheduler);
  return new JustObservable(value, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.merge"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>merge ()](#apidoc.element.rx.Observable.merge)
- description and source-code
```javascript
merge = function () {
  var scheduler, sources = [], i, len = arguments.length;
  if (!arguments[0]) {
    scheduler = immediateScheduler;
    for(i = 1; i < len; i++) { sources.push(arguments[i]); }
  } else if (isScheduler(arguments[0])) {
    scheduler = arguments[0];
    for(i = 1; i < len; i++) { sources.push(arguments[i]); }
  } else {
    scheduler = immediateScheduler;
    for(i = 0; i < len; i++) { sources.push(arguments[i]); }
  }
  if (Array.isArray(sources[0])) {
    sources = sources[0];
  }
  return observableOf(scheduler, sources).mergeAll();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.mergeDelayError"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>mergeDelayError ()](#apidoc.element.rx.Observable.mergeDelayError)
- description and source-code
```javascript
mergeDelayError = function () {
  var args;
  if (Array.isArray(arguments[0])) {
    args = arguments[0];
  } else {
    var len = arguments.length;
    args = new Array(len);
    for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  }
  var source = observableOf(null, args);
  return new MergeDelayErrorObservable(source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.never"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>never ()](#apidoc.element.rx.Observable.never)
- description and source-code
```javascript
never = function () {
  return NEVER_OBSERVABLE;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.of"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>of ()](#apidoc.element.rx.Observable.of)
- description and source-code
```javascript
of = function () {
  var len = arguments.length, args = new Array(len);
  for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  return new FromArrayObservable(args, currentThreadScheduler);
}
```
- example usage
```shell
...
'''js
require({
  'paths': {
    'rx': 'path/to/rx-lite.js'
  }
},
['rx'], (Rx) => {
  const obs = Rx.Observable.of(42);
  obs.forEach(x => console.log(x));
});
'''

## What about my libraries? ##

The Reactive Extensions for JavaScript have no external dependencies on any library, so they'll work well with just about any library
.  We provide bridges and support for various libraries including:
...
```

#### <a name="apidoc.element.rx.Observable.ofWithScheduler"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>ofWithScheduler (scheduler)](#apidoc.element.rx.Observable.ofWithScheduler)
- description and source-code
```javascript
ofWithScheduler = function (scheduler) {
  var len = arguments.length, args = new Array(len - 1);
  for(var i = 1; i < len; i++) { args[i - 1] = arguments[i]; }
  return new FromArrayObservable(args, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.onErrorResumeNext"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>onErrorResumeNext ()](#apidoc.element.rx.Observable.onErrorResumeNext)
- description and source-code
```javascript
onErrorResumeNext = function () {
  var sources = [];
  if (Array.isArray(arguments[0])) {
    sources = arguments[0];
  } else {
    var len = arguments.length;
    sources = new Array(len);
    for(var i = 0; i < len; i++) { sources[i] = arguments[i]; }
  }
  return new OnErrorResumeNextObservable(sources);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.pairs"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>pairs (obj, scheduler)](#apidoc.element.rx.Observable.pairs)
- description and source-code
```javascript
pairs = function (obj, scheduler) {
  scheduler || (scheduler = currentThreadScheduler);
  return new PairsObservable(obj, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.range"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>range (start, count, scheduler)](#apidoc.element.rx.Observable.range)
- description and source-code
```javascript
range = function (start, count, scheduler) {
  isScheduler(scheduler) || (scheduler = currentThreadScheduler);
  return new RangeObservable(start, count, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.repeat"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>repeat (value, repeatCount, scheduler)](#apidoc.element.rx.Observable.repeat)
- description and source-code
```javascript
repeat = function (value, repeatCount, scheduler) {
  isScheduler(scheduler) || (scheduler = currentThreadScheduler);
  return new RepeatObservable(value, repeatCount, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.return"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>return (value, scheduler)](#apidoc.element.rx.Observable.return)
- description and source-code
```javascript
return = function (value, scheduler) {
  isScheduler(scheduler) || (scheduler = immediateScheduler);
  return new JustObservable(value, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.spawn"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>spawn ()](#apidoc.element.rx.Observable.spawn)
- description and source-code
```javascript
spawn = function () {
  var gen = arguments[0], self = this, args = [];
  for (var i = 1, len = arguments.length; i < len; i++) { args.push(arguments[i]); }

  return new AnonymousObservable(function (o) {
    var g = new CompositeDisposable();

    if (isFunction(gen)) { gen = gen.apply(self, args); }
    if (!gen || !isFunction(gen.next)) {
      o.onNext(gen);
      return o.onCompleted();
    }

    function processGenerator(res) {
      var ret = tryCatch(gen.next).call(gen, res);
      if (ret === errorObj) { return o.onError(ret.e); }
      next(ret);
    }

    processGenerator();

    function onError(err) {
      var ret = tryCatch(gen.next).call(gen, err);
      if (ret === errorObj) { return o.onError(ret.e); }
      next(ret);
    }

    function next(ret) {
      if (ret.done) {
        o.onNext(ret.value);
        o.onCompleted();
        return;
      }
      var obs = toObservable.call(self, ret.value);
      var value = null;
      var hasValue = false;
      if (Observable.isObservable(obs)) {
        g.add(obs.subscribe(function(val) {
          hasValue = true;
          value = val;
        }, onError, function() {
          hasValue && processGenerator(value);
        }));
      } else {
        onError(new TypeError('type not supported'));
      }
    }

    return g;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.start"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>start (func, context, scheduler)](#apidoc.element.rx.Observable.start)
- description and source-code
```javascript
start = function (func, context, scheduler) {
  return observableToAsync(func, context, scheduler)();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.startAsync"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>startAsync (functionAsync)](#apidoc.element.rx.Observable.startAsync)
- description and source-code
```javascript
startAsync = function (functionAsync) {
  var promise = tryCatch(functionAsync)();
  if (promise === errorObj) { return observableThrow(promise.e); }
  return observableFromPromise(promise);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.throw"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>throw (error, scheduler)](#apidoc.element.rx.Observable.throw)
- description and source-code
```javascript
throw = function (error, scheduler) {
  isScheduler(scheduler) || (scheduler = immediateScheduler);
  return new ThrowObservable(error, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.timer"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>timer (dueTime, periodOrScheduler, scheduler)](#apidoc.element.rx.Observable.timer)
- description and source-code
```javascript
timer = function (dueTime, periodOrScheduler, scheduler) {
  var period;
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  if (periodOrScheduler != null && typeof periodOrScheduler === 'number') {
    period = periodOrScheduler;
  } else if (isScheduler(periodOrScheduler)) {
    scheduler = periodOrScheduler;
  }
  if ((dueTime instanceof Date || typeof dueTime === 'number') && period === undefined) {
    return _observableTimer(dueTime, scheduler);
  }
  if (dueTime instanceof Date && period !== undefined) {
    return observableTimerDateAndPeriod(dueTime, periodOrScheduler, scheduler);
  }
  return observableTimerTimeSpanAndPeriod(dueTime, period, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.toAsync"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>toAsync (func, context, scheduler)](#apidoc.element.rx.Observable.toAsync)
- description and source-code
```javascript
toAsync = function (func, context, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return function () {
    var args = arguments,
      subject = new AsyncSubject();

    scheduler.schedule(null, function () {
      var result;
      try {
        result = func.apply(context, args);
      } catch (e) {
        subject.onError(e);
        return;
      }
      subject.onNext(result);
      subject.onCompleted();
    });
    return subject.asObservable();
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.using"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>using (resourceFactory, observableFactory)](#apidoc.element.rx.Observable.using)
- description and source-code
```javascript
using = function (resourceFactory, observableFactory) {
  return new UsingObservable(resourceFactory, observableFactory);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.when"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>when ()](#apidoc.element.rx.Observable.when)
- description and source-code
```javascript
when = function () {
  var len = arguments.length, plans;
  if (Array.isArray(arguments[0])) {
    plans = arguments[0];
  } else {
    plans = new Array(len);
    for(var i = 0; i < len; i++) { plans[i] = arguments[i]; }
  }
  return new AnonymousObservable(function (o) {
    var activePlans = [],
        externalSubscriptions = new Map();
    var outObserver = observerCreate(
      function (x) { o.onNext(x); },
      function (err) {
        externalSubscriptions.forEach(function (v) { v.onError(err); });
        o.onError(err);
      },
      function (x) { o.onCompleted(); }
    );
    try {
      for (var i = 0, len = plans.length; i < len; i++) {
        activePlans.push(plans[i].activate(externalSubscriptions, outObserver, function (activePlan) {
          var idx = activePlans.indexOf(activePlan);
          activePlans.splice(idx, 1);
          activePlans.length === 0 && o.onCompleted();
        }));
      }
    } catch (e) {
      return observableThrow(e).subscribe(o);
    }
    var group = new CompositeDisposable();
    externalSubscriptions.forEach(function (joinObserver) {
      joinObserver.subscribe();
      group.add(joinObserver);
    });

    return group;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.while"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>while (condition, source)](#apidoc.element.rx.Observable.while)
- description and source-code
```javascript
while = function (condition, source) {
  isPromise(source) && (source = observableFromPromise(source));
  return enumerableWhile(condition, source).concat();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.whileDo"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>whileDo (condition, source)](#apidoc.element.rx.Observable.whileDo)
- description and source-code
```javascript
whileDo = function (condition, source) {
  isPromise(source) && (source = observableFromPromise(source));
  return enumerableWhile(condition, source).concat();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.wrap"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>wrap (fn)](#apidoc.element.rx.Observable.wrap)
- description and source-code
```javascript
wrap = function (fn) {
  function createObservable() {
    return Observable.spawn.call(this, fn.apply(this, arguments));
  }

  createObservable.__generatorFunction__ = fn;
  return createObservable;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.zip"></a>[function <span class="apidocSignatureSpan">rx.Observable.</span>zip ()](#apidoc.element.rx.Observable.zip)
- description and source-code
```javascript
zip = function () {
  var len = arguments.length, args = new Array(len);
  for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  if (Array.isArray(args[0])) {
    args = isFunction(args[1]) ? args[0].concat(args[1]) : args[0];
  }
  var first = args.shift();
  return first.zip.apply(first, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Observable.prototype"></a>[module rx.Observable.prototype](#apidoc.module.rx.Observable.prototype)

#### <a name="apidoc.element.rx.Observable.prototype.amb"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>amb (rightSource)](#apidoc.element.rx.Observable.prototype.amb)
- description and source-code
```javascript
amb = function (rightSource) {
  var leftSource = this;
  return new AnonymousObservable(function (observer) {
    var choice,
      leftChoice = 'L', rightChoice = 'R',
      leftSubscription = new SingleAssignmentDisposable(),
      rightSubscription = new SingleAssignmentDisposable();

    isPromise(rightSource) && (rightSource = observableFromPromise(rightSource));

    function choiceL() {
      if (!choice) {
        choice = leftChoice;
        rightSubscription.dispose();
      }
    }

    function choiceR() {
      if (!choice) {
        choice = rightChoice;
        leftSubscription.dispose();
      }
    }

    var leftSubscribe = observerCreate(
      function (left) {
        choiceL();
        choice === leftChoice && observer.onNext(left);
      },
      function (e) {
        choiceL();
        choice === leftChoice && observer.onError(e);
      },
      function () {
        choiceL();
        choice === leftChoice && observer.onCompleted();
      }
    );
    var rightSubscribe = observerCreate(
      function (right) {
        choiceR();
        choice === rightChoice && observer.onNext(right);
      },
      function (e) {
        choiceR();
        choice === rightChoice && observer.onError(e);
      },
      function () {
        choiceR();
        choice === rightChoice && observer.onCompleted();
      }
    );

    leftSubscription.setDisposable(leftSource.subscribe(leftSubscribe));
    rightSubscription.setDisposable(rightSource.subscribe(rightSubscribe));

    return new BinaryDisposable(leftSubscription, rightSubscription);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.and"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>and (right)](#apidoc.element.rx.Observable.prototype.and)
- description and source-code
```javascript
and = function (right) {
  return new Pattern([this, right]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.asObservable"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>asObservable ()](#apidoc.element.rx.Observable.prototype.asObservable)
- description and source-code
```javascript
asObservable = function () {
  return new AnonymousObservable(asObservable(this), this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.average"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>average (keySelector, thisArg)](#apidoc.element.rx.Observable.prototype.average)
- description and source-code
```javascript
average = function (keySelector, thisArg) {
  var source = this, fn;
  if (isFunction(keySelector)) {
    fn = bindCallback(keySelector, thisArg, 3);
  }
  return new AverageObservable(source, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.buffer"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>buffer ()](#apidoc.element.rx.Observable.prototype.buffer)
- description and source-code
```javascript
buffer = function () {
  return this.window.apply(this, arguments)
    .flatMap(toArray);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.bufferCount"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferCount (count, skip)](#apidoc.element.rx.Observable.prototype.bufferCount)
- description and source-code
```javascript
bufferCount = function (count, skip) {
  typeof skip !== 'number' && (skip = count);
  return this.windowWithCount(count, skip)
    .flatMap(toArray)
    .filter(notEmpty);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.bufferTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferTime (timeSpan, timeShiftOrScheduler, scheduler)](#apidoc.element.rx.Observable.prototype.bufferTime)
- description and source-code
```javascript
bufferTime = function (timeSpan, timeShiftOrScheduler, scheduler) {
  return this.windowWithTime(timeSpan, timeShiftOrScheduler, scheduler).flatMap(toArray);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.bufferTimeOrCount"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferTimeOrCount (timeSpan, count, scheduler)](#apidoc.element.rx.Observable.prototype.bufferTimeOrCount)
- description and source-code
```javascript
bufferTimeOrCount = function (timeSpan, count, scheduler) {
  return this.windowWithTimeOrCount(timeSpan, count, scheduler).flatMap(toArray);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.bufferWithCount"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferWithCount (count, skip)](#apidoc.element.rx.Observable.prototype.bufferWithCount)
- description and source-code
```javascript
bufferWithCount = function (count, skip) {
  typeof skip !== 'number' && (skip = count);
  return this.windowWithCount(count, skip)
    .flatMap(toArray)
    .filter(notEmpty);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.bufferWithTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferWithTime (timeSpan, timeShiftOrScheduler, scheduler)](#apidoc.element.rx.Observable.prototype.bufferWithTime)
- description and source-code
```javascript
bufferWithTime = function (timeSpan, timeShiftOrScheduler, scheduler) {
  return this.windowWithTime(timeSpan, timeShiftOrScheduler, scheduler).flatMap(toArray);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.bufferWithTimeOrCount"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>bufferWithTimeOrCount (timeSpan, count, scheduler)](#apidoc.element.rx.Observable.prototype.bufferWithTimeOrCount)
- description and source-code
```javascript
bufferWithTimeOrCount = function (timeSpan, count, scheduler) {
  return this.windowWithTimeOrCount(timeSpan, count, scheduler).flatMap(toArray);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.catch"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>catch (handlerOrSecond)](#apidoc.element.rx.Observable.prototype.catch)
- description and source-code
```javascript
catch = function (handlerOrSecond) {
  return isFunction(handlerOrSecond) ? new CatchObservable(this, handlerOrSecond) : observableCatch([this, handlerOrSecond]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.combineLatest"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>combineLatest ()](#apidoc.element.rx.Observable.prototype.combineLatest)
- description and source-code
```javascript
combineLatest = function () {
  var len = arguments.length, args = new Array(len);
  for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  if (Array.isArray(args[0])) {
    args[0].unshift(this);
  } else {
    args.unshift(this);
  }
  return combineLatest.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.concat"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>concat ()](#apidoc.element.rx.Observable.prototype.concat)
- description and source-code
```javascript
concat = function () {
  for(var args = [], i = 0, len = arguments.length; i < len; i++) { args.push(arguments[i]); }
  args.unshift(this);
  return observableConcat.apply(null, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.concatAll"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>concatAll ()](#apidoc.element.rx.Observable.prototype.concatAll)
- description and source-code
```javascript
concatAll = function () {
  return this.merge(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.concatMap"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>concatMap (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.concatMap)
- description and source-code
```javascript
concatMap = function (selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).merge(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.concatMapObserver"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>concatMapObserver (onNext, onError, onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.concatMapObserver)
- description and source-code
```javascript
concatMapObserver = function (onNext, onError, onCompleted, thisArg) {
  var source = this,
      onNextFunc = bindCallback(onNext, thisArg, 2),
      onErrorFunc = bindCallback(onError, thisArg, 1),
      onCompletedFunc = bindCallback(onCompleted, thisArg, 0);
  return new AnonymousObservable(function (observer) {
    var index = 0;
    return source.subscribe(
      function (x) {
        var result;
        try {
          result = onNextFunc(x, index++);
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
      },
      function (err) {
        var result;
        try {
          result = onErrorFunc(err);
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
        observer.onCompleted();
      },
      function () {
        var result;
        try {
          result = onCompletedFunc();
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
        observer.onCompleted();
      });
  }, this).concatAll();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.controlled"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>controlled (enableQueue, scheduler)](#apidoc.element.rx.Observable.prototype.controlled)
- description and source-code
```javascript
controlled = function (enableQueue, scheduler) {

  if (enableQueue && isScheduler(enableQueue)) {
    scheduler = enableQueue;
    enableQueue = true;
  }

  if (enableQueue == null) {  enableQueue = true; }
  return new ControlledObservable(this, enableQueue, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.count"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>count (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.count)
- description and source-code
```javascript
count = function (predicate, thisArg) {
  var fn = bindCallback(predicate, thisArg, 3);
  return new CountObservable(this, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.debounce"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>debounce ()](#apidoc.element.rx.Observable.prototype.debounce)
- description and source-code
```javascript
debounce = function () {
  if (isFunction (arguments[0])) {
    return debounceWithSelector(this, arguments[0]);
  } else if (typeof arguments[0] === 'number') {
    return new DebounceObservable(this, arguments[0], arguments[1]);
  } else {
    throw new Error('Invalid arguments');
  }
}
```
- example usage
```shell
...
/* Only get the value from each key up */
var keyups = Rx.Observable.fromEvent($input, 'keyup')
  .pluck('target', 'value')
  .filter(text => text.length > 2 );

/* Now debounce the input for 500ms */
var debounced = keyups
  .debounce(500 /* ms */);

/* Now get only distinct values, so we eliminate the arrows and other control characters */
var distinct = debounced
  .distinctUntilChanged();
'''

Now, let's query Wikipedia!  In RxJS, we can instantly bind to any [Promises A+](https://github.com/promises-aplus/promises-spec
) implementation through the 'Rx.Observable.fromPromise' method. Or, directly return it and RxJS will wrap it for you.
...
```

#### <a name="apidoc.element.rx.Observable.prototype.defaultIfEmpty"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>defaultIfEmpty (defaultValue)](#apidoc.element.rx.Observable.prototype.defaultIfEmpty)
- description and source-code
```javascript
defaultIfEmpty = function (defaultValue) {
  var source = this;
  defaultValue === undefined && (defaultValue = null);
  return new AnonymousObservable(function (o) {
    return source.subscribe(new DefaultIfEmptyObserver(o, defaultValue));
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.delay"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>delay ()](#apidoc.element.rx.Observable.prototype.delay)
- description and source-code
```javascript
delay = function () {
  var firstArg = arguments[0];
  if (typeof firstArg === 'number' || firstArg instanceof Date) {
    var dueTime = firstArg, scheduler = arguments[1];
    isScheduler(scheduler) || (scheduler = defaultScheduler);
    return dueTime instanceof Date ?
      observableDelayAbsolute(this, dueTime, scheduler) :
      observableDelayRelative(this, dueTime, scheduler);
  } else if (Observable.isObservable(firstArg) || isFunction(firstArg)) {
    return delayWithSelector(this, firstArg, arguments[1]);
  } else {
    throw new Error('Invalid arguments');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.delaySubscription"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>delaySubscription (dueTime, scheduler)](#apidoc.element.rx.Observable.prototype.delaySubscription)
- description and source-code
```javascript
delaySubscription = function (dueTime, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new DelaySubscription(this, dueTime, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.dematerialize"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>dematerialize ()](#apidoc.element.rx.Observable.prototype.dematerialize)
- description and source-code
```javascript
dematerialize = function () {
  return new DematerializeObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.distinct"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>distinct (keySelector, comparer)](#apidoc.element.rx.Observable.prototype.distinct)
- description and source-code
```javascript
distinct = function (keySelector, comparer) {
  comparer || (comparer = defaultComparer);
  return new DistinctObservable(this, keySelector, comparer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.distinctUntilChanged"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>distinctUntilChanged (keyFn, comparer)](#apidoc.element.rx.Observable.prototype.distinctUntilChanged)
- description and source-code
```javascript
distinctUntilChanged = function (keyFn, comparer) {
  comparer || (comparer = defaultComparer);
  return new DistinctUntilChangedObservable(this, keyFn, comparer);
}
```
- example usage
```shell
...

/* Now debounce the input for 500ms */
var debounced = keyups
.debounce(500 /* ms */);

/* Now get only distinct values, so we eliminate the arrows and other control characters */
var distinct = debounced
.distinctUntilChanged();
'''

Now, let's query Wikipedia!  In RxJS, we can instantly bind to any [Promises A+](https://github.com/promises-aplus/promises-spec
) implementation through the 'Rx.Observable.fromPromise' method. Or, directly return it and RxJS will wrap it for you.

'''js
function searchWikipedia (term) {
return $.ajax({
...
```

#### <a name="apidoc.element.rx.Observable.prototype.do"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>do (observerOrOnNext, onError, onCompleted)](#apidoc.element.rx.Observable.prototype.do)
- description and source-code
```javascript
do = function (observerOrOnNext, onError, onCompleted) {
  return new TapObservable(this, observerOrOnNext, onError, onCompleted);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.doAction"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>doAction (observerOrOnNext, onError, onCompleted)](#apidoc.element.rx.Observable.prototype.doAction)
- description and source-code
```javascript
doAction = function (observerOrOnNext, onError, onCompleted) {
  return new TapObservable(this, observerOrOnNext, onError, onCompleted);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.doOnCompleted"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>doOnCompleted (onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.doOnCompleted)
- description and source-code
```javascript
doOnCompleted = function (onCompleted, thisArg) {
  return this.tap(noop, null, typeof thisArg !== 'undefined' ? function () { onCompleted.call(thisArg); } : onCompleted);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.doOnError"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>doOnError (onError, thisArg)](#apidoc.element.rx.Observable.prototype.doOnError)
- description and source-code
```javascript
doOnError = function (onError, thisArg) {
  return this.tap(noop, typeof thisArg !== 'undefined' ? function (e) { onError.call(thisArg, e); } : onError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.doOnNext"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>doOnNext (onNext, thisArg)](#apidoc.element.rx.Observable.prototype.doOnNext)
- description and source-code
```javascript
doOnNext = function (onNext, thisArg) {
  return this.tap(typeof thisArg !== 'undefined' ? function (x) { onNext.call(thisArg, x); } : onNext);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.doWhile"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>doWhile (condition)](#apidoc.element.rx.Observable.prototype.doWhile)
- description and source-code
```javascript
doWhile = function (condition) {
  return observableConcat([this, observableWhileDo(condition, this)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.elementAt"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>elementAt (index, defaultValue)](#apidoc.element.rx.Observable.prototype.elementAt)
- description and source-code
```javascript
elementAt = function (index, defaultValue) {
  if (index < 0) { throw new ArgumentOutOfRangeError(); }
  return new ElementAtObservable(this, index, defaultValue);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.every"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>every (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.every)
- description and source-code
```javascript
every = function (predicate, thisArg) {
  var fn = bindCallback(predicate, thisArg, 3);
  return new EveryObservable(this, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.exhaustMap"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>exhaustMap (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.exhaustMap)
- description and source-code
```javascript
exhaustMap = function (selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).switchFirst();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.expand"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>expand (selector, scheduler)](#apidoc.element.rx.Observable.prototype.expand)
- description and source-code
```javascript
expand = function (selector, scheduler) {
  isScheduler(scheduler) || (scheduler = currentThreadScheduler);
  return new ExpandObservable(this, selector, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.extend"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>extend (selector, scheduler)](#apidoc.element.rx.Observable.prototype.extend)
- description and source-code
```javascript
extend = function (selector, scheduler) {
  isScheduler(scheduler) || (scheduler = Rx.Scheduler.immediate);
  var source = this;
  return observableDefer(function () {
    var chain;

    return source
      .map(function (x) {
        var curr = new ChainObservable(x);

        chain && chain.onNext(x);
        chain = curr;

        return curr;
      })
      .tap(
        noop,
        function (e) { chain && chain.onError(e); },
        function () { chain && chain.onCompleted(); }
      )
      .observeOn(scheduler)
      .map(selector);
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.filter"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>filter (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.filter)
- description and source-code
```javascript
filter = function (predicate, thisArg) {
  return this instanceof FilterObservable ? this.internalFilter(predicate, thisArg) :
    new FilterObservable(this, predicate, thisArg);
}
```
- example usage
```shell
...
But the best news of all is that you already know how to program like this.  Take for example the following JavaScript code, where
 we get some stock data and then manipulate and iterate the results.

'''js
/* Get stock data somehow */
const source = getAsyncStockData();

const subscription = source
  .filter(quote => quote.price > 30)
  .map(quote => quote.price)
  .forEach(price => console.log('Prices higher than $30: ${price}');
'''

Now what if this data were to come as some sort of event, for example a stream, such as a WebSocket? Then we could pretty much write
 the same query to iterate our data, with very little change.

'''js
...
```

#### <a name="apidoc.element.rx.Observable.prototype.finally"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>finally (action, thisArg)](#apidoc.element.rx.Observable.prototype.finally)
- description and source-code
```javascript
finally = function (action, thisArg) {
  return new FinallyObservable(this, action, thisArg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.find"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>find (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.find)
- description and source-code
```javascript
find = function (predicate, thisArg) {
  return findValue(this, predicate, thisArg, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.findIndex"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>findIndex (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.findIndex)
- description and source-code
```javascript
findIndex = function (predicate, thisArg) {
  return findValue(this, predicate, thisArg, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.first"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>first ()](#apidoc.element.rx.Observable.prototype.first)
- description and source-code
```javascript
first = function () {
  var obj = {}, source = this;
  if (typeof arguments[0] === 'object') {
    obj = arguments[0];
  } else {
    obj = {
      predicate: arguments[0],
      thisArg: arguments[1],
      defaultValue: arguments[2]
    };
  }
  if (isFunction (obj.predicate)) {
    var fn = obj.predicate;
    obj.predicate = bindCallback(fn, obj.thisArg, 3);
  }
  return new FirstObservable(this, obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.flatMap"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMap (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMap)
- description and source-code
```javascript
flatMap = function (selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).mergeAll();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.flatMapConcat"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapConcat (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapConcat)
- description and source-code
```javascript
flatMapConcat = function (selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).merge(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.flatMapFirst"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapFirst (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapFirst)
- description and source-code
```javascript
flatMapFirst = function (selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).switchFirst();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.flatMapLatest"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapLatest (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapLatest)
- description and source-code
```javascript
flatMapLatest = function (selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).switchLatest();
}
```
- example usage
```shell
...
}
'''

Once that is created, we can tie together the distinct throttled input and query the service.  In this case, we'll call 'flatMapLatest
' to get the value and ensure we're not introducing any out of order sequence calls.

'''js
var suggestions = distinct
.flatMapLatest(searchWikipedia);
'''

Finally, we call the 'subscribe' method on our observable sequence to start pulling data.

'''js
suggestions.subscribe(
data => {
...
```

#### <a name="apidoc.element.rx.Observable.prototype.flatMapMaxConcurrent"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapMaxConcurrent (limit, selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapMaxConcurrent)
- description and source-code
```javascript
flatMapMaxConcurrent = function (limit, selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).merge(limit);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.flatMapObserver"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapObserver (onNext, onError, onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapObserver)
- description and source-code
```javascript
flatMapObserver = function (onNext, onError, onCompleted, thisArg) {
  var source = this;
  return new AnonymousObservable(function (observer) {
    var index = 0;

    return source.subscribe(
      function (x) {
        var result;
        try {
          result = onNext.call(thisArg, x, index++);
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
      },
      function (err) {
        var result;
        try {
          result = onError.call(thisArg, err);
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
        observer.onCompleted();
      },
      function () {
        var result;
        try {
          result = onCompleted.call(thisArg);
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
        observer.onCompleted();
      });
  }, source).mergeAll();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.flatMapWithMaxConcurrent"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>flatMapWithMaxConcurrent (limit, selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.flatMapWithMaxConcurrent)
- description and source-code
```javascript
flatMapWithMaxConcurrent = function (limit, selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).merge(limit);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.forEach"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>forEach (oOrOnNext, onError, onCompleted)](#apidoc.element.rx.Observable.prototype.forEach)
- description and source-code
```javascript
forEach = function (oOrOnNext, onError, onCompleted) {
  return this._subscribe(typeof oOrOnNext === 'object' ?
    oOrOnNext :
    observerCreate(oOrOnNext, onError, onCompleted));
}
```
- example usage
```shell
...
'''js
/* Get stock data somehow */
const source = getAsyncStockData();

const subscription = source
  .filter(quote => quote.price > 30)
  .map(quote => quote.price)
  .forEach(price => console.log('Prices higher than $30: ${price}');
'''

Now what if this data were to come as some sort of event, for example a stream, such as a WebSocket? Then we could pretty much write
 the same query to iterate our data, with very little change.

'''js
/* Get stock data somehow */
const source = getAsyncStockData();
...
```

#### <a name="apidoc.element.rx.Observable.prototype.forkJoin"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>forkJoin ()](#apidoc.element.rx.Observable.prototype.forkJoin)
- description and source-code
```javascript
forkJoin = function () {
  var len = arguments.length, args = new Array(len);
  for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  if (Array.isArray(args[0])) {
    args[0].unshift(this);
  } else {
    args.unshift(this);
  }
  return Observable.forkJoin.apply(null, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.groupBy"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>groupBy (keySelector, elementSelector)](#apidoc.element.rx.Observable.prototype.groupBy)
- description and source-code
```javascript
groupBy = function (keySelector, elementSelector) {
  return this.groupByUntil(keySelector, elementSelector, observableNever);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.groupByUntil"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>groupByUntil (keySelector, elementSelector, durationSelector)](#apidoc.element.rx.Observable.prototype.groupByUntil)
- description and source-code
```javascript
groupByUntil = function (keySelector, elementSelector, durationSelector) {
    var source = this;
    return new AnonymousObservable(function (o) {
      var map = new Map(),
        groupDisposable = new CompositeDisposable(),
        refCountDisposable = new RefCountDisposable(groupDisposable),
        handleError = function (e) { return function (item) { item.onError(e); }; };

      groupDisposable.add(
        source.subscribe(function (x) {
          var key = tryCatch(keySelector)(x);
          if (key === errorObj) {
            map.forEach(handleError(key.e));
            return o.onError(key.e);
          }

          var fireNewMapEntry = false, writer = map.get(key);
          if (writer === undefined) {
            writer = new Subject();
            map.set(key, writer);
            fireNewMapEntry = true;
          }

          if (fireNewMapEntry) {
            var group = new GroupedObservable(key, writer, refCountDisposable),
              durationGroup = new GroupedObservable(key, writer);
            var duration = tryCatch(durationSelector)(durationGroup);
            if (duration === errorObj) {
              map.forEach(handleError(duration.e));
              return o.onError(duration.e);
            }

            o.onNext(group);

            var md = new SingleAssignmentDisposable();
            groupDisposable.add(md);

            md.setDisposable(duration.take(1).subscribe(
              noop,
              function (e) {
                map.forEach(handleError(e));
                o.onError(e);
              },
              function () {
                if (map['delete'](key)) { writer.onCompleted(); }
                groupDisposable.remove(md);
              }));
          }

          var element = x;
          if (isFunction(elementSelector)) {
            element = tryCatch(elementSelector)(x);
            if (element === errorObj) {
              map.forEach(handleError(element.e));
              return o.onError(element.e);
            }
          }

          writer.onNext(element);
      }, function (e) {
        map.forEach(handleError(e));
        o.onError(e);
      }, function () {
        map.forEach(function (item) { item.onCompleted(); });
        o.onCompleted();
      }));

    return refCountDisposable;
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.groupJoin"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>groupJoin (right, leftDurationSelector, rightDurationSelector, resultSelector)](#apidoc.element.rx.Observable.prototype.groupJoin)
- description and source-code
```javascript
groupJoin = function (right, leftDurationSelector, rightDurationSelector, resultSelector) {
  var left = this;
  return new AnonymousObservable(function (o) {
    var group = new CompositeDisposable();
    var r = new RefCountDisposable(group);
    var leftMap = new Map(), rightMap = new Map();
    var leftId = 0, rightId = 0;
    var handleError = function (e) { return function (v) { v.onError(e); }; };

    function handleError(e) { };

    group.add(left.subscribe(
      function (value) {
        var s = new Subject();
        var id = leftId++;
        leftMap.set(id, s);

        var result = tryCatch(resultSelector)(value, addRef(s, r));
        if (result === errorObj) {
          leftMap.forEach(handleError(result.e));
          return o.onError(result.e);
        }
        o.onNext(result);

        rightMap.forEach(function (v) { s.onNext(v); });

        var md = new SingleAssignmentDisposable();
        group.add(md);

        var duration = tryCatch(leftDurationSelector)(value);
        if (duration === errorObj) {
          leftMap.forEach(handleError(duration.e));
          return o.onError(duration.e);
        }

        md.setDisposable(duration.take(1).subscribe(
          noop,
          function (e) {
            leftMap.forEach(handleError(e));
            o.onError(e);
          },
          function () {
            leftMap['delete'](id) && s.onCompleted();
            group.remove(md);
          }));
      },
      function (e) {
        leftMap.forEach(handleError(e));
        o.onError(e);
      },
      function () { o.onCompleted(); })
    );

    group.add(right.subscribe(
      function (value) {
        var id = rightId++;
        rightMap.set(id, value);

        var md = new SingleAssignmentDisposable();
        group.add(md);

        var duration = tryCatch(rightDurationSelector)(value);
        if (duration === errorObj) {
          leftMap.forEach(handleError(duration.e));
          return o.onError(duration.e);
        }

        md.setDisposable(duration.take(1).subscribe(
          noop,
          function (e) {
            leftMap.forEach(handleError(e));
            o.onError(e);
          },
          function () {
            rightMap['delete'](id);
            group.remove(md);
          }));

        leftMap.forEach(function (v) { v.onNext(value); });
      },
      function (e) {
        leftMap.forEach(handleError(e));
        o.onError(e);
      })
    );

    return r;
  }, left);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.ignoreElements"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>ignoreElements ()](#apidoc.element.rx.Observable.prototype.ignoreElements)
- description and source-code
```javascript
ignoreElements = function () {
  return new IgnoreElementsObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.includes"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>includes (searchElement, fromIndex)](#apidoc.element.rx.Observable.prototype.includes)
- description and source-code
```javascript
includes = function (searchElement, fromIndex) {
  return new IncludesObservable(this, searchElement, fromIndex);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>indexOf (searchElement, fromIndex)](#apidoc.element.rx.Observable.prototype.indexOf)
- description and source-code
```javascript
indexOf = function (searchElement, fromIndex) {
  var n = +fromIndex || 0;
  Math.abs(n) === Infinity && (n = 0);
  return new IndexOfObservable(this, searchElement, n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>isEmpty ()](#apidoc.element.rx.Observable.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  return new IsEmptyObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.join"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>join (right, leftDurationSelector, rightDurationSelector, resultSelector)](#apidoc.element.rx.Observable.prototype.join)
- description and source-code
```javascript
join = function (right, leftDurationSelector, rightDurationSelector, resultSelector) {
  var left = this;
  return new AnonymousObservable(function (o) {
    var group = new CompositeDisposable();
    var leftDone = false, rightDone = false;
    var leftId = 0, rightId = 0;
    var leftMap = new Map(), rightMap = new Map();
    var handleError = function (e) { o.onError(e); };

    group.add(left.subscribe(
      function (value) {
        var id = leftId++, md = new SingleAssignmentDisposable();

        leftMap.set(id, value);
        group.add(md);

        var duration = tryCatch(leftDurationSelector)(value);
        if (duration === errorObj) { return o.onError(duration.e); }

        md.setDisposable(duration.take(1).subscribe(
          noop,
          handleError,
          function () {
            leftMap['delete'](id) && leftMap.size === 0 && leftDone && o.onCompleted();
            group.remove(md);
          }));

        rightMap.forEach(function (v) {
          var result = tryCatch(resultSelector)(value, v);
          if (result === errorObj) { return o.onError(result.e); }
          o.onNext(result);
        });
      },
      handleError,
      function () {
        leftDone = true;
        (rightDone || leftMap.size === 0) && o.onCompleted();
      })
    );

    group.add(right.subscribe(
      function (value) {
        var id = rightId++, md = new SingleAssignmentDisposable();

        rightMap.set(id, value);
        group.add(md);

        var duration = tryCatch(rightDurationSelector)(value);
        if (duration === errorObj) { return o.onError(duration.e); }

        md.setDisposable(duration.take(1).subscribe(
          noop,
          handleError,
          function () {
            rightMap['delete'](id) && rightMap.size === 0 && rightDone && o.onCompleted();
            group.remove(md);
          }));

        leftMap.forEach(function (v) {
          var result = tryCatch(resultSelector)(v, value);
          if (result === errorObj) { return o.onError(result.e); }
          o.onNext(result);
        });
      },
      handleError,
      function () {
        rightDone = true;
        (leftDone || rightMap.size === 0) && o.onCompleted();
      })
    );
    return group;
  }, left);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.jortSort"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>jortSort ()](#apidoc.element.rx.Observable.prototype.jortSort)
- description and source-code
```javascript
jortSort = function () {
  return this.jortSortUntil(observableNever());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.jortSortUntil"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>jortSortUntil (other)](#apidoc.element.rx.Observable.prototype.jortSortUntil)
- description and source-code
```javascript
jortSortUntil = function (other) {
  var source = this;
  return new AnonymousObservable(function (observer) {
    var arr = [];
    return source.takeUntil(other).subscribe(
      arr.push.bind(arr),
      observer.onError.bind(observer),
      function () {
        var sorted = arr.slice(0).sort(defaultSubComparer);
        observer.onNext(isEqual(arr, sorted));
        observer.onCompleted();
      });
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.last"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>last ()](#apidoc.element.rx.Observable.prototype.last)
- description and source-code
```javascript
last = function () {
  var obj = {}, source = this;
  if (typeof arguments[0] === 'object') {
    obj = arguments[0];
  } else {
    obj = {
      predicate: arguments[0],
      thisArg: arguments[1],
      defaultValue: arguments[2]
    };
  }
  if (isFunction (obj.predicate)) {
    var fn = obj.predicate;
    obj.predicate = bindCallback(fn, obj.thisArg, 3);
  }
  return new LastObservable(this, obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>lastIndexOf (searchElement, fromIndex)](#apidoc.element.rx.Observable.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function (searchElement, fromIndex) {
  var n = +fromIndex || 0;
  Math.abs(n) === Infinity && (n = 0);
  return new LastIndexOfObservable(this, searchElement, n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.let"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>let (func)](#apidoc.element.rx.Observable.prototype.let)
- description and source-code
```javascript
let = function (func) {
  return func(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.letBind"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>letBind (func)](#apidoc.element.rx.Observable.prototype.letBind)
- description and source-code
```javascript
letBind = function (func) {
  return func(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.manySelect"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>manySelect (selector, scheduler)](#apidoc.element.rx.Observable.prototype.manySelect)
- description and source-code
```javascript
manySelect = function (selector, scheduler) {
  isScheduler(scheduler) || (scheduler = Rx.Scheduler.immediate);
  var source = this;
  return observableDefer(function () {
    var chain;

    return source
      .map(function (x) {
        var curr = new ChainObservable(x);

        chain && chain.onNext(x);
        chain = curr;

        return curr;
      })
      .tap(
        noop,
        function (e) { chain && chain.onError(e); },
        function () { chain && chain.onCompleted(); }
      )
      .observeOn(scheduler)
      .map(selector);
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.map"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>map (selector, thisArg)](#apidoc.element.rx.Observable.prototype.map)
- description and source-code
```javascript
map = function (selector, thisArg) {
  var selectorFn = typeof selector === 'function' ? selector : function () { return selector; };
  return this instanceof MapObservable ?
    this.internalMap(selectorFn, thisArg) :
    new MapObservable(this, selectorFn, thisArg);
}
```
- example usage
```shell
...

'''js
/* Get stock data somehow */
const source = getAsyncStockData();

const subscription = source
  .filter(quote => quote.price > 30)
  .map(quote => quote.price)
  .forEach(price => console.log('Prices higher than $30: ${price}');
'''

Now what if this data were to come as some sort of event, for example a stream, such as a WebSocket? Then we could pretty much write
 the same query to iterate our data, with very little change.

'''js
/* Get stock data somehow */
...
```

#### <a name="apidoc.element.rx.Observable.prototype.materialize"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>materialize ()](#apidoc.element.rx.Observable.prototype.materialize)
- description and source-code
```javascript
materialize = function () {
  return new MaterializeObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.max"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>max (comparer)](#apidoc.element.rx.Observable.prototype.max)
- description and source-code
```javascript
max = function (comparer) {
  return this.maxBy(identity, comparer).map(firstOnly);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.maxBy"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>maxBy (keySelector, comparer)](#apidoc.element.rx.Observable.prototype.maxBy)
- description and source-code
```javascript
maxBy = function (keySelector, comparer) {
  comparer || (comparer = defaultSubComparer);
  return new ExtremaByObservable(this, keySelector, comparer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.merge"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>merge (maxConcurrentOrOther)](#apidoc.element.rx.Observable.prototype.merge)
- description and source-code
```javascript
merge = function (maxConcurrentOrOther) {
  return typeof maxConcurrentOrOther !== 'number' ?
    observableMerge(this, maxConcurrentOrOther) :
    new MergeObservable(this, maxConcurrentOrOther);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.mergeAll"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>mergeAll ()](#apidoc.element.rx.Observable.prototype.mergeAll)
- description and source-code
```javascript
mergeAll = function () {
  return new MergeAllObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.mergeMap"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>mergeMap (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.mergeMap)
- description and source-code
```javascript
mergeMap = function (selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).mergeAll();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.min"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>min (comparer)](#apidoc.element.rx.Observable.prototype.min)
- description and source-code
```javascript
min = function (comparer) {
  return this.minBy(identity, comparer).map(firstOnly);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.minBy"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>minBy (keySelector, comparer)](#apidoc.element.rx.Observable.prototype.minBy)
- description and source-code
```javascript
minBy = function (keySelector, comparer) {
  comparer || (comparer = defaultSubComparer);
  return new ExtremaByObservable(this, keySelector, function (x, y) { return comparer(x, y) * -1; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.multicast"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>multicast (subjectOrSubjectSelector, selector)](#apidoc.element.rx.Observable.prototype.multicast)
- description and source-code
```javascript
multicast = function (subjectOrSubjectSelector, selector) {
  return isFunction(subjectOrSubjectSelector) ?
    new MulticastObservable(this, subjectOrSubjectSelector, selector) :
    new ConnectableObservable(this, subjectOrSubjectSelector);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.observeOn"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>observeOn (scheduler)](#apidoc.element.rx.Observable.prototype.observeOn)
- description and source-code
```javascript
observeOn = function (scheduler) {
  return new ObserveOnObservable(this, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.onErrorResumeNext"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>onErrorResumeNext (second)](#apidoc.element.rx.Observable.prototype.onErrorResumeNext)
- description and source-code
```javascript
onErrorResumeNext = function (second) {
  if (!second) { throw new Error('Second observable is required'); }
  return onErrorResumeNext([this, second]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.pairwise"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>pairwise ()](#apidoc.element.rx.Observable.prototype.pairwise)
- description and source-code
```javascript
pairwise = function () {
  return new PairwiseObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.partition"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>partition (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.partition)
- description and source-code
```javascript
partition = function (predicate, thisArg) {
  var fn = bindCallback(predicate, thisArg, 3);
  return [
    this.filter(predicate, thisArg),
    this.filter(function (x, i, o) { return !fn(x, i, o); })
  ];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.pausable"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>pausable (pauser)](#apidoc.element.rx.Observable.prototype.pausable)
- description and source-code
```javascript
pausable = function (pauser) {
  return new PausableObservable(this, pauser);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.pausableBuffered"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>pausableBuffered (pauser)](#apidoc.element.rx.Observable.prototype.pausableBuffered)
- description and source-code
```javascript
pausableBuffered = function (pauser) {
  return new PausableBufferedObservable(this, pauser);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.pipe"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>pipe (dest)](#apidoc.element.rx.Observable.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest) {
  var source = this.pausableBuffered();

  function onDrain() {
    source.resume();
  }

  dest.addListener('drain', onDrain);

  source.subscribe(
    function (x) {
      !dest.write(x) && source.pause();
    },
    function (err) {
      dest.emit('error', err);
    },
    function () {
      // Hack check because STDIO is not closable
      !dest._isStdio && dest.end();
      dest.removeListener('drain', onDrain);
    });

  source.resume();

  return dest;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.pluck"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>pluck ()](#apidoc.element.rx.Observable.prototype.pluck)
- description and source-code
```javascript
pluck = function () {
  var len = arguments.length, args = new Array(len);
  if (len === 0) { throw new Error('List of properties cannot be empty.'); }
  for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  return this.map(plucker(args, len));
}
```
- example usage
```shell
...

'''js
const $input = $('#input');
const $results = $('#results');

/* Only get the value from each key up */
var keyups = Rx.Observable.fromEvent($input, 'keyup')
  .pluck('target', 'value')
  .filter(text => text.length > 2 );

/* Now debounce the input for 500ms */
var debounced = keyups
  .debounce(500 /* ms */);

/* Now get only distinct values, so we eliminate the arrows and other control characters */
...
```

#### <a name="apidoc.element.rx.Observable.prototype.publish"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>publish (selector)](#apidoc.element.rx.Observable.prototype.publish)
- description and source-code
```javascript
publish = function (selector) {
  return selector && isFunction(selector) ?
    this.multicast(function () { return new Subject(); }, selector) :
    this.multicast(new Subject());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.publishLast"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>publishLast (selector)](#apidoc.element.rx.Observable.prototype.publishLast)
- description and source-code
```javascript
publishLast = function (selector) {
  return selector && isFunction(selector) ?
    this.multicast(function () { return new AsyncSubject(); }, selector) :
    this.multicast(new AsyncSubject());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.publishValue"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>publishValue (initialValueOrSelector, initialValue)](#apidoc.element.rx.Observable.prototype.publishValue)
- description and source-code
```javascript
publishValue = function (initialValueOrSelector, initialValue) {
  return arguments.length === 2 ?
    this.multicast(function () {
      return new BehaviorSubject(initialValue);
    }, initialValueOrSelector) :
    this.multicast(new BehaviorSubject(initialValueOrSelector));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.reduce"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>reduce ()](#apidoc.element.rx.Observable.prototype.reduce)
- description and source-code
```javascript
reduce = function () {
  var hasSeed = false, seed, accumulator = arguments[0];
  if (arguments.length === 2) {
    hasSeed = true;
    seed = arguments[1];
  }
  return new ReduceObservable(this, accumulator, hasSeed, seed);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.repeat"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>repeat (repeatCount)](#apidoc.element.rx.Observable.prototype.repeat)
- description and source-code
```javascript
repeat = function (repeatCount) {
  return enumerableRepeat(this, repeatCount).concat();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.repeatWhen"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>repeatWhen (notifier)](#apidoc.element.rx.Observable.prototype.repeatWhen)
- description and source-code
```javascript
repeatWhen = function (notifier) {
  return new RepeatWhenObservable(repeat(this), notifier);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.replay"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>replay (selector, bufferSize, windowSize, scheduler)](#apidoc.element.rx.Observable.prototype.replay)
- description and source-code
```javascript
replay = function (selector, bufferSize, windowSize, scheduler) {
  return selector && isFunction(selector) ?
    this.multicast(function () { return new ReplaySubject(bufferSize, windowSize, scheduler); }, selector) :
    this.multicast(new ReplaySubject(bufferSize, windowSize, scheduler));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.retry"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>retry (retryCount)](#apidoc.element.rx.Observable.prototype.retry)
- description and source-code
```javascript
retry = function (retryCount) {
  return enumerableRepeat(this, retryCount).catchError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.retryWhen"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>retryWhen (notifier)](#apidoc.element.rx.Observable.prototype.retryWhen)
- description and source-code
```javascript
retryWhen = function (notifier) {
  return new RetryWhenObservable(repeat(this), notifier);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.sample"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>sample (intervalOrSampler, scheduler)](#apidoc.element.rx.Observable.prototype.sample)
- description and source-code
```javascript
sample = function (intervalOrSampler, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return typeof intervalOrSampler === 'number' ?
    new SampleObservable(this, observableinterval(intervalOrSampler, scheduler)) :
    new SampleObservable(this, intervalOrSampler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.scan"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>scan ()](#apidoc.element.rx.Observable.prototype.scan)
- description and source-code
```javascript
scan = function () {
  var hasSeed = false, seed, accumulator = arguments[0];
  if (arguments.length === 2) {
    hasSeed = true;
    seed = arguments[1];
  }
  return new ScanObservable(this, accumulator, hasSeed, seed);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.select"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>select (selector, thisArg)](#apidoc.element.rx.Observable.prototype.select)
- description and source-code
```javascript
select = function (selector, thisArg) {
  var selectorFn = typeof selector === 'function' ? selector : function () { return selector; };
  return this instanceof MapObservable ?
    this.internalMap(selectorFn, thisArg) :
    new MapObservable(this, selectorFn, thisArg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.selectConcatObserver"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>selectConcatObserver (onNext, onError, onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.selectConcatObserver)
- description and source-code
```javascript
selectConcatObserver = function (onNext, onError, onCompleted, thisArg) {
  var source = this,
      onNextFunc = bindCallback(onNext, thisArg, 2),
      onErrorFunc = bindCallback(onError, thisArg, 1),
      onCompletedFunc = bindCallback(onCompleted, thisArg, 0);
  return new AnonymousObservable(function (observer) {
    var index = 0;
    return source.subscribe(
      function (x) {
        var result;
        try {
          result = onNextFunc(x, index++);
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
      },
      function (err) {
        var result;
        try {
          result = onErrorFunc(err);
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
        observer.onCompleted();
      },
      function () {
        var result;
        try {
          result = onCompletedFunc();
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
        observer.onCompleted();
      });
  }, this).concatAll();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.selectMany"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>selectMany (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.selectMany)
- description and source-code
```javascript
selectMany = function (selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).mergeAll();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.selectManyObserver"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>selectManyObserver (onNext, onError, onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.selectManyObserver)
- description and source-code
```javascript
selectManyObserver = function (onNext, onError, onCompleted, thisArg) {
  var source = this;
  return new AnonymousObservable(function (observer) {
    var index = 0;

    return source.subscribe(
      function (x) {
        var result;
        try {
          result = onNext.call(thisArg, x, index++);
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
      },
      function (err) {
        var result;
        try {
          result = onError.call(thisArg, err);
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
        observer.onCompleted();
      },
      function () {
        var result;
        try {
          result = onCompleted.call(thisArg);
        } catch (e) {
          observer.onError(e);
          return;
        }
        isPromise(result) && (result = observableFromPromise(result));
        observer.onNext(result);
        observer.onCompleted();
      });
  }, source).mergeAll();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.sequenceEqual"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>sequenceEqual (second, comparer)](#apidoc.element.rx.Observable.prototype.sequenceEqual)
- description and source-code
```javascript
sequenceEqual = function (second, comparer) {
  var first = this;
  comparer || (comparer = defaultComparer);
  return new AnonymousObservable(function (o) {
    var donel = false, doner = false, ql = [], qr = [];
    var subscription1 = first.subscribe(function (x) {
      if (qr.length > 0) {
        var v = qr.shift();
        var equal = tryCatch(comparer)(v, x);
        if (equal === errorObj) { return o.onError(equal.e); }
        if (!equal) {
          o.onNext(false);
          o.onCompleted();
        }
      } else if (doner) {
        o.onNext(false);
        o.onCompleted();
      } else {
        ql.push(x);
      }
    }, function(e) { o.onError(e); }, function () {
      donel = true;
      if (ql.length === 0) {
        if (qr.length > 0) {
          o.onNext(false);
          o.onCompleted();
        } else if (doner) {
          o.onNext(true);
          o.onCompleted();
        }
      }
    });

    (isArrayLike(second) || isIterable(second)) && (second = observableFrom(second));
    isPromise(second) && (second = observableFromPromise(second));
    var subscription2 = second.subscribe(function (x) {
      if (ql.length > 0) {
        var v = ql.shift();
        var equal = tryCatch(comparer)(v, x);
        if (equal === errorObj) { return o.onError(equal.e); }
        if (!equal) {
          o.onNext(false);
          o.onCompleted();
        }
      } else if (donel) {
        o.onNext(false);
        o.onCompleted();
      } else {
        qr.push(x);
      }
    }, function(e) { o.onError(e); }, function () {
      doner = true;
      if (qr.length === 0) {
        if (ql.length > 0) {
          o.onNext(false);
          o.onCompleted();
        } else if (donel) {
          o.onNext(true);
          o.onCompleted();
        }
      }
    });
    return new BinaryDisposable(subscription1, subscription2);
  }, first);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.share"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>share ()](#apidoc.element.rx.Observable.prototype.share)
- description and source-code
```javascript
share = function () {
  return this.publish().refCount();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.shareReplay"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>shareReplay (bufferSize, windowSize, scheduler)](#apidoc.element.rx.Observable.prototype.shareReplay)
- description and source-code
```javascript
shareReplay = function (bufferSize, windowSize, scheduler) {
  return this.replay(null, bufferSize, windowSize, scheduler).refCount();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.shareValue"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>shareValue (initialValue)](#apidoc.element.rx.Observable.prototype.shareValue)
- description and source-code
```javascript
shareValue = function (initialValue) {
  return this.publishValue(initialValue).refCount();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.single"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>single (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.single)
- description and source-code
```javascript
single = function (predicate, thisArg) {
  var obj = {}, source = this;
  if (typeof arguments[0] === 'object') {
    obj = arguments[0];
  } else {
    obj = {
      predicate: arguments[0],
      thisArg: arguments[1],
      defaultValue: arguments[2]
    };
  }
  if (isFunction (obj.predicate)) {
    var fn = obj.predicate;
    obj.predicate = bindCallback(fn, obj.thisArg, 3);
  }
  return new AnonymousObservable(function (o) {
    return source.subscribe(new SingleObserver(o, obj, source));
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.singleInstance"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>singleInstance ()](#apidoc.element.rx.Observable.prototype.singleInstance)
- description and source-code
```javascript
singleInstance = function () {
  var source = this, hasObservable = false, observable;

  function getObservable() {
    if (!hasObservable) {
      hasObservable = true;
      observable = source['finally'](function() { hasObservable = false; }).publish().refCount();
    }
    return observable;
  }

  return new AnonymousObservable(function(o) {
    return getObservable().subscribe(o);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.skip"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skip (count)](#apidoc.element.rx.Observable.prototype.skip)
- description and source-code
```javascript
skip = function (count) {
  if (count < 0) { throw new ArgumentOutOfRangeError(); }
  return new SkipObservable(this, count);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.skipLast"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipLast (count)](#apidoc.element.rx.Observable.prototype.skipLast)
- description and source-code
```javascript
skipLast = function (count) {
  if (count < 0) { throw new ArgumentOutOfRangeError(); }
  return new SkipLastObservable(this, count);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.skipLastWithTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipLastWithTime (duration, scheduler)](#apidoc.element.rx.Observable.prototype.skipLastWithTime)
- description and source-code
```javascript
skipLastWithTime = function (duration, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new SkipLastWithTimeObservable(this, duration, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.skipUntil"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipUntil (other)](#apidoc.element.rx.Observable.prototype.skipUntil)
- description and source-code
```javascript
skipUntil = function (other) {
  return new SkipUntilObservable(this, other);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.skipUntilWithTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipUntilWithTime (startTime, scheduler)](#apidoc.element.rx.Observable.prototype.skipUntilWithTime)
- description and source-code
```javascript
skipUntilWithTime = function (startTime, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new SkipUntilWithTimeObservable(this, startTime, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.skipWhile"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipWhile (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.skipWhile)
- description and source-code
```javascript
skipWhile = function (predicate, thisArg) {
  var fn = bindCallback(predicate, thisArg, 3);
  return new SkipWhileObservable(this, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.skipWithTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>skipWithTime (duration, scheduler)](#apidoc.element.rx.Observable.prototype.skipWithTime)
- description and source-code
```javascript
skipWithTime = function (duration, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new SkipWithTimeObservable(this, duration, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.slice"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>slice (begin, end)](#apidoc.element.rx.Observable.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  var start = begin || 0;
  if (start < 0) { throw new Rx.ArgumentOutOfRangeError(); }
  if (typeof end === 'number' && end < start) {
    throw new Rx.ArgumentOutOfRangeError();
  }
  return new SliceObservable(this, start, end);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.some"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>some (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.some)
- description and source-code
```javascript
some = function (predicate, thisArg) {
  var fn = bindCallback(predicate, thisArg, 3);
  return new SomeObservable(this, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.startWith"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>startWith ()](#apidoc.element.rx.Observable.prototype.startWith)
- description and source-code
```javascript
startWith = function () {
  var values, scheduler, start = 0;
  if (!!arguments.length && isScheduler(arguments[0])) {
    scheduler = arguments[0];
    start = 1;
  } else {
    scheduler = immediateScheduler;
  }
  for(var args = [], i = start, len = arguments.length; i < len; i++) { args.push(arguments[i]); }
  return observableConcat.apply(null, [observableFromArray(args, scheduler), this]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.subscribe"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>subscribe (oOrOnNext, onError, onCompleted)](#apidoc.element.rx.Observable.prototype.subscribe)
- description and source-code
```javascript
subscribe = function (oOrOnNext, onError, onCompleted) {
  return this._subscribe(typeof oOrOnNext === 'object' ?
    oOrOnNext :
    observerCreate(oOrOnNext, onError, onCompleted));
}
```
- example usage
```shell
...
'''js
/* Get stock data somehow */
const source = getAsyncStockData();

const subscription = source
  .filter(quote => quote.price > 30)
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''
...
```

#### <a name="apidoc.element.rx.Observable.prototype.subscribeOn"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>subscribeOn (scheduler)](#apidoc.element.rx.Observable.prototype.subscribeOn)
- description and source-code
```javascript
subscribeOn = function (scheduler) {
  return new SubscribeOnObservable(this, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.subscribeOnCompleted"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>subscribeOnCompleted (onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.subscribeOnCompleted)
- description and source-code
```javascript
subscribeOnCompleted = function (onCompleted, thisArg) {
  return this._subscribe(observerCreate(null, null, typeof thisArg !== 'undefined' ? function() { onCompleted.call(thisArg); } :
onCompleted));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.subscribeOnError"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>subscribeOnError (onError, thisArg)](#apidoc.element.rx.Observable.prototype.subscribeOnError)
- description and source-code
```javascript
subscribeOnError = function (onError, thisArg) {
  return this._subscribe(observerCreate(null, typeof thisArg !== 'undefined' ? function(e) { onError.call(thisArg, e); } : onError
));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.subscribeOnNext"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>subscribeOnNext (onNext, thisArg)](#apidoc.element.rx.Observable.prototype.subscribeOnNext)
- description and source-code
```javascript
subscribeOnNext = function (onNext, thisArg) {
  return this._subscribe(observerCreate(typeof thisArg !== 'undefined' ? function(x) { onNext.call(thisArg, x); } : onNext));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.sum"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>sum (keySelector, thisArg)](#apidoc.element.rx.Observable.prototype.sum)
- description and source-code
```javascript
sum = function (keySelector, thisArg) {
  var fn = bindCallback(keySelector, thisArg, 3);
  return new SumObservable(this, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.switch"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>switch ()](#apidoc.element.rx.Observable.prototype.switch)
- description and source-code
```javascript
switch = function () {
  return new SwitchObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.switchFirst"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>switchFirst ()](#apidoc.element.rx.Observable.prototype.switchFirst)
- description and source-code
```javascript
switchFirst = function () {
  return new SwitchFirstObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.switchLatest"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>switchLatest ()](#apidoc.element.rx.Observable.prototype.switchLatest)
- description and source-code
```javascript
switchLatest = function () {
  return new SwitchObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.switchMap"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>switchMap (selector, resultSelector, thisArg)](#apidoc.element.rx.Observable.prototype.switchMap)
- description and source-code
```javascript
switchMap = function (selector, resultSelector, thisArg) {
    return new FlatMapObservable(this, selector, resultSelector, thisArg).switchLatest();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.take"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>take (count, scheduler)](#apidoc.element.rx.Observable.prototype.take)
- description and source-code
```javascript
take = function (count, scheduler) {
  if (count < 0) { throw new ArgumentOutOfRangeError(); }
  if (count === 0) { return observableEmpty(scheduler); }
  return new TakeObservable(this, count);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.takeLast"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeLast (count)](#apidoc.element.rx.Observable.prototype.takeLast)
- description and source-code
```javascript
takeLast = function (count) {
  if (count < 0) { throw new ArgumentOutOfRangeError(); }
  var source = this;
  return new AnonymousObservable(function (o) {
    return source.subscribe(new TakeLastObserver(o, count));
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.takeLastBuffer"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeLastBuffer (count)](#apidoc.element.rx.Observable.prototype.takeLastBuffer)
- description and source-code
```javascript
takeLastBuffer = function (count) {
  if (count < 0) { throw new ArgumentOutOfRangeError(); }
  var source = this;
  return new AnonymousObservable(function (o) {
    return source.subscribe(new TakeLastBufferObserver(o, count));
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.takeLastBufferWithTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeLastBufferWithTime (duration, scheduler)](#apidoc.element.rx.Observable.prototype.takeLastBufferWithTime)
- description and source-code
```javascript
takeLastBufferWithTime = function (duration, scheduler) {
  var source = this;
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new AnonymousObservable(function (o) {
    var q = [];
    return source.subscribe(function (x) {
      var now = scheduler.now();
      q.push({ interval: now, value: x });
      while (q.length > 0 && now - q[0].interval >= duration) {
        q.shift();
      }
    }, function (e) { o.onError(e); }, function () {
      var now = scheduler.now(), res = [];
      while (q.length > 0) {
        var next = q.shift();
        now - next.interval <= duration && res.push(next.value);
      }
      o.onNext(res);
      o.onCompleted();
    });
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.takeLastWithTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeLastWithTime (duration, scheduler)](#apidoc.element.rx.Observable.prototype.takeLastWithTime)
- description and source-code
```javascript
takeLastWithTime = function (duration, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new TakeLastWithTimeObservable(this, duration, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.takeUntil"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeUntil (other)](#apidoc.element.rx.Observable.prototype.takeUntil)
- description and source-code
```javascript
takeUntil = function (other) {
  return new TakeUntilObservable(this, other);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.takeUntilWithTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeUntilWithTime (endTime, scheduler)](#apidoc.element.rx.Observable.prototype.takeUntilWithTime)
- description and source-code
```javascript
takeUntilWithTime = function (endTime, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  var source = this;
  return new AnonymousObservable(function (o) {
    return new BinaryDisposable(
      scheduler.scheduleFuture(o, endTime, function (_, o) { o.onCompleted(); }),
      source.subscribe(o));
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.takeWhile"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeWhile (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.takeWhile)
- description and source-code
```javascript
takeWhile = function (predicate, thisArg) {
  var fn = bindCallback(predicate, thisArg, 3);
  return new TakeWhileObservable(this, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.takeWithTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>takeWithTime (duration, scheduler)](#apidoc.element.rx.Observable.prototype.takeWithTime)
- description and source-code
```javascript
takeWithTime = function (duration, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new TakeWithTimeObservable(this, duration, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.tap"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>tap (observerOrOnNext, onError, onCompleted)](#apidoc.element.rx.Observable.prototype.tap)
- description and source-code
```javascript
tap = function (observerOrOnNext, onError, onCompleted) {
  return new TapObservable(this, observerOrOnNext, onError, onCompleted);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.tapOnCompleted"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>tapOnCompleted (onCompleted, thisArg)](#apidoc.element.rx.Observable.prototype.tapOnCompleted)
- description and source-code
```javascript
tapOnCompleted = function (onCompleted, thisArg) {
  return this.tap(noop, null, typeof thisArg !== 'undefined' ? function () { onCompleted.call(thisArg); } : onCompleted);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.tapOnError"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>tapOnError (onError, thisArg)](#apidoc.element.rx.Observable.prototype.tapOnError)
- description and source-code
```javascript
tapOnError = function (onError, thisArg) {
  return this.tap(noop, typeof thisArg !== 'undefined' ? function (e) { onError.call(thisArg, e); } : onError);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.tapOnNext"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>tapOnNext (onNext, thisArg)](#apidoc.element.rx.Observable.prototype.tapOnNext)
- description and source-code
```javascript
tapOnNext = function (onNext, thisArg) {
  return this.tap(typeof thisArg !== 'undefined' ? function (x) { onNext.call(thisArg, x); } : onNext);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.thenDo"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>thenDo (selector)](#apidoc.element.rx.Observable.prototype.thenDo)
- description and source-code
```javascript
thenDo = function (selector) {
  return new Pattern([this]).thenDo(selector);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.throttle"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>throttle (windowDuration, scheduler)](#apidoc.element.rx.Observable.prototype.throttle)
- description and source-code
```javascript
throttle = function (windowDuration, scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  var duration = +windowDuration || 0;
  if (duration <= 0) { throw new RangeError('windowDuration cannot be less or equal zero.'); }
  var source = this;
  return new AnonymousObservable(function (o) {
    var lastOnNext = 0;
    return source.subscribe(
      function (x) {
        var now = scheduler.now();
        if (lastOnNext === 0 || now - lastOnNext >= duration) {
          lastOnNext = now;
          o.onNext(x);
        }
      },function (e) { o.onError(e); }, function () { o.onCompleted(); }
    );
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.timeInterval"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>timeInterval (scheduler)](#apidoc.element.rx.Observable.prototype.timeInterval)
- description and source-code
```javascript
timeInterval = function (scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new TimeIntervalObservable(this, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.timeout"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>timeout ()](#apidoc.element.rx.Observable.prototype.timeout)
- description and source-code
```javascript
timeout = function () {
  var firstArg = arguments[0];
  if (firstArg instanceof Date || typeof firstArg === 'number') {
    return timeout(this, firstArg, arguments[1], arguments[2]);
  } else if (Observable.isObservable(firstArg) || isFunction(firstArg)) {
    return timeoutWithSelector(this, firstArg, arguments[1], arguments[2]);
  } else {
    throw new Error('Invalid arguments');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.timestamp"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>timestamp (scheduler)](#apidoc.element.rx.Observable.prototype.timestamp)
- description and source-code
```javascript
timestamp = function (scheduler) {
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new TimestampObservable(this, scheduler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.toArray"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>toArray ()](#apidoc.element.rx.Observable.prototype.toArray)
- description and source-code
```javascript
toArray = function () {
  return new ToArrayObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.toMap"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>toMap (keySelector, elementSelector)](#apidoc.element.rx.Observable.prototype.toMap)
- description and source-code
```javascript
toMap = function (keySelector, elementSelector) {
  if (typeof root.Map === 'undefined') { throw new TypeError(); }
  return new ToMapObservable(this, keySelector, elementSelector);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.toPromise"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>toPromise (promiseCtor)](#apidoc.element.rx.Observable.prototype.toPromise)
- description and source-code
```javascript
toPromise = function (promiseCtor) {
  promiseCtor || (promiseCtor = Rx.config.Promise);
  if (!promiseCtor) { throw new NotSupportedError('Promise type not provided nor in Rx.config.Promise'); }
  var source = this;
  return new promiseCtor(function (resolve, reject) {
    // No cancellation can be done
    var value;
    source.subscribe(function (v) {
      value = v;
    }, reject, function () {
      resolve(value);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.toSet"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>toSet ()](#apidoc.element.rx.Observable.prototype.toSet)
- description and source-code
```javascript
toSet = function () {
  if (typeof root.Set === 'undefined') { throw new TypeError(); }
  return new ToSetObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.transduce"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>transduce (transducer)](#apidoc.element.rx.Observable.prototype.transduce)
- description and source-code
```javascript
transduce = function (transducer) {
  var source = this;
  return new AnonymousObservable(function(o) {
    var xform = transducer(transformForObserver(o));
    return source.subscribe(new TransduceObserver(o, xform));
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.where"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>where (predicate, thisArg)](#apidoc.element.rx.Observable.prototype.where)
- description and source-code
```javascript
where = function (predicate, thisArg) {
  return this instanceof FilterObservable ? this.internalFilter(predicate, thisArg) :
    new FilterObservable(this, predicate, thisArg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.window"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>window (windowOpeningsOrClosingSelector, windowClosingSelector)](#apidoc.element.rx.Observable.prototype.window)
- description and source-code
```javascript
window = function (windowOpeningsOrClosingSelector, windowClosingSelector) {
  if (arguments.length === 1 && typeof arguments[0] !== 'function') {
    return observableWindowWithBoundaries.call(this, windowOpeningsOrClosingSelector);
  }
  return typeof windowOpeningsOrClosingSelector === 'function' ?
    observableWindowWithClosingSelector.call(this, windowOpeningsOrClosingSelector) :
    observableWindowWithOpenings.call(this, windowOpeningsOrClosingSelector, windowClosingSelector);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.windowCount"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowCount (count, skip)](#apidoc.element.rx.Observable.prototype.windowCount)
- description and source-code
```javascript
windowCount = function (count, skip) {
  var source = this;
  +count || (count = 0);
  Math.abs(count) === Infinity && (count = 0);
  if (count <= 0) { throw new ArgumentOutOfRangeError(); }
  skip == null && (skip = count);
  +skip || (skip = 0);
  Math.abs(skip) === Infinity && (skip = 0);

  if (skip <= 0) { throw new ArgumentOutOfRangeError(); }
  return new AnonymousObservable(function (observer) {
    var m = new SingleAssignmentDisposable(),
      refCountDisposable = new RefCountDisposable(m),
      n = 0,
      q = [];

    function createWindow () {
      var s = new Subject();
      q.push(s);
      observer.onNext(addRef(s, refCountDisposable));
    }

    createWindow();

    m.setDisposable(source.subscribe(
      function (x) {
        for (var i = 0, len = q.length; i < len; i++) { q[i].onNext(x); }
        var c = n - count + 1;
        c >= 0 && c % skip === 0 && q.shift().onCompleted();
        ++n % skip === 0 && createWindow();
      },
      function (e) {
        while (q.length > 0) { q.shift().onError(e); }
        observer.onError(e);
      },
      function () {
        while (q.length > 0) { q.shift().onCompleted(); }
        observer.onCompleted();
      }
    ));
    return refCountDisposable;
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.windowTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowTime (timeSpan, timeShiftOrScheduler, scheduler)](#apidoc.element.rx.Observable.prototype.windowTime)
- description and source-code
```javascript
windowTime = function (timeSpan, timeShiftOrScheduler, scheduler) {
  var source = this, timeShift;
  timeShiftOrScheduler == null && (timeShift = timeSpan);
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  if (typeof timeShiftOrScheduler === 'number') {
    timeShift = timeShiftOrScheduler;
  } else if (isScheduler(timeShiftOrScheduler)) {
    timeShift = timeSpan;
    scheduler = timeShiftOrScheduler;
  }
  return new AnonymousObservable(function (observer) {
    var groupDisposable,
      nextShift = timeShift,
      nextSpan = timeSpan,
      q = [],
      refCountDisposable,
      timerD = new SerialDisposable(),
      totalTime = 0;
      groupDisposable = new CompositeDisposable(timerD),
      refCountDisposable = new RefCountDisposable(groupDisposable);

     function createTimer () {
      var m = new SingleAssignmentDisposable(),
        isSpan = false,
        isShift = false;
      timerD.setDisposable(m);
      if (nextSpan === nextShift) {
        isSpan = true;
        isShift = true;
      } else if (nextSpan < nextShift) {
          isSpan = true;
      } else {
        isShift = true;
      }
      var newTotalTime = isSpan ? nextSpan : nextShift,
        ts = newTotalTime - totalTime;
      totalTime = newTotalTime;
      if (isSpan) {
        nextSpan += timeShift;
      }
      if (isShift) {
        nextShift += timeShift;
      }
      m.setDisposable(scheduler.scheduleFuture(null, ts, function () {
        if (isShift) {
          var s = new Subject();
          q.push(s);
          observer.onNext(addRef(s, refCountDisposable));
        }
        isSpan && q.shift().onCompleted();
        createTimer();
      }));
    };
    q.push(new Subject());
    observer.onNext(addRef(q[0], refCountDisposable));
    createTimer();
    groupDisposable.add(source.subscribe(
      function (x) {
        for (var i = 0, len = q.length; i < len; i++) { q[i].onNext(x); }
      },
      function (e) {
        for (var i = 0, len = q.length; i < len; i++) { q[i].onError(e); }
        observer.onError(e);
      },
      function () {
        for (var i = 0, len = q.length; i < len; i++) { q[i].onCompleted(); }
        observer.onCompleted();
      }
    ));
    return refCountDisposable;
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.windowTimeOrCount"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowTimeOrCount (timeSpan, count, scheduler)](#apidoc.element.rx.Observable.prototype.windowTimeOrCount)
- description and source-code
```javascript
windowTimeOrCount = function (timeSpan, count, scheduler) {
  var source = this;
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new AnonymousObservable(function (observer) {
    var timerD = new SerialDisposable(),
        groupDisposable = new CompositeDisposable(timerD),
        refCountDisposable = new RefCountDisposable(groupDisposable),
        n = 0,
        windowId = 0,
        s = new Subject();

    function createTimer(id) {
      var m = new SingleAssignmentDisposable();
      timerD.setDisposable(m);
      m.setDisposable(scheduler.scheduleFuture(null, timeSpan, function () {
        if (id !== windowId) { return; }
        n = 0;
        var newId = ++windowId;
        s.onCompleted();
        s = new Subject();
        observer.onNext(addRef(s, refCountDisposable));
        createTimer(newId);
      }));
    }

    observer.onNext(addRef(s, refCountDisposable));
    createTimer(0);

    groupDisposable.add(source.subscribe(
      function (x) {
        var newId = 0, newWindow = false;
        s.onNext(x);
        if (++n === count) {
          newWindow = true;
          n = 0;
          newId = ++windowId;
          s.onCompleted();
          s = new Subject();
          observer.onNext(addRef(s, refCountDisposable));
        }
        newWindow && createTimer(newId);
      },
      function (e) {
        s.onError(e);
        observer.onError(e);
      }, function () {
        s.onCompleted();
        observer.onCompleted();
      }
    ));
    return refCountDisposable;
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.windowWithCount"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowWithCount (count, skip)](#apidoc.element.rx.Observable.prototype.windowWithCount)
- description and source-code
```javascript
windowWithCount = function (count, skip) {
  var source = this;
  +count || (count = 0);
  Math.abs(count) === Infinity && (count = 0);
  if (count <= 0) { throw new ArgumentOutOfRangeError(); }
  skip == null && (skip = count);
  +skip || (skip = 0);
  Math.abs(skip) === Infinity && (skip = 0);

  if (skip <= 0) { throw new ArgumentOutOfRangeError(); }
  return new AnonymousObservable(function (observer) {
    var m = new SingleAssignmentDisposable(),
      refCountDisposable = new RefCountDisposable(m),
      n = 0,
      q = [];

    function createWindow () {
      var s = new Subject();
      q.push(s);
      observer.onNext(addRef(s, refCountDisposable));
    }

    createWindow();

    m.setDisposable(source.subscribe(
      function (x) {
        for (var i = 0, len = q.length; i < len; i++) { q[i].onNext(x); }
        var c = n - count + 1;
        c >= 0 && c % skip === 0 && q.shift().onCompleted();
        ++n % skip === 0 && createWindow();
      },
      function (e) {
        while (q.length > 0) { q.shift().onError(e); }
        observer.onError(e);
      },
      function () {
        while (q.length > 0) { q.shift().onCompleted(); }
        observer.onCompleted();
      }
    ));
    return refCountDisposable;
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.windowWithTime"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowWithTime (timeSpan, timeShiftOrScheduler, scheduler)](#apidoc.element.rx.Observable.prototype.windowWithTime)
- description and source-code
```javascript
windowWithTime = function (timeSpan, timeShiftOrScheduler, scheduler) {
  var source = this, timeShift;
  timeShiftOrScheduler == null && (timeShift = timeSpan);
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  if (typeof timeShiftOrScheduler === 'number') {
    timeShift = timeShiftOrScheduler;
  } else if (isScheduler(timeShiftOrScheduler)) {
    timeShift = timeSpan;
    scheduler = timeShiftOrScheduler;
  }
  return new AnonymousObservable(function (observer) {
    var groupDisposable,
      nextShift = timeShift,
      nextSpan = timeSpan,
      q = [],
      refCountDisposable,
      timerD = new SerialDisposable(),
      totalTime = 0;
      groupDisposable = new CompositeDisposable(timerD),
      refCountDisposable = new RefCountDisposable(groupDisposable);

     function createTimer () {
      var m = new SingleAssignmentDisposable(),
        isSpan = false,
        isShift = false;
      timerD.setDisposable(m);
      if (nextSpan === nextShift) {
        isSpan = true;
        isShift = true;
      } else if (nextSpan < nextShift) {
          isSpan = true;
      } else {
        isShift = true;
      }
      var newTotalTime = isSpan ? nextSpan : nextShift,
        ts = newTotalTime - totalTime;
      totalTime = newTotalTime;
      if (isSpan) {
        nextSpan += timeShift;
      }
      if (isShift) {
        nextShift += timeShift;
      }
      m.setDisposable(scheduler.scheduleFuture(null, ts, function () {
        if (isShift) {
          var s = new Subject();
          q.push(s);
          observer.onNext(addRef(s, refCountDisposable));
        }
        isSpan && q.shift().onCompleted();
        createTimer();
      }));
    };
    q.push(new Subject());
    observer.onNext(addRef(q[0], refCountDisposable));
    createTimer();
    groupDisposable.add(source.subscribe(
      function (x) {
        for (var i = 0, len = q.length; i < len; i++) { q[i].onNext(x); }
      },
      function (e) {
        for (var i = 0, len = q.length; i < len; i++) { q[i].onError(e); }
        observer.onError(e);
      },
      function () {
        for (var i = 0, len = q.length; i < len; i++) { q[i].onCompleted(); }
        observer.onCompleted();
      }
    ));
    return refCountDisposable;
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.windowWithTimeOrCount"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>windowWithTimeOrCount (timeSpan, count, scheduler)](#apidoc.element.rx.Observable.prototype.windowWithTimeOrCount)
- description and source-code
```javascript
windowWithTimeOrCount = function (timeSpan, count, scheduler) {
  var source = this;
  isScheduler(scheduler) || (scheduler = defaultScheduler);
  return new AnonymousObservable(function (observer) {
    var timerD = new SerialDisposable(),
        groupDisposable = new CompositeDisposable(timerD),
        refCountDisposable = new RefCountDisposable(groupDisposable),
        n = 0,
        windowId = 0,
        s = new Subject();

    function createTimer(id) {
      var m = new SingleAssignmentDisposable();
      timerD.setDisposable(m);
      m.setDisposable(scheduler.scheduleFuture(null, timeSpan, function () {
        if (id !== windowId) { return; }
        n = 0;
        var newId = ++windowId;
        s.onCompleted();
        s = new Subject();
        observer.onNext(addRef(s, refCountDisposable));
        createTimer(newId);
      }));
    }

    observer.onNext(addRef(s, refCountDisposable));
    createTimer(0);

    groupDisposable.add(source.subscribe(
      function (x) {
        var newId = 0, newWindow = false;
        s.onNext(x);
        if (++n === count) {
          newWindow = true;
          n = 0;
          newId = ++windowId;
          s.onCompleted();
          s = new Subject();
          observer.onNext(addRef(s, refCountDisposable));
        }
        newWindow && createTimer(newId);
      },
      function (e) {
        s.onError(e);
        observer.onError(e);
      }, function () {
        s.onCompleted();
        observer.onCompleted();
      }
    ));
    return refCountDisposable;
  }, source);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.withLatestFrom"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>withLatestFrom ()](#apidoc.element.rx.Observable.prototype.withLatestFrom)
- description and source-code
```javascript
withLatestFrom = function () {
  if (arguments.length === 0) { throw new Error('invalid arguments'); }

  var len = arguments.length, args = new Array(len);
  for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  var resultSelector = isFunction(args[len - 1]) ? args.pop() : argumentsToArray;
  Array.isArray(args[0]) && (args = args[0]);

  return new WithLatestFromObservable(this, args, resultSelector);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.zip"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>zip ()](#apidoc.element.rx.Observable.prototype.zip)
- description and source-code
```javascript
zip = function () {
  if (arguments.length === 0) { throw new Error('invalid arguments'); }

  var len = arguments.length, args = new Array(len);
  for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  var resultSelector = isFunction(args[len - 1]) ? args.pop() : argumentsToArray;
  Array.isArray(args[0]) && (args = args[0]);

  var parent = this;
  args.unshift(parent);

  return new ZipObservable(args, resultSelector);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observable.prototype.zipIterable"></a>[function <span class="apidocSignatureSpan">rx.Observable.prototype.</span>zipIterable ()](#apidoc.element.rx.Observable.prototype.zipIterable)
- description and source-code
```javascript
zipIterable = function () {
  if (arguments.length === 0) { throw new Error('invalid arguments'); }

  var len = arguments.length, args = new Array(len);
  for(var i = 0; i < len; i++) { args[i] = arguments[i]; }
  var resultSelector = isFunction(args[len - 1]) ? args.pop() : argumentsToArray;

  var parent = this;
  args.unshift(parent);
  return new ZipIterableObservable(args, resultSelector);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.ObservableBase"></a>[module rx.ObservableBase](#apidoc.module.rx.ObservableBase)

#### <a name="apidoc.element.rx.ObservableBase.ObservableBase"></a>[function <span class="apidocSignatureSpan">rx.</span>ObservableBase ()](#apidoc.element.rx.ObservableBase.ObservableBase)
- description and source-code
```javascript
function ObservableBase() {
  __super__.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.ObservableBase.prototype"></a>[module rx.ObservableBase.prototype](#apidoc.module.rx.ObservableBase.prototype)

#### <a name="apidoc.element.rx.ObservableBase.prototype._subscribe"></a>[function <span class="apidocSignatureSpan">rx.ObservableBase.prototype.</span>_subscribe (o)](#apidoc.element.rx.ObservableBase.prototype._subscribe)
- description and source-code
```javascript
_subscribe = function (o) {
  var ado = new AutoDetachObserver(o), state = [ado, this];

  if (currentThreadScheduler.scheduleRequired()) {
    currentThreadScheduler.schedule(state, setDisposable);
  } else {
    setDisposable(null, state);
  }
  return ado;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ObservableBase.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.ObservableBase.prototype.</span>constructor ()](#apidoc.element.rx.ObservableBase.prototype.constructor)
- description and source-code
```javascript
function ObservableBase() {
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ObservableBase.prototype.subscribeCore"></a>[function <span class="apidocSignatureSpan">rx.ObservableBase.prototype.</span>subscribeCore ()](#apidoc.element.rx.ObservableBase.prototype.subscribeCore)
- description and source-code
```javascript
subscribeCore = function () {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Observer"></a>[module rx.Observer](#apidoc.module.rx.Observer)

#### <a name="apidoc.element.rx.Observer.Observer"></a>[function <span class="apidocSignatureSpan">rx.</span>Observer ()](#apidoc.element.rx.Observer.Observer)
- description and source-code
```javascript
Observer = function () { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observer.create"></a>[function <span class="apidocSignatureSpan">rx.Observer.</span>create (onNext, onError, onCompleted)](#apidoc.element.rx.Observer.create)
- description and source-code
```javascript
create = function (onNext, onError, onCompleted) {
  onNext || (onNext = noop);
  onError || (onError = defaultError);
  onCompleted || (onCompleted = noop);
  return new AnonymousObserver(onNext, onError, onCompleted);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observer.fromNotifier"></a>[function <span class="apidocSignatureSpan">rx.Observer.</span>fromNotifier (handler, thisArg)](#apidoc.element.rx.Observer.fromNotifier)
- description and source-code
```javascript
fromNotifier = function (handler, thisArg) {
  var cb = bindCallback(handler, thisArg, 1);
  return new AnonymousObserver(function (x) {
    return cb(notificationCreateOnNext(x));
  }, function (e) {
    return cb(notificationCreateOnError(e));
  }, function () {
    return cb(notificationCreateOnCompleted());
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Observer.prototype"></a>[module rx.Observer.prototype](#apidoc.module.rx.Observer.prototype)

#### <a name="apidoc.element.rx.Observer.prototype.asObserver"></a>[function <span class="apidocSignatureSpan">rx.Observer.prototype.</span>asObserver ()](#apidoc.element.rx.Observer.prototype.asObserver)
- description and source-code
```javascript
asObserver = function () {
  var self = this;
  return new AnonymousObserver(
    function (x) { self.onNext(x); },
    function (err) { self.onError(err); },
    function () { self.onCompleted(); });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observer.prototype.checked"></a>[function <span class="apidocSignatureSpan">rx.Observer.prototype.</span>checked ()](#apidoc.element.rx.Observer.prototype.checked)
- description and source-code
```javascript
checked = function () { return new CheckedObserver(this); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observer.prototype.makeSafe"></a>[function <span class="apidocSignatureSpan">rx.Observer.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.Observer.prototype.makeSafe)
- description and source-code
```javascript
makeSafe = function (disposable) {
  return new AnonymousSafeObserver(this._onNext, this._onError, this._onCompleted, disposable);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observer.prototype.notifyOn"></a>[function <span class="apidocSignatureSpan">rx.Observer.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.Observer.prototype.notifyOn)
- description and source-code
```javascript
notifyOn = function (scheduler) {
  return new ObserveOnObserver(scheduler, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Observer.prototype.toNotifier"></a>[function <span class="apidocSignatureSpan">rx.Observer.prototype.</span>toNotifier ()](#apidoc.element.rx.Observer.prototype.toNotifier)
- description and source-code
```javascript
toNotifier = function () {
  var observer = this;
  return function (n) { return n.accept(observer); };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Pauser"></a>[module rx.Pauser](#apidoc.module.rx.Pauser)

#### <a name="apidoc.element.rx.Pauser.Pauser"></a>[function <span class="apidocSignatureSpan">rx.</span>Pauser ()](#apidoc.element.rx.Pauser.Pauser)
- description and source-code
```javascript
function Pauser() {
  __super__.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Pauser.prototype"></a>[module rx.Pauser.prototype](#apidoc.module.rx.Pauser.prototype)

#### <a name="apidoc.element.rx.Pauser.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.Pauser.prototype.</span>constructor ()](#apidoc.element.rx.Pauser.prototype.constructor)
- description and source-code
```javascript
function Pauser() {
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Pauser.prototype.pause"></a>[function <span class="apidocSignatureSpan">rx.Pauser.prototype.</span>pause ()](#apidoc.element.rx.Pauser.prototype.pause)
- description and source-code
```javascript
pause = function () { this.onNext(false); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Pauser.prototype.resume"></a>[function <span class="apidocSignatureSpan">rx.Pauser.prototype.</span>resume ()](#apidoc.element.rx.Pauser.prototype.resume)
- description and source-code
```javascript
resume = function () { this.onNext(true); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.ReactiveTest"></a>[module rx.ReactiveTest](#apidoc.module.rx.ReactiveTest)

#### <a name="apidoc.element.rx.ReactiveTest.onCompleted"></a>[function <span class="apidocSignatureSpan">rx.ReactiveTest.</span>onCompleted (ticks)](#apidoc.element.rx.ReactiveTest.onCompleted)
- description and source-code
```javascript
onCompleted = function (ticks) {
  return new Recorded(ticks, Notification.createOnCompleted());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReactiveTest.onError"></a>[function <span class="apidocSignatureSpan">rx.ReactiveTest.</span>onError (ticks, error)](#apidoc.element.rx.ReactiveTest.onError)
- description and source-code
```javascript
onError = function (ticks, error) {
  return typeof error === 'function' ?
    new Recorded(ticks, new OnErrorPredicate(error)) :
    new Recorded(ticks, Notification.createOnError(error));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReactiveTest.onNext"></a>[function <span class="apidocSignatureSpan">rx.ReactiveTest.</span>onNext (ticks, value)](#apidoc.element.rx.ReactiveTest.onNext)
- description and source-code
```javascript
onNext = function (ticks, value) {
  return typeof value === 'function' ?
    new Recorded(ticks, new OnNextPredicate(value)) :
    new Recorded(ticks, Notification.createOnNext(value));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReactiveTest.subscribe"></a>[function <span class="apidocSignatureSpan">rx.ReactiveTest.</span>subscribe (start, end)](#apidoc.element.rx.ReactiveTest.subscribe)
- description and source-code
```javascript
subscribe = function (start, end) {
  return new Subscription(start, end);
}
```
- example usage
```shell
...
'''js
/* Get stock data somehow */
const source = getAsyncStockData();

const subscription = source
  .filter(quote => quote.price > 30)
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''
...
```



# <a name="apidoc.module.rx.Recorded"></a>[module rx.Recorded](#apidoc.module.rx.Recorded)

#### <a name="apidoc.element.rx.Recorded.Recorded"></a>[function <span class="apidocSignatureSpan">rx.</span>Recorded (time, value, comparer)](#apidoc.element.rx.Recorded.Recorded)
- description and source-code
```javascript
Recorded = function (time, value, comparer) {
  this.time = time;
  this.value = value;
  this.comparer = comparer || defaultComparer;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Recorded.prototype"></a>[module rx.Recorded.prototype](#apidoc.module.rx.Recorded.prototype)

#### <a name="apidoc.element.rx.Recorded.prototype.equals"></a>[function <span class="apidocSignatureSpan">rx.Recorded.prototype.</span>equals (other)](#apidoc.element.rx.Recorded.prototype.equals)
- description and source-code
```javascript
equals = function (other) {
  return this.time === other.time && this.comparer(this.value, other.value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Recorded.prototype.toString"></a>[function <span class="apidocSignatureSpan">rx.Recorded.prototype.</span>toString ()](#apidoc.element.rx.Recorded.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.value.toString() + '@' + this.time;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.RefCountDisposable"></a>[module rx.RefCountDisposable](#apidoc.module.rx.RefCountDisposable)

#### <a name="apidoc.element.rx.RefCountDisposable.RefCountDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>RefCountDisposable (disposable)](#apidoc.element.rx.RefCountDisposable.RefCountDisposable)
- description and source-code
```javascript
function RefCountDisposable(disposable) {
  this.underlyingDisposable = disposable;
  this.isDisposed = false;
  this.isPrimaryDisposed = false;
  this.count = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.RefCountDisposable.prototype"></a>[module rx.RefCountDisposable.prototype](#apidoc.module.rx.RefCountDisposable.prototype)

#### <a name="apidoc.element.rx.RefCountDisposable.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.RefCountDisposable.prototype.</span>dispose ()](#apidoc.element.rx.RefCountDisposable.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  if (!this.isDisposed && !this.isPrimaryDisposed) {
    this.isPrimaryDisposed = true;
    if (this.count === 0) {
      this.isDisposed = true;
      this.underlyingDisposable.dispose();
    }
  }
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```

#### <a name="apidoc.element.rx.RefCountDisposable.prototype.getDisposable"></a>[function <span class="apidocSignatureSpan">rx.RefCountDisposable.prototype.</span>getDisposable ()](#apidoc.element.rx.RefCountDisposable.prototype.getDisposable)
- description and source-code
```javascript
getDisposable = function () {
  return this.isDisposed ? disposableEmpty : new InnerDisposable(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.ReplaySubject"></a>[module rx.ReplaySubject](#apidoc.module.rx.ReplaySubject)

#### <a name="apidoc.element.rx.ReplaySubject.ReplaySubject"></a>[function <span class="apidocSignatureSpan">rx.</span>ReplaySubject (bufferSize, windowSize, scheduler)](#apidoc.element.rx.ReplaySubject.ReplaySubject)
- description and source-code
```javascript
function ReplaySubject(bufferSize, windowSize, scheduler) {
  this.bufferSize = bufferSize == null ? maxSafeInteger : bufferSize;
  this.windowSize = windowSize == null ? maxSafeInteger : windowSize;
  this.scheduler = scheduler || currentThreadScheduler;
  this.q = [];
  this.observers = [];
  this.isStopped = false;
  this.isDisposed = false;
  this.hasError = false;
  this.error = null;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.ReplaySubject.prototype"></a>[module rx.ReplaySubject.prototype](#apidoc.module.rx.ReplaySubject.prototype)

#### <a name="apidoc.element.rx.ReplaySubject.prototype._subscribe"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>_subscribe (o)](#apidoc.element.rx.ReplaySubject.prototype._subscribe)
- description and source-code
```javascript
_subscribe = function (o) {
  checkDisposed(this);
  var so = new ScheduledObserver(this.scheduler, o), subscription = createRemovableDisposable(this, so);

  this._trim(this.scheduler.now());
  this.observers.push(so);

  for (var i = 0, len = this.q.length; i < len; i++) {
    so.onNext(this.q[i].value);
  }

  if (this.hasError) {
    so.onError(this.error);
  } else if (this.isStopped) {
    so.onCompleted();
  }

  so.ensureActive();
  return subscription;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype._trim"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>_trim (now)](#apidoc.element.rx.ReplaySubject.prototype._trim)
- description and source-code
```javascript
_trim = function (now) {
  while (this.q.length > this.bufferSize) {
    this.q.shift();
  }
  while (this.q.length > 0 && (now - this.q[0].interval) > this.windowSize) {
    this.q.shift();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.asObserver"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>asObserver ()](#apidoc.element.rx.ReplaySubject.prototype.asObserver)
- description and source-code
```javascript
asObserver = function () {
  var self = this;
  return new AnonymousObserver(
    function (x) { self.onNext(x); },
    function (err) { self.onError(err); },
    function () { self.onCompleted(); });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.checked"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>checked ()](#apidoc.element.rx.ReplaySubject.prototype.checked)
- description and source-code
```javascript
checked = function () { return new CheckedObserver(this); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>constructor (bufferSize, windowSize, scheduler)](#apidoc.element.rx.ReplaySubject.prototype.constructor)
- description and source-code
```javascript
function ReplaySubject(bufferSize, windowSize, scheduler) {
  this.bufferSize = bufferSize == null ? maxSafeInteger : bufferSize;
  this.windowSize = windowSize == null ? maxSafeInteger : windowSize;
  this.scheduler = scheduler || currentThreadScheduler;
  this.q = [];
  this.observers = [];
  this.isStopped = false;
  this.isDisposed = false;
  this.hasError = false;
  this.error = null;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>dispose ()](#apidoc.element.rx.ReplaySubject.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  this.isDisposed = true;
  this.observers = null;
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.hasObservers"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>hasObservers ()](#apidoc.element.rx.ReplaySubject.prototype.hasObservers)
- description and source-code
```javascript
hasObservers = function () { checkDisposed(this); return this.observers.length > 0; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.makeSafe"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.ReplaySubject.prototype.makeSafe)
- description and source-code
```javascript
makeSafe = function (disposable) {
  return new AnonymousSafeObserver(this._onNext, this._onError, this._onCompleted, disposable);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.notifyOn"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.ReplaySubject.prototype.notifyOn)
- description and source-code
```javascript
notifyOn = function (scheduler) {
  return new ObserveOnObserver(scheduler, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.onCompleted"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>onCompleted ()](#apidoc.element.rx.ReplaySubject.prototype.onCompleted)
- description and source-code
```javascript
onCompleted = function () {
  checkDisposed(this);
  if (this.isStopped) { return; }
  this.isStopped = true;
  var now = this.scheduler.now();
  this._trim(now);
  for (var i = 0, os = cloneArray(this.observers), len = os.length; i < len; i++) {
    var observer = os[i];
    observer.onCompleted();
    observer.ensureActive();
  }
  this.observers.length = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.onError"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>onError (error)](#apidoc.element.rx.ReplaySubject.prototype.onError)
- description and source-code
```javascript
onError = function (error) {
  checkDisposed(this);
  if (this.isStopped) { return; }
  this.isStopped = true;
  this.error = error;
  this.hasError = true;
  var now = this.scheduler.now();
  this._trim(now);
  for (var i = 0, os = cloneArray(this.observers), len = os.length; i < len; i++) {
    var observer = os[i];
    observer.onError(error);
    observer.ensureActive();
  }
  this.observers.length = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.onNext"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>onNext (value)](#apidoc.element.rx.ReplaySubject.prototype.onNext)
- description and source-code
```javascript
onNext = function (value) {
  checkDisposed(this);
  if (this.isStopped) { return; }
  var now = this.scheduler.now();
  this.q.push({ interval: now, value: value });
  this._trim(now);

  for (var i = 0, os = cloneArray(this.observers), len = os.length; i < len; i++) {
    var observer = os[i];
    observer.onNext(value);
    observer.ensureActive();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.ReplaySubject.prototype.toNotifier"></a>[function <span class="apidocSignatureSpan">rx.ReplaySubject.prototype.</span>toNotifier ()](#apidoc.element.rx.ReplaySubject.prototype.toNotifier)
- description and source-code
```javascript
toNotifier = function () {
  var observer = this;
  return function (n) { return n.accept(observer); };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Rx"></a>[module rx.Rx](#apidoc.module.rx.Rx)

#### <a name="apidoc.element.rx.Rx.AnonymousObservable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>AnonymousObservable (subscribe, parent)](#apidoc.element.rx.Rx.AnonymousObservable)
- description and source-code
```javascript
function AnonymousObservable(subscribe, parent) {
  this.source = parent;
  this.__subscribe = subscribe;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.AnonymousObserver"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>AnonymousObserver (onNext, onError, onCompleted)](#apidoc.element.rx.Rx.AnonymousObserver)
- description and source-code
```javascript
function AnonymousObserver(onNext, onError, onCompleted) {
  __super__.call(this);
  this._onNext = onNext;
  this._onError = onError;
  this._onCompleted = onCompleted;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.AnonymousSubject"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>AnonymousSubject (observer, observable)](#apidoc.element.rx.Rx.AnonymousSubject)
- description and source-code
```javascript
function AnonymousSubject(observer, observable) {
  this.observer = observer;
  this.observable = observable;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.ArgumentOutOfRangeError"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>ArgumentOutOfRangeError ()](#apidoc.element.rx.Rx.ArgumentOutOfRangeError)
- description and source-code
```javascript
ArgumentOutOfRangeError = function () {
  this.message = 'Argument out of range';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.AsyncSubject"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>AsyncSubject ()](#apidoc.element.rx.Rx.AsyncSubject)
- description and source-code
```javascript
function AsyncSubject() {
  __super__.call(this);
  this.isDisposed = false;
  this.isStopped = false;
  this.hasValue = false;
  this.observers = [];
  this.hasError = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.BehaviorSubject"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>BehaviorSubject (value)](#apidoc.element.rx.Rx.BehaviorSubject)
- description and source-code
```javascript
function BehaviorSubject(value) {
  __super__.call(this);
  this.value = value;
  this.observers = [];
  this.isDisposed = false;
  this.isStopped = false;
  this.hasError = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.BinaryDisposable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>BinaryDisposable (first, second)](#apidoc.element.rx.Rx.BinaryDisposable)
- description and source-code
```javascript
BinaryDisposable = function (first, second) {
  this._first = first;
  this._second = second;
  this.isDisposed = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.CompositeDisposable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>CompositeDisposable ()](#apidoc.element.rx.Rx.CompositeDisposable)
- description and source-code
```javascript
CompositeDisposable = function () {
  var args = [], i, len;
  if (Array.isArray(arguments[0])) {
    args = arguments[0];
  } else {
    len = arguments.length;
    args = new Array(len);
    for(i = 0; i < len; i++) { args[i] = arguments[i]; }
  }
  this.disposables = args;
  this.isDisposed = false;
  this.length = args.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.CompositeError"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>CompositeError (errors)](#apidoc.element.rx.Rx.CompositeError)
- description and source-code
```javascript
CompositeError = function (errors) {
  this.innerErrors = errors;
  this.message = 'This contains multiple errors. Check the innerErrors';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.ConnectableObservable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>ConnectableObservable (source, subject)](#apidoc.element.rx.Rx.ConnectableObservable)
- description and source-code
```javascript
function ConnectableObservable(source, subject) {
  this.source = source;
  this._connection = null;
  this._source = source.asObservable();
  this._subject = subject;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.Disposable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>Disposable (action)](#apidoc.element.rx.Rx.Disposable)
- description and source-code
```javascript
Disposable = function (action) {
  this.isDisposed = false;
  this.action = action || noop;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.EmptyError"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>EmptyError ()](#apidoc.element.rx.Rx.EmptyError)
- description and source-code
```javascript
EmptyError = function () {
  this.message = 'Sequence contains no elements.';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.FlatMapObservable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>FlatMapObservable (source, selector, resultSelector, thisArg)](#apidoc.element.rx.Rx.FlatMapObservable)
- description and source-code
```javascript
function FlatMapObservable(source, selector, resultSelector, thisArg) {
  this.resultSelector = isFunction(resultSelector) ? resultSelector : null;
  this.selector = bindCallback(isFunction(selector) ? selector : function() { return selector; }, thisArg, 3);
  this.source = source;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.HistoricalScheduler"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>HistoricalScheduler (initialClock, comparer)](#apidoc.element.rx.Rx.HistoricalScheduler)
- description and source-code
```javascript
function HistoricalScheduler(initialClock, comparer) {
  var clock = initialClock == null ? 0 : initialClock;
  var cmp = comparer || defaultSubComparer;
  __super__.call(this, clock, cmp);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.MockDisposable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>MockDisposable (scheduler)](#apidoc.element.rx.Rx.MockDisposable)
- description and source-code
```javascript
MockDisposable = function (scheduler) {
  this.scheduler = scheduler;
  this.disposes = [];
  this.disposes.push(this.scheduler.clock);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.NAryDisposable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>NAryDisposable (disposables)](#apidoc.element.rx.Rx.NAryDisposable)
- description and source-code
```javascript
NAryDisposable = function (disposables) {
  this._disposables = disposables;
  this.isDisposed = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.NotImplementedError"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>NotImplementedError (message)](#apidoc.element.rx.Rx.NotImplementedError)
- description and source-code
```javascript
NotImplementedError = function (message) {
  this.message = message || 'This operation is not implemented';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.NotSupportedError"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>NotSupportedError (message)](#apidoc.element.rx.Rx.NotSupportedError)
- description and source-code
```javascript
NotSupportedError = function (message) {
  this.message = message || 'This operation is not supported';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.Notification"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>Notification ()](#apidoc.element.rx.Rx.Notification)
- description and source-code
```javascript
function Notification() {

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.ObjectDisposedError"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>ObjectDisposedError ()](#apidoc.element.rx.Rx.ObjectDisposedError)
- description and source-code
```javascript
ObjectDisposedError = function () {
  this.message = 'Object has been disposed';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.Observable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>Observable ()](#apidoc.element.rx.Rx.Observable)
- description and source-code
```javascript
function Observable() {
  if (Rx.config.longStackSupport && hasStacks) {
    var oldSubscribe = this._subscribe;
    var e = tryCatch(thrower)(new Error()).e;
    this.stack = e.stack.substring(e.stack.indexOf('\n') + 1);
    this._subscribe = makeSubscribe(this, oldSubscribe);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.ObservableBase"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>ObservableBase ()](#apidoc.element.rx.Rx.ObservableBase)
- description and source-code
```javascript
function ObservableBase() {
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.Observer"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>Observer ()](#apidoc.element.rx.Rx.Observer)
- description and source-code
```javascript
Observer = function () { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.Pauser"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>Pauser ()](#apidoc.element.rx.Rx.Pauser)
- description and source-code
```javascript
function Pauser() {
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.Recorded"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>Recorded (time, value, comparer)](#apidoc.element.rx.Rx.Recorded)
- description and source-code
```javascript
Recorded = function (time, value, comparer) {
  this.time = time;
  this.value = value;
  this.comparer = comparer || defaultComparer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.RefCountDisposable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>RefCountDisposable (disposable)](#apidoc.element.rx.Rx.RefCountDisposable)
- description and source-code
```javascript
function RefCountDisposable(disposable) {
  this.underlyingDisposable = disposable;
  this.isDisposed = false;
  this.isPrimaryDisposed = false;
  this.count = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.ReplaySubject"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>ReplaySubject (bufferSize, windowSize, scheduler)](#apidoc.element.rx.Rx.ReplaySubject)
- description and source-code
```javascript
function ReplaySubject(bufferSize, windowSize, scheduler) {
  this.bufferSize = bufferSize == null ? maxSafeInteger : bufferSize;
  this.windowSize = windowSize == null ? maxSafeInteger : windowSize;
  this.scheduler = scheduler || currentThreadScheduler;
  this.q = [];
  this.observers = [];
  this.isStopped = false;
  this.isDisposed = false;
  this.hasError = false;
  this.error = null;
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.Scheduler"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>Scheduler ()](#apidoc.element.rx.Rx.Scheduler)
- description and source-code
```javascript
function Scheduler() { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.SerialDisposable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>SerialDisposable ()](#apidoc.element.rx.Rx.SerialDisposable)
- description and source-code
```javascript
SerialDisposable = function () {
  this.isDisposed = false;
  this.current = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.SingleAssignmentDisposable"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>SingleAssignmentDisposable ()](#apidoc.element.rx.Rx.SingleAssignmentDisposable)
- description and source-code
```javascript
SingleAssignmentDisposable = function () {
  this.isDisposed = false;
  this.current = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.Subject"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>Subject ()](#apidoc.element.rx.Rx.Subject)
- description and source-code
```javascript
function Subject() {
  __super__.call(this);
  this.isDisposed = false;
  this.isStopped = false;
  this.observers = [];
  this.hasError = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.Subscription"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>Subscription (start, end)](#apidoc.element.rx.Rx.Subscription)
- description and source-code
```javascript
Subscription = function (start, end) {
  this.subscribe = start;
  this.unsubscribe = end || Number.MAX_VALUE;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.TestScheduler"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>TestScheduler ()](#apidoc.element.rx.Rx.TestScheduler)
- description and source-code
```javascript
function TestScheduler() {
  __super__.call(this, 0, baseComparer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.TimeoutError"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>TimeoutError (message)](#apidoc.element.rx.Rx.TimeoutError)
- description and source-code
```javascript
TimeoutError = function (message) {
  this.message = message || 'Timeout has occurred';
  this.name = 'TimeoutError';
  Error.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Rx.VirtualTimeScheduler"></a>[function <span class="apidocSignatureSpan">rx.Rx.</span>VirtualTimeScheduler (initialClock, comparer)](#apidoc.element.rx.Rx.VirtualTimeScheduler)
- description and source-code
```javascript
function VirtualTimeScheduler(initialClock, comparer) {
  this.clock = initialClock;
  this.comparer = comparer;
  this.isEnabled = false;
  this.queue = new PriorityQueue(1024);
  __super__.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Scheduler"></a>[module rx.Scheduler](#apidoc.module.rx.Scheduler)

#### <a name="apidoc.element.rx.Scheduler.Scheduler"></a>[function <span class="apidocSignatureSpan">rx.</span>Scheduler ()](#apidoc.element.rx.Scheduler.Scheduler)
- description and source-code
```javascript
function Scheduler() { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.isScheduler"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.</span>isScheduler (s)](#apidoc.element.rx.Scheduler.isScheduler)
- description and source-code
```javascript
isScheduler = function (s) {
  return s instanceof Scheduler;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.normalize"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.</span>normalize (timeSpan)](#apidoc.element.rx.Scheduler.normalize)
- description and source-code
```javascript
normalize = function (timeSpan) {
  timeSpan < 0 && (timeSpan = 0);
  return timeSpan;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.now"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.</span>now ()](#apidoc.element.rx.Scheduler.now)
- description and source-code
```javascript
function now() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Scheduler.prototype"></a>[module rx.Scheduler.prototype](#apidoc.module.rx.Scheduler.prototype)

#### <a name="apidoc.element.rx.Scheduler.prototype._scheduleFuture"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>_scheduleFuture (state, dueTime, action)](#apidoc.element.rx.Scheduler.prototype._scheduleFuture)
- description and source-code
```javascript
_scheduleFuture = function (state, dueTime, action) {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.prototype.catch"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>catch (handler)](#apidoc.element.rx.Scheduler.prototype.catch)
- description and source-code
```javascript
catch = function (handler) {
  return new CatchScheduler(this, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.prototype.catchError"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>catchError (handler)](#apidoc.element.rx.Scheduler.prototype.catchError)
- description and source-code
```javascript
catchError = function (handler) {
  return new CatchScheduler(this, handler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.prototype.now"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>now ()](#apidoc.element.rx.Scheduler.prototype.now)
- description and source-code
```javascript
function now() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.prototype.schedule"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>schedule (state, action)](#apidoc.element.rx.Scheduler.prototype.schedule)
- description and source-code
```javascript
schedule = function (state, action) {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.prototype.scheduleFuture"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>scheduleFuture (state, dueTime, action)](#apidoc.element.rx.Scheduler.prototype.scheduleFuture)
- description and source-code
```javascript
scheduleFuture = function (state, dueTime, action) {
  var dt = dueTime;
  dt instanceof Date && (dt = dt - this.now());
  dt = Scheduler.normalize(dt);

  if (dt === 0) { return this.schedule(state, action); }

  return this._scheduleFuture(state, dt, action);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.prototype.schedulePeriodic"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>schedulePeriodic (state, period, action)](#apidoc.element.rx.Scheduler.prototype.schedulePeriodic)
- description and source-code
```javascript
schedulePeriodic = function (state, period, action) {
  if (typeof root.setInterval === 'undefined') { throw new NotSupportedError(); }
  period = normalizeTime(period);
  var s = state, id = root.setInterval(function () { s = action(s); }, period);
  return disposableCreate(function () { root.clearInterval(id); });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.prototype.scheduleRecursive"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>scheduleRecursive (state, action)](#apidoc.element.rx.Scheduler.prototype.scheduleRecursive)
- description and source-code
```javascript
scheduleRecursive = function (state, action) {
  return this.schedule([state, action], invokeRecImmediate);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Scheduler.prototype.scheduleRecursiveFuture"></a>[function <span class="apidocSignatureSpan">rx.Scheduler.prototype.</span>scheduleRecursiveFuture (state, dueTime, action)](#apidoc.element.rx.Scheduler.prototype.scheduleRecursiveFuture)
- description and source-code
```javascript
scheduleRecursiveFuture = function (state, dueTime, action) {
  return this.scheduleFuture([state, action], dueTime, invokeRecDate);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.SerialDisposable"></a>[module rx.SerialDisposable](#apidoc.module.rx.SerialDisposable)

#### <a name="apidoc.element.rx.SerialDisposable.SerialDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>SerialDisposable ()](#apidoc.element.rx.SerialDisposable.SerialDisposable)
- description and source-code
```javascript
SerialDisposable = function () {
  this.isDisposed = false;
  this.current = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.SerialDisposable.prototype"></a>[module rx.SerialDisposable.prototype](#apidoc.module.rx.SerialDisposable.prototype)

#### <a name="apidoc.element.rx.SerialDisposable.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.SerialDisposable.prototype.</span>dispose ()](#apidoc.element.rx.SerialDisposable.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  if (!this.isDisposed) {
    this.isDisposed = true;
    var old = this.current;
    this.current = null;
  }
  old && old.dispose();
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```

#### <a name="apidoc.element.rx.SerialDisposable.prototype.getDisposable"></a>[function <span class="apidocSignatureSpan">rx.SerialDisposable.prototype.</span>getDisposable ()](#apidoc.element.rx.SerialDisposable.prototype.getDisposable)
- description and source-code
```javascript
getDisposable = function () {
  return this.current;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.SerialDisposable.prototype.setDisposable"></a>[function <span class="apidocSignatureSpan">rx.SerialDisposable.prototype.</span>setDisposable (value)](#apidoc.element.rx.SerialDisposable.prototype.setDisposable)
- description and source-code
```javascript
setDisposable = function (value) {
  var shouldDispose = this.isDisposed;
  if (!shouldDispose) {
    var old = this.current;
    this.current = value;
  }
  old && old.dispose();
  shouldDispose && value && value.dispose();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.SingleAssignmentDisposable"></a>[module rx.SingleAssignmentDisposable](#apidoc.module.rx.SingleAssignmentDisposable)

#### <a name="apidoc.element.rx.SingleAssignmentDisposable.SingleAssignmentDisposable"></a>[function <span class="apidocSignatureSpan">rx.</span>SingleAssignmentDisposable ()](#apidoc.element.rx.SingleAssignmentDisposable.SingleAssignmentDisposable)
- description and source-code
```javascript
SingleAssignmentDisposable = function () {
  this.isDisposed = false;
  this.current = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.SingleAssignmentDisposable.prototype"></a>[module rx.SingleAssignmentDisposable.prototype](#apidoc.module.rx.SingleAssignmentDisposable.prototype)

#### <a name="apidoc.element.rx.SingleAssignmentDisposable.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.SingleAssignmentDisposable.prototype.</span>dispose ()](#apidoc.element.rx.SingleAssignmentDisposable.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  if (!this.isDisposed) {
    this.isDisposed = true;
    var old = this.current;
    this.current = null;
    old && old.dispose();
  }
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```

#### <a name="apidoc.element.rx.SingleAssignmentDisposable.prototype.getDisposable"></a>[function <span class="apidocSignatureSpan">rx.SingleAssignmentDisposable.prototype.</span>getDisposable ()](#apidoc.element.rx.SingleAssignmentDisposable.prototype.getDisposable)
- description and source-code
```javascript
getDisposable = function () {
  return this.current;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.SingleAssignmentDisposable.prototype.setDisposable"></a>[function <span class="apidocSignatureSpan">rx.SingleAssignmentDisposable.prototype.</span>setDisposable (value)](#apidoc.element.rx.SingleAssignmentDisposable.prototype.setDisposable)
- description and source-code
```javascript
setDisposable = function (value) {
  if (this.current) { throw new Error('Disposable has already been assigned'); }
  var shouldDispose = this.isDisposed;
  !shouldDispose && (this.current = value);
  shouldDispose && value && value.dispose();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Subject"></a>[module rx.Subject](#apidoc.module.rx.Subject)

#### <a name="apidoc.element.rx.Subject.Subject"></a>[function <span class="apidocSignatureSpan">rx.</span>Subject ()](#apidoc.element.rx.Subject.Subject)
- description and source-code
```javascript
function Subject() {
  __super__.call(this);
  this.isDisposed = false;
  this.isStopped = false;
  this.observers = [];
  this.hasError = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.create"></a>[function <span class="apidocSignatureSpan">rx.Subject.</span>create (observer, observable)](#apidoc.element.rx.Subject.create)
- description and source-code
```javascript
create = function (observer, observable) {
  return new AnonymousSubject(observer, observable);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Subject.prototype"></a>[module rx.Subject.prototype](#apidoc.module.rx.Subject.prototype)

#### <a name="apidoc.element.rx.Subject.prototype._subscribe"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>_subscribe (o)](#apidoc.element.rx.Subject.prototype._subscribe)
- description and source-code
```javascript
_subscribe = function (o) {
  checkDisposed(this);
  if (!this.isStopped) {
    this.observers.push(o);
    return new InnerSubscription(this, o);
  }
  if (this.hasError) {
    o.onError(this.error);
    return disposableEmpty;
  }
  o.onCompleted();
  return disposableEmpty;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.prototype.asObserver"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>asObserver ()](#apidoc.element.rx.Subject.prototype.asObserver)
- description and source-code
```javascript
asObserver = function () {
  var self = this;
  return new AnonymousObserver(
    function (x) { self.onNext(x); },
    function (err) { self.onError(err); },
    function () { self.onCompleted(); });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.prototype.checked"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>checked ()](#apidoc.element.rx.Subject.prototype.checked)
- description and source-code
```javascript
checked = function () { return new CheckedObserver(this); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>constructor ()](#apidoc.element.rx.Subject.prototype.constructor)
- description and source-code
```javascript
function Subject() {
  __super__.call(this);
  this.isDisposed = false;
  this.isStopped = false;
  this.observers = [];
  this.hasError = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>dispose ()](#apidoc.element.rx.Subject.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  this.isDisposed = true;
  this.observers = null;
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```

#### <a name="apidoc.element.rx.Subject.prototype.hasObservers"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>hasObservers ()](#apidoc.element.rx.Subject.prototype.hasObservers)
- description and source-code
```javascript
hasObservers = function () { checkDisposed(this); return this.observers.length > 0; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.prototype.makeSafe"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>makeSafe (disposable)](#apidoc.element.rx.Subject.prototype.makeSafe)
- description and source-code
```javascript
makeSafe = function (disposable) {
  return new AnonymousSafeObserver(this._onNext, this._onError, this._onCompleted, disposable);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.prototype.notifyOn"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>notifyOn (scheduler)](#apidoc.element.rx.Subject.prototype.notifyOn)
- description and source-code
```javascript
notifyOn = function (scheduler) {
  return new ObserveOnObserver(scheduler, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.prototype.onCompleted"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>onCompleted ()](#apidoc.element.rx.Subject.prototype.onCompleted)
- description and source-code
```javascript
onCompleted = function () {
  checkDisposed(this);
  if (!this.isStopped) {
    this.isStopped = true;
    for (var i = 0, os = cloneArray(this.observers), len = os.length; i < len; i++) {
      os[i].onCompleted();
    }

    this.observers.length = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.prototype.onError"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>onError (error)](#apidoc.element.rx.Subject.prototype.onError)
- description and source-code
```javascript
onError = function (error) {
  checkDisposed(this);
  if (!this.isStopped) {
    this.isStopped = true;
    this.error = error;
    this.hasError = true;
    for (var i = 0, os = cloneArray(this.observers), len = os.length; i < len; i++) {
      os[i].onError(error);
    }

    this.observers.length = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.prototype.onNext"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>onNext (value)](#apidoc.element.rx.Subject.prototype.onNext)
- description and source-code
```javascript
onNext = function (value) {
  checkDisposed(this);
  if (!this.isStopped) {
    for (var i = 0, os = cloneArray(this.observers), len = os.length; i < len; i++) {
      os[i].onNext(value);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subject.prototype.toNotifier"></a>[function <span class="apidocSignatureSpan">rx.Subject.prototype.</span>toNotifier ()](#apidoc.element.rx.Subject.prototype.toNotifier)
- description and source-code
```javascript
toNotifier = function () {
  var observer = this;
  return function (n) { return n.accept(observer); };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Subscription"></a>[module rx.Subscription](#apidoc.module.rx.Subscription)

#### <a name="apidoc.element.rx.Subscription.Subscription"></a>[function <span class="apidocSignatureSpan">rx.</span>Subscription (start, end)](#apidoc.element.rx.Subscription.Subscription)
- description and source-code
```javascript
Subscription = function (start, end) {
  this.subscribe = start;
  this.unsubscribe = end || Number.MAX_VALUE;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.Subscription.prototype"></a>[module rx.Subscription.prototype](#apidoc.module.rx.Subscription.prototype)

#### <a name="apidoc.element.rx.Subscription.prototype.equals"></a>[function <span class="apidocSignatureSpan">rx.Subscription.prototype.</span>equals (other)](#apidoc.element.rx.Subscription.prototype.equals)
- description and source-code
```javascript
equals = function (other) {
  return this.subscribe === other.subscribe && this.unsubscribe === other.unsubscribe;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.Subscription.prototype.toString"></a>[function <span class="apidocSignatureSpan">rx.Subscription.prototype.</span>toString ()](#apidoc.element.rx.Subscription.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return '(' + this.subscribe + ', ' + (this.unsubscribe === Number.MAX_VALUE ? 'Infinite' : this.unsubscribe) + ')';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.TestScheduler"></a>[module rx.TestScheduler](#apidoc.module.rx.TestScheduler)

#### <a name="apidoc.element.rx.TestScheduler.TestScheduler"></a>[function <span class="apidocSignatureSpan">rx.</span>TestScheduler ()](#apidoc.element.rx.TestScheduler.TestScheduler)
- description and source-code
```javascript
function TestScheduler() {
  __super__.call(this, 0, baseComparer);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.TestScheduler.prototype"></a>[module rx.TestScheduler.prototype](#apidoc.module.rx.TestScheduler.prototype)

#### <a name="apidoc.element.rx.TestScheduler.prototype.add"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>add (absolute, relative)](#apidoc.element.rx.TestScheduler.prototype.add)
- description and source-code
```javascript
add = function (absolute, relative) {
  return absolute + relative;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>constructor ()](#apidoc.element.rx.TestScheduler.prototype.constructor)
- description and source-code
```javascript
function TestScheduler() {
  __super__.call(this, 0, baseComparer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler.prototype.createColdObservable"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>createColdObservable ()](#apidoc.element.rx.TestScheduler.prototype.createColdObservable)
- description and source-code
```javascript
createColdObservable = function () {
  var len = arguments.length, args;
  if (Array.isArray(arguments[0])) {
    args = arguments[0];
  } else {
    args = new Array(len);
    for (var i = 0; i < len; i++) { args[i] = arguments[i]; }
  }
  return new ColdObservable(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler.prototype.createHotObservable"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>createHotObservable ()](#apidoc.element.rx.TestScheduler.prototype.createHotObservable)
- description and source-code
```javascript
createHotObservable = function () {
  var len = arguments.length, args;
  if (Array.isArray(arguments[0])) {
    args = arguments[0];
  } else {
    args = new Array(len);
    for (var i = 0; i < len; i++) { args[i] = arguments[i]; }
  }
  return new HotObservable(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler.prototype.createObserver"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>createObserver ()](#apidoc.element.rx.TestScheduler.prototype.createObserver)
- description and source-code
```javascript
createObserver = function () {
  return new MockObserver(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler.prototype.createRejectedPromise"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>createRejectedPromise (ticks, reason)](#apidoc.element.rx.TestScheduler.prototype.createRejectedPromise)
- description and source-code
```javascript
createRejectedPromise = function (ticks, reason) {
  return new MockPromise(this, [Rx.ReactiveTest.onError(ticks, reason)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler.prototype.createResolvedPromise"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>createResolvedPromise (ticks, value)](#apidoc.element.rx.TestScheduler.prototype.createResolvedPromise)
- description and source-code
```javascript
createResolvedPromise = function (ticks, value) {
  return new MockPromise(this, [Rx.ReactiveTest.onNext(ticks, value), Rx.ReactiveTest.onCompleted(ticks)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler.prototype.scheduleAbsolute"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>scheduleAbsolute (state, dueTime, action)](#apidoc.element.rx.TestScheduler.prototype.scheduleAbsolute)
- description and source-code
```javascript
scheduleAbsolute = function (state, dueTime, action) {
  dueTime <= this.clock && (dueTime = this.clock + 1);
  return __super__.prototype.scheduleAbsolute.call(this, state, dueTime, action);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler.prototype.startScheduler"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>startScheduler (createFn, settings)](#apidoc.element.rx.TestScheduler.prototype.startScheduler)
- description and source-code
```javascript
startScheduler = function (createFn, settings) {
  settings || (settings = {});
  settings.created == null && (settings.created = ReactiveTest.created);
  settings.subscribed == null && (settings.subscribed = ReactiveTest.subscribed);
  settings.disposed == null && (settings.disposed = ReactiveTest.disposed);

  var observer = this.createObserver(), source, subscription;

  this.scheduleAbsolute(null, settings.created, function () {
    source = createFn();
    return disposableEmpty;
  });

  this.scheduleAbsolute(null, settings.subscribed, function () {
    subscription = source.subscribe(observer);
    return disposableEmpty;
  });

  this.scheduleAbsolute(null, settings.disposed, function () {
    subscription.dispose();
    return disposableEmpty;
  });

  this.start();

  return observer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler.prototype.toAbsoluteTime"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>toAbsoluteTime (absolute)](#apidoc.element.rx.TestScheduler.prototype.toAbsoluteTime)
- description and source-code
```javascript
toAbsoluteTime = function (absolute) {
  return new Date(absolute).getTime();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.TestScheduler.prototype.toRelativeTime"></a>[function <span class="apidocSignatureSpan">rx.TestScheduler.prototype.</span>toRelativeTime (timeSpan)](#apidoc.element.rx.TestScheduler.prototype.toRelativeTime)
- description and source-code
```javascript
toRelativeTime = function (timeSpan) {
  return timeSpan;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.VirtualTimeScheduler"></a>[module rx.VirtualTimeScheduler](#apidoc.module.rx.VirtualTimeScheduler)

#### <a name="apidoc.element.rx.VirtualTimeScheduler.VirtualTimeScheduler"></a>[function <span class="apidocSignatureSpan">rx.</span>VirtualTimeScheduler (initialClock, comparer)](#apidoc.element.rx.VirtualTimeScheduler.VirtualTimeScheduler)
- description and source-code
```javascript
function VirtualTimeScheduler(initialClock, comparer) {
  this.clock = initialClock;
  this.comparer = comparer;
  this.isEnabled = false;
  this.queue = new PriorityQueue(1024);
  __super__.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.VirtualTimeScheduler.prototype"></a>[module rx.VirtualTimeScheduler.prototype](#apidoc.module.rx.VirtualTimeScheduler.prototype)

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.add"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>add ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.add)
- description and source-code
```javascript
add = function () {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.advanceBy"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>advanceBy (time)](#apidoc.element.rx.VirtualTimeScheduler.prototype.advanceBy)
- description and source-code
```javascript
advanceBy = function (time) {
  var dt = this.add(this.clock, time),
      dueToClock = this.comparer(this.clock, dt);
  if (dueToClock > 0) { throw new ArgumentOutOfRangeError(); }
  if (dueToClock === 0) {  return; }

  this.advanceTo(dt);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.advanceTo"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>advanceTo (time)](#apidoc.element.rx.VirtualTimeScheduler.prototype.advanceTo)
- description and source-code
```javascript
advanceTo = function (time) {
  var dueToClock = this.comparer(this.clock, time);
  if (this.comparer(this.clock, time) > 0) { throw new ArgumentOutOfRangeError(); }
  if (dueToClock === 0) { return; }
  if (!this.isEnabled) {
    this.isEnabled = true;
    do {
      var next = this.getNext();
      if (next !== null && this.comparer(next.dueTime, time) <= 0) {
        this.comparer(next.dueTime, this.clock) > 0 && (this.clock = next.dueTime);
        next.invoke();
      } else {
        this.isEnabled = false;
      }
    } while (this.isEnabled);
    this.clock = time;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>constructor (initialClock, comparer)](#apidoc.element.rx.VirtualTimeScheduler.prototype.constructor)
- description and source-code
```javascript
function VirtualTimeScheduler(initialClock, comparer) {
  this.clock = initialClock;
  this.comparer = comparer;
  this.isEnabled = false;
  this.queue = new PriorityQueue(1024);
  __super__.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.getNext"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>getNext ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.getNext)
- description and source-code
```javascript
getNext = function () {
  while (this.queue.length > 0) {
    var next = this.queue.peek();
    if (next.isCancelled()) {
      this.queue.dequeue();
    } else {
      return next;
    }
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.now"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>now ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.now)
- description and source-code
```javascript
now = function () {
  return this.toAbsoluteTime(this.clock);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.schedule"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>schedule (state, action)](#apidoc.element.rx.VirtualTimeScheduler.prototype.schedule)
- description and source-code
```javascript
schedule = function (state, action) {
  return this.scheduleAbsolute(state, this.clock, action);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.scheduleAbsolute"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>scheduleAbsolute (state, dueTime, action)](#apidoc.element.rx.VirtualTimeScheduler.prototype.scheduleAbsolute)
- description and source-code
```javascript
scheduleAbsolute = function (state, dueTime, action) {
  var self = this;

  function run(scheduler, state1) {
    self.queue.remove(si);
    return action(scheduler, state1);
  }

  var si = new ScheduledItem(this, state, run, dueTime, this.comparer);
  this.queue.enqueue(si);

  return si.disposable;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.scheduleFuture"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>scheduleFuture (state, dueTime, action)](#apidoc.element.rx.VirtualTimeScheduler.prototype.scheduleFuture)
- description and source-code
```javascript
scheduleFuture = function (state, dueTime, action) {
  var dt = dueTime instanceof Date ?
    this.toRelativeTime(dueTime - this.now()) :
    this.toRelativeTime(dueTime);

  return this.scheduleRelative(state, dt, action);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.schedulePeriodic"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>schedulePeriodic (state, period, action)](#apidoc.element.rx.VirtualTimeScheduler.prototype.schedulePeriodic)
- description and source-code
```javascript
schedulePeriodic = function (state, period, action) {
  var s = new SchedulePeriodicRecursive(this, state, period, action);
  return s.start();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.scheduleRelative"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>scheduleRelative (state, dueTime, action)](#apidoc.element.rx.VirtualTimeScheduler.prototype.scheduleRelative)
- description and source-code
```javascript
scheduleRelative = function (state, dueTime, action) {
  var runAt = this.add(this.clock, dueTime);
  return this.scheduleAbsolute(state, runAt, action);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.sleep"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>sleep (time)](#apidoc.element.rx.VirtualTimeScheduler.prototype.sleep)
- description and source-code
```javascript
sleep = function (time) {
  var dt = this.add(this.clock, time);
  if (this.comparer(this.clock, dt) >= 0) { throw new ArgumentOutOfRangeError(); }

  this.clock = dt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.start"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>start ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.start)
- description and source-code
```javascript
start = function () {
  if (!this.isEnabled) {
    this.isEnabled = true;
    do {
      var next = this.getNext();
      if (next !== null) {
        this.comparer(next.dueTime, this.clock) > 0 && (this.clock = next.dueTime);
        next.invoke();
      } else {
        this.isEnabled = false;
      }
    } while (this.isEnabled);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.stop"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>stop ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.stop)
- description and source-code
```javascript
stop = function () {
  this.isEnabled = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.toAbsoluteTime"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>toAbsoluteTime ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.toAbsoluteTime)
- description and source-code
```javascript
toAbsoluteTime = function () {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.VirtualTimeScheduler.prototype.toRelativeTime"></a>[function <span class="apidocSignatureSpan">rx.VirtualTimeScheduler.prototype.</span>toRelativeTime ()](#apidoc.element.rx.VirtualTimeScheduler.prototype.toRelativeTime)
- description and source-code
```javascript
toRelativeTime = function () {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.config"></a>[module rx.config](#apidoc.module.rx.config)

#### <a name="apidoc.element.rx.config.Promise"></a>[function <span class="apidocSignatureSpan">rx.config.</span>Promise ()](#apidoc.element.rx.config.Promise)
- description and source-code
```javascript
function Promise() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.helpers"></a>[module rx.helpers](#apidoc.module.rx.helpers)

#### <a name="apidoc.element.rx.helpers.defaultComparer"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>defaultComparer (x, y)](#apidoc.element.rx.helpers.defaultComparer)
- description and source-code
```javascript
defaultComparer = function (x, y) { return isEqual(x, y); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.defaultError"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>defaultError (err)](#apidoc.element.rx.helpers.defaultError)
- description and source-code
```javascript
defaultError = function (err) { throw err; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.defaultKeySerializer"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>defaultKeySerializer (x)](#apidoc.element.rx.helpers.defaultKeySerializer)
- description and source-code
```javascript
defaultKeySerializer = function (x) { return x.toString(); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.defaultNow"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>defaultNow ()](#apidoc.element.rx.helpers.defaultNow)
- description and source-code
```javascript
function now() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.defaultSubComparer"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>defaultSubComparer (x, y)](#apidoc.element.rx.helpers.defaultSubComparer)
- description and source-code
```javascript
defaultSubComparer = function (x, y) { return x > y ? 1 : (x < y ? -1 : 0); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.identity"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>identity (x)](#apidoc.element.rx.helpers.identity)
- description and source-code
```javascript
identity = function (x) { return x; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.isArrayLike"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>isArrayLike (o)](#apidoc.element.rx.helpers.isArrayLike)
- description and source-code
```javascript
isArrayLike = function (o) {
  return o && o.length !== undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.isFunction"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>isFunction (value)](#apidoc.element.rx.helpers.isFunction)
- description and source-code
```javascript
isFunction = function (value) {
  return typeof value == 'function' || false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.isIterable"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>isIterable (o)](#apidoc.element.rx.helpers.isIterable)
- description and source-code
```javascript
isIterable = function (o) {
  return o && o[$iterator$] !== undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.isPromise"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>isPromise (p)](#apidoc.element.rx.helpers.isPromise)
- description and source-code
```javascript
isPromise = function (p) { return !!p && typeof p.subscribe !== 'function' && typeof p.then === 'function'; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.noop"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>noop ()](#apidoc.element.rx.helpers.noop)
- description and source-code
```javascript
noop = function () { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.notImplemented"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>notImplemented ()](#apidoc.element.rx.helpers.notImplemented)
- description and source-code
```javascript
notImplemented = function () {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.helpers.notSupported"></a>[function <span class="apidocSignatureSpan">rx.helpers.</span>notSupported ()](#apidoc.element.rx.helpers.notSupported)
- description and source-code
```javascript
notSupported = function () {
  throw new NotSupportedError();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals"></a>[module rx.internals](#apidoc.module.rx.internals)

#### <a name="apidoc.element.rx.internals.AbstractObserver"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>AbstractObserver ()](#apidoc.element.rx.internals.AbstractObserver)
- description and source-code
```javascript
function AbstractObserver() {
  this.isStopped = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.Enumerable"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>Enumerable ()](#apidoc.element.rx.internals.Enumerable)
- description and source-code
```javascript
Enumerable = function () { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.PriorityQueue"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>PriorityQueue (capacity)](#apidoc.element.rx.internals.PriorityQueue)
- description and source-code
```javascript
PriorityQueue = function (capacity) {
  this.items = new Array(capacity);
  this.length = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.SchedulePeriodicRecursive"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>SchedulePeriodicRecursive (scheduler, state, period, action)](#apidoc.element.rx.internals.SchedulePeriodicRecursive)
- description and source-code
```javascript
function SchedulePeriodicRecursive(scheduler, state, period, action) {
  this._scheduler = scheduler;
  this._state = state;
  this._period = period;
  this._action = action;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledItem"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>ScheduledItem (scheduler, state, action, dueTime, comparer)](#apidoc.element.rx.internals.ScheduledItem)
- description and source-code
```javascript
ScheduledItem = function (scheduler, state, action, dueTime, comparer) {
  this.scheduler = scheduler;
  this.state = state;
  this.action = action;
  this.dueTime = dueTime;
  this.comparer = comparer || defaultSubComparer;
  this.disposable = new SingleAssignmentDisposable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledObserver"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>ScheduledObserver (scheduler, observer)](#apidoc.element.rx.internals.ScheduledObserver)
- description and source-code
```javascript
function ScheduledObserver(scheduler, observer) {
  __super__.call(this);
  this.scheduler = scheduler;
  this.observer = observer;
  this.isAcquired = false;
  this.hasFaulted = false;
  this.queue = [];
  this.disposable = new SerialDisposable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.addProperties"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>addProperties (obj)](#apidoc.element.rx.internals.addProperties)
- description and source-code
```javascript
addProperties = function (obj) {
  for(var sources = [], i = 1, len = arguments.length; i < len; i++) { sources.push(arguments[i]); }
  for (var idx = 0, ln = sources.length; idx < ln; idx++) {
    var source = sources[idx];
    for (var prop in source) {
      obj[prop] = source[prop];
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.addRef"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>addRef (xs, r)](#apidoc.element.rx.internals.addRef)
- description and source-code
```javascript
addRef = function (xs, r) {
  return new AnonymousObservable(function (observer) {
    return new BinaryDisposable(r.getDisposable(), xs.subscribe(observer));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.bindCallback"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>bindCallback (func, thisArg, argCount)](#apidoc.element.rx.internals.bindCallback)
- description and source-code
```javascript
bindCallback = function (func, thisArg, argCount) {
  if (typeof thisArg === 'undefined') { return func; }
  switch(argCount) {
    case 0:
      return function() {
        return func.call(thisArg)
      };
    case 1:
      return function(arg) {
        return func.call(thisArg, arg);
      };
    case 2:
      return function(value, index) {
        return func.call(thisArg, value, index);
      };
    case 3:
      return function(value, index, collection) {
        return func.call(thisArg, value, index, collection);
      };
  }

  return function() {
    return func.apply(thisArg, arguments);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.inherits"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>inherits (child, parent)](#apidoc.element.rx.internals.inherits)
- description and source-code
```javascript
inherits = function (child, parent) {
  function __() { this.constructor = child; }
  __.prototype = parent.prototype;
  child.prototype = new __();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.isEqual"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>isEqual (value, other)](#apidoc.element.rx.internals.isEqual)
- description and source-code
```javascript
isEqual = function (value, other) {
  return baseIsEqual(value, other);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.isObject"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>isObject (value)](#apidoc.element.rx.internals.isObject)
- description and source-code
```javascript
isObject = function (value) {
  var type = typeof value;
  return !!value && (type === 'object' || type === 'function');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.tryCatch"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>tryCatch (fn)](#apidoc.element.rx.internals.tryCatch)
- description and source-code
```javascript
function tryCatch(fn) {
  if (!isFunction(fn)) { throw new TypeError('fn must be a function'); }
  return tryCatcherGen(fn);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.AbstractObserver"></a>[module rx.internals.AbstractObserver](#apidoc.module.rx.internals.AbstractObserver)

#### <a name="apidoc.element.rx.internals.AbstractObserver.AbstractObserver"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>AbstractObserver ()](#apidoc.element.rx.internals.AbstractObserver.AbstractObserver)
- description and source-code
```javascript
function AbstractObserver() {
  this.isStopped = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.AbstractObserver.prototype"></a>[module rx.internals.AbstractObserver.prototype](#apidoc.module.rx.internals.AbstractObserver.prototype)

#### <a name="apidoc.element.rx.internals.AbstractObserver.prototype.completed"></a>[function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>completed ()](#apidoc.element.rx.internals.AbstractObserver.prototype.completed)
- description and source-code
```javascript
completed = function () {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.AbstractObserver.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>constructor ()](#apidoc.element.rx.internals.AbstractObserver.prototype.constructor)
- description and source-code
```javascript
function AbstractObserver() {
  this.isStopped = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.AbstractObserver.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>dispose ()](#apidoc.element.rx.internals.AbstractObserver.prototype.dispose)
- description and source-code
```javascript
dispose = function () { this.isStopped = true; }
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```

#### <a name="apidoc.element.rx.internals.AbstractObserver.prototype.error"></a>[function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>error ()](#apidoc.element.rx.internals.AbstractObserver.prototype.error)
- description and source-code
```javascript
error = function () {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.AbstractObserver.prototype.fail"></a>[function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>fail (e)](#apidoc.element.rx.internals.AbstractObserver.prototype.fail)
- description and source-code
```javascript
fail = function (e) {
  if (!this.isStopped) {
    this.isStopped = true;
    this.error(e);
    return true;
  }

  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.AbstractObserver.prototype.next"></a>[function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>next ()](#apidoc.element.rx.internals.AbstractObserver.prototype.next)
- description and source-code
```javascript
next = function () {
  throw new NotImplementedError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.AbstractObserver.prototype.onCompleted"></a>[function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>onCompleted ()](#apidoc.element.rx.internals.AbstractObserver.prototype.onCompleted)
- description and source-code
```javascript
onCompleted = function () {
  if (!this.isStopped) {
    this.isStopped = true;
    this.completed();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.AbstractObserver.prototype.onError"></a>[function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>onError (error)](#apidoc.element.rx.internals.AbstractObserver.prototype.onError)
- description and source-code
```javascript
onError = function (error) {
  if (!this.isStopped) {
    this.isStopped = true;
    this.error(error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.AbstractObserver.prototype.onNext"></a>[function <span class="apidocSignatureSpan">rx.internals.AbstractObserver.prototype.</span>onNext (value)](#apidoc.element.rx.internals.AbstractObserver.prototype.onNext)
- description and source-code
```javascript
onNext = function (value) {
  !this.isStopped && this.next(value);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.Enumerable"></a>[module rx.internals.Enumerable](#apidoc.module.rx.internals.Enumerable)

#### <a name="apidoc.element.rx.internals.Enumerable.Enumerable"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>Enumerable ()](#apidoc.element.rx.internals.Enumerable.Enumerable)
- description and source-code
```javascript
Enumerable = function () { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.Enumerable.of"></a>[function <span class="apidocSignatureSpan">rx.internals.Enumerable.</span>of (source, selector, thisArg)](#apidoc.element.rx.internals.Enumerable.of)
- description and source-code
```javascript
of = function (source, selector, thisArg) {
  return new OfEnumerable(source, selector, thisArg);
}
```
- example usage
```shell
...
'''js
require({
  'paths': {
    'rx': 'path/to/rx-lite.js'
  }
},
['rx'], (Rx) => {
  const obs = Rx.Observable.of(42);
  obs.forEach(x => console.log(x));
});
'''

## What about my libraries? ##

The Reactive Extensions for JavaScript have no external dependencies on any library, so they'll work well with just about any library
.  We provide bridges and support for various libraries including:
...
```

#### <a name="apidoc.element.rx.internals.Enumerable.repeat"></a>[function <span class="apidocSignatureSpan">rx.internals.Enumerable.</span>repeat (value, repeatCount)](#apidoc.element.rx.internals.Enumerable.repeat)
- description and source-code
```javascript
repeat = function (value, repeatCount) {
  return new RepeatEnumerable(value, repeatCount);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.Enumerable.prototype"></a>[module rx.internals.Enumerable.prototype](#apidoc.module.rx.internals.Enumerable.prototype)

#### <a name="apidoc.element.rx.internals.Enumerable.prototype.catchError"></a>[function <span class="apidocSignatureSpan">rx.internals.Enumerable.prototype.</span>catchError ()](#apidoc.element.rx.internals.Enumerable.prototype.catchError)
- description and source-code
```javascript
catchError = function () {
  return new CatchErrorObservable(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.Enumerable.prototype.concat"></a>[function <span class="apidocSignatureSpan">rx.internals.Enumerable.prototype.</span>concat ()](#apidoc.element.rx.internals.Enumerable.prototype.concat)
- description and source-code
```javascript
concat = function () {
  return new ConcatEnumerableObservable(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.PriorityQueue"></a>[module rx.internals.PriorityQueue](#apidoc.module.rx.internals.PriorityQueue)

#### <a name="apidoc.element.rx.internals.PriorityQueue.PriorityQueue"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>PriorityQueue (capacity)](#apidoc.element.rx.internals.PriorityQueue.PriorityQueue)
- description and source-code
```javascript
PriorityQueue = function (capacity) {
  this.items = new Array(capacity);
  this.length = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.PriorityQueue.prototype"></a>[module rx.internals.PriorityQueue.prototype](#apidoc.module.rx.internals.PriorityQueue.prototype)

#### <a name="apidoc.element.rx.internals.PriorityQueue.prototype.dequeue"></a>[function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>dequeue ()](#apidoc.element.rx.internals.PriorityQueue.prototype.dequeue)
- description and source-code
```javascript
dequeue = function () {
  var result = this.peek();
  this.removeAt(0);
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.PriorityQueue.prototype.enqueue"></a>[function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>enqueue (item)](#apidoc.element.rx.internals.PriorityQueue.prototype.enqueue)
- description and source-code
```javascript
enqueue = function (item) {
  var index = this.length++;
  this.items[index] = new IndexedItem(PriorityQueue.count++, item);
  this.percolate(index);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.PriorityQueue.prototype.heapify"></a>[function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>heapify (index)](#apidoc.element.rx.internals.PriorityQueue.prototype.heapify)
- description and source-code
```javascript
heapify = function (index) {
  +index || (index = 0);
  if (index >= this.length || index < 0) { return; }
  var left = 2 * index + 1,
      right = 2 * index + 2,
      first = index;
  if (left < this.length && this.isHigherPriority(left, first)) {
    first = left;
  }
  if (right < this.length && this.isHigherPriority(right, first)) {
    first = right;
  }
  if (first !== index) {
    var temp = this.items[index];
    this.items[index] = this.items[first];
    this.items[first] = temp;
    this.heapify(first);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.PriorityQueue.prototype.isHigherPriority"></a>[function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>isHigherPriority (left, right)](#apidoc.element.rx.internals.PriorityQueue.prototype.isHigherPriority)
- description and source-code
```javascript
isHigherPriority = function (left, right) {
  return this.items[left].compareTo(this.items[right]) < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.PriorityQueue.prototype.peek"></a>[function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>peek ()](#apidoc.element.rx.internals.PriorityQueue.prototype.peek)
- description and source-code
```javascript
peek = function () { return this.items[0].value; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.PriorityQueue.prototype.percolate"></a>[function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>percolate (index)](#apidoc.element.rx.internals.PriorityQueue.prototype.percolate)
- description and source-code
```javascript
percolate = function (index) {
  if (index >= this.length || index < 0) { return; }
  var parent = index - 1 >> 1;
  if (parent < 0 || parent === index) { return; }
  if (this.isHigherPriority(index, parent)) {
    var temp = this.items[index];
    this.items[index] = this.items[parent];
    this.items[parent] = temp;
    this.percolate(parent);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.PriorityQueue.prototype.remove"></a>[function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>remove (item)](#apidoc.element.rx.internals.PriorityQueue.prototype.remove)
- description and source-code
```javascript
remove = function (item) {
  for (var i = 0; i < this.length; i++) {
    if (this.items[i].value === item) {
      this.removeAt(i);
      return true;
    }
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.PriorityQueue.prototype.removeAt"></a>[function <span class="apidocSignatureSpan">rx.internals.PriorityQueue.prototype.</span>removeAt (index)](#apidoc.element.rx.internals.PriorityQueue.prototype.removeAt)
- description and source-code
```javascript
removeAt = function (index) {
  this.items[index] = this.items[--this.length];
  this.items[this.length] = undefined;
  this.heapify();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.SchedulePeriodicRecursive"></a>[module rx.internals.SchedulePeriodicRecursive](#apidoc.module.rx.internals.SchedulePeriodicRecursive)

#### <a name="apidoc.element.rx.internals.SchedulePeriodicRecursive.SchedulePeriodicRecursive"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>SchedulePeriodicRecursive (scheduler, state, period, action)](#apidoc.element.rx.internals.SchedulePeriodicRecursive.SchedulePeriodicRecursive)
- description and source-code
```javascript
function SchedulePeriodicRecursive(scheduler, state, period, action) {
  this._scheduler = scheduler;
  this._state = state;
  this._period = period;
  this._action = action;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.SchedulePeriodicRecursive.prototype"></a>[module rx.internals.SchedulePeriodicRecursive.prototype](#apidoc.module.rx.internals.SchedulePeriodicRecursive.prototype)

#### <a name="apidoc.element.rx.internals.SchedulePeriodicRecursive.prototype.start"></a>[function <span class="apidocSignatureSpan">rx.internals.SchedulePeriodicRecursive.prototype.</span>start ()](#apidoc.element.rx.internals.SchedulePeriodicRecursive.prototype.start)
- description and source-code
```javascript
start = function () {
  var d = new SingleAssignmentDisposable();
  this._cancel = d;
  d.setDisposable(this._scheduler.scheduleRecursiveFuture(0, this._period, createTick(this)));

  return d;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.ScheduledItem"></a>[module rx.internals.ScheduledItem](#apidoc.module.rx.internals.ScheduledItem)

#### <a name="apidoc.element.rx.internals.ScheduledItem.ScheduledItem"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>ScheduledItem (scheduler, state, action, dueTime, comparer)](#apidoc.element.rx.internals.ScheduledItem.ScheduledItem)
- description and source-code
```javascript
ScheduledItem = function (scheduler, state, action, dueTime, comparer) {
  this.scheduler = scheduler;
  this.state = state;
  this.action = action;
  this.dueTime = dueTime;
  this.comparer = comparer || defaultSubComparer;
  this.disposable = new SingleAssignmentDisposable();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.ScheduledItem.prototype"></a>[module rx.internals.ScheduledItem.prototype](#apidoc.module.rx.internals.ScheduledItem.prototype)

#### <a name="apidoc.element.rx.internals.ScheduledItem.prototype.compareTo"></a>[function <span class="apidocSignatureSpan">rx.internals.ScheduledItem.prototype.</span>compareTo (other)](#apidoc.element.rx.internals.ScheduledItem.prototype.compareTo)
- description and source-code
```javascript
compareTo = function (other) {
  return this.comparer(this.dueTime, other.dueTime);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledItem.prototype.invoke"></a>[function <span class="apidocSignatureSpan">rx.internals.ScheduledItem.prototype.</span>invoke ()](#apidoc.element.rx.internals.ScheduledItem.prototype.invoke)
- description and source-code
```javascript
invoke = function () {
  this.disposable.setDisposable(this.invokeCore());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledItem.prototype.invokeCore"></a>[function <span class="apidocSignatureSpan">rx.internals.ScheduledItem.prototype.</span>invokeCore ()](#apidoc.element.rx.internals.ScheduledItem.prototype.invokeCore)
- description and source-code
```javascript
invokeCore = function () {
  return disposableFixup(this.action(this.scheduler, this.state));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledItem.prototype.isCancelled"></a>[function <span class="apidocSignatureSpan">rx.internals.ScheduledItem.prototype.</span>isCancelled ()](#apidoc.element.rx.internals.ScheduledItem.prototype.isCancelled)
- description and source-code
```javascript
isCancelled = function () {
  return this.disposable.isDisposed;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.ScheduledObserver"></a>[module rx.internals.ScheduledObserver](#apidoc.module.rx.internals.ScheduledObserver)

#### <a name="apidoc.element.rx.internals.ScheduledObserver.ScheduledObserver"></a>[function <span class="apidocSignatureSpan">rx.internals.</span>ScheduledObserver (scheduler, observer)](#apidoc.element.rx.internals.ScheduledObserver.ScheduledObserver)
- description and source-code
```javascript
function ScheduledObserver(scheduler, observer) {
  __super__.call(this);
  this.scheduler = scheduler;
  this.observer = observer;
  this.isAcquired = false;
  this.hasFaulted = false;
  this.queue = [];
  this.disposable = new SerialDisposable();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rx.internals.ScheduledObserver.prototype"></a>[module rx.internals.ScheduledObserver.prototype](#apidoc.module.rx.internals.ScheduledObserver.prototype)

#### <a name="apidoc.element.rx.internals.ScheduledObserver.prototype.completed"></a>[function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>completed ()](#apidoc.element.rx.internals.ScheduledObserver.prototype.completed)
- description and source-code
```javascript
completed = function () {
  this.queue.push(enqueueCompleted(this.observer));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledObserver.prototype.constructor"></a>[function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>constructor (scheduler, observer)](#apidoc.element.rx.internals.ScheduledObserver.prototype.constructor)
- description and source-code
```javascript
function ScheduledObserver(scheduler, observer) {
  __super__.call(this);
  this.scheduler = scheduler;
  this.observer = observer;
  this.isAcquired = false;
  this.hasFaulted = false;
  this.queue = [];
  this.disposable = new SerialDisposable();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledObserver.prototype.dispose"></a>[function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>dispose ()](#apidoc.element.rx.internals.ScheduledObserver.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
  __super__.prototype.dispose.call(this);
  this.disposable.dispose();
}
```
- example usage
```shell
...
  .map(quote => quote.price)
  .subscribe(
    price => console.log('Prices higher than $30: ${price}'),
    err => console.log('Something went wrong: ${err.message}');
  );

/* When we're done */
subscription.dispose();
'''

The only difference is that we can handle the errors inline with our subscription.  And when we're no longer interested in receiving
 the data as it comes streaming in, we call 'dispose' on our subscription.  Note the use of 'subscribe' instead of 'forEach'.  We
 could also use 'forEach' which is an alias for 'subscribe' but we highly suggest you use 'subscribe'.

## Batteries Included ##

Sure, there are a lot of libraries to get started with RxJS. Confused on where to get started?  Start out with the complete set
of operators with ['rx.all.js'](doc/libraries/main/rx.complete.md), then you can reduce it to the number of operators that you really
 need, and perhaps stick with something as small as ['rx.lite.js'](doc/libraries/lite/rx.lite.md).  If you're an implementor of
RxJS, then you can start out with ['rx.core.js'](doc/libraries/core/rx.core.md).
...
```

#### <a name="apidoc.element.rx.internals.ScheduledObserver.prototype.ensureActive"></a>[function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>ensureActive ()](#apidoc.element.rx.internals.ScheduledObserver.prototype.ensureActive)
- description and source-code
```javascript
ensureActive = function () {
  var isOwner = false;
  if (!this.hasFaulted && this.queue.length > 0) {
    isOwner = !this.isAcquired;
    this.isAcquired = true;
  }
  isOwner &&
    this.disposable.setDisposable(this.scheduler.scheduleRecursive(this, scheduleMethod));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledObserver.prototype.error"></a>[function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>error (e)](#apidoc.element.rx.internals.ScheduledObserver.prototype.error)
- description and source-code
```javascript
error = function (e) {
  this.queue.push(enqueueError(this.observer, e));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rx.internals.ScheduledObserver.prototype.next"></a>[function <span class="apidocSignatureSpan">rx.internals.ScheduledObserver.prototype.</span>next (x)](#apidoc.element.rx.internals.ScheduledObserver.prototype.next)
- description and source-code
```javascript
next = function (x) {
  this.queue.push(enqueueNext(this.observer, x));
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
