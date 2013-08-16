//
// When you need to access an API service using $http via CORS, the preflight OPTION
// will be call every time you make a request. The idea is enable Angularjs to send its
// requests with the appropriate CORS headers globally for the whole app.
//

var myApps = angular.module('myApps', [ 'myServices' ]);

myApps
  .config( function ($routeProvider, $httpProvider) {

    $httpProvider.defaults.useXDomain = true;
    delete $httpProvider.defaults.headers.common['X-Requested-With'];

    $routeProvider
      .when(.....);

  });