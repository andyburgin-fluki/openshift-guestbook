# openshift-guestbook

Add urls to route/ingress in:

  ./deployment/guestbook-frontend-ingress.yaml:  - host: gbingress.apps.xxxxx.clusters.xxxxxxxxxx.tld
  ./deployment/guestbook-frontend-route.yaml:  host: gbroute.apps.xxxxx.clusters.xxxxxxxxxx.tld
  ./scaling/script.js:  http.get('http://gbroute.apps.xxxxx.clusters.xxxxxxxxxx.tld/');


deploy in order - deployment, network_policies, monitoring, storage, scaling
