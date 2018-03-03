# ppusespringng2webapp
### Routing
Router Events
- NavigationStart  when navigation starts
- RoutesRegognized when the routes are recognized
- RouteConfigLoadStart after/before a route has been loaded, depends from the lazy loaded config
- NavigationEnd when navigatoin ends successfully
- NavigationCancel - When navigation is calcelled
- NavagationError

Route Guards
- CanActivate
- CanActivateChild
- CanDeactivate ->get invoked before navigating away from the current route
- Resolve -> performs route data retrival before route activation
- CanLoad -> check if an async load module is available

```
ng new app --routing


### Observable
Subject
- Subject is a special type of Observable that multicast values to many Observers and can subscribe to other observables

```
import {Observable} from 'rxjs/Observable';
import {Subject} from 'rxjs/Subject';
const observableOne = new Observable(observer=>{observer.next(Math.random());
observableOne.subscribe(value=>console.log('',value));

const observableTwo = new Observable(observer=>{observer.next(Math.random());
const subject = new Subject();
subject.subscribe(value=>console.log(value));
subject.next("xx")
observableTwo.subscribe(subject);
```

