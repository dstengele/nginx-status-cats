# HTTP Status Cats for Nginx

Currently implemented: HTTP 3xx, 4xx and 5xx

## Setup

Clone this Repo somewhere to your web root.
Insert the following snippet into the server block that is going to use the new error pages:

```nginx
# Custom error pages
error_page 300 /error/300.html;
error_page 301 /error/301.html;
error_page 302 /error/302.html;
error_page 303 /error/303.html;
error_page 304 /error/304.html;
error_page 305 /error/305.html;
error_page 307 /error/307.html;
error_page 400 /error/400.html;
error_page 401 /error/401.html;
error_page 403 /error/403.html;
error_page 404 /error/404.html;
error_page 405 /error/405.html;
error_page 406 /error/406.html;
error_page 408 /error/408.html;
error_page 409 /error/409.html;
error_page 410 /error/410.html;
error_page 414 /error/414.html;
error_page 416 /error/416.html;
error_page 417 /error/417.html;
error_page 418 /error/418.html;
error_page 422 /error/422.html;
error_page 423 /error/423.html;
error_page 424 /error/424.html;
error_page 425 /error/425.html;
error_page 426 /error/426.html;
error_page 429 /error/429.html;
error_page 431 /error/431.html;
error_page 444 /error/444.html;
error_page 450 /error/450.html;
error_page 451 /error/451.html;
error_page 500 /error/500.html;
error_page 502 /error/502.html;
error_page 503 /error/503.html;
error_page 506 /error/506.html;
error_page 507 /error/507.html;
error_page 508 /error/508.html;
error_page 509 /error/509.html;
error_page 599 /error/599.html;


location ^~ /error/ {
›   root /srv/http/nginx-status-cats;
}
```

You're done!
