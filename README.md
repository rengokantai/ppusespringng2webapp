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
