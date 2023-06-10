[![Build Status](https://travis-ci.org/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny.svg?branch=master)](https://travis-ci.org/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny)[![CPAN version](https://badge.fury.io/pl/Plack-App-Proxy-Backend-HTTP-Tiny.svg)](https://metacpan.org/release/Plack-App-Proxy-Backend-HTTP-Tiny)

# NAME

Plack::App::Proxy::HTTP::Tiny - backend for Plack::App::Proxy

# SYNOPSIS

    # In app.psgi
    use Plack::Builder;
    use Plack::App::Proxy::Anonymous;

    builder {
        enable "Proxy::Requests";
        Plack::App::Proxy->new(backend => 'HTTP::Tiny')->to_app;
    };

# DESCRIPTION

This backend uses [HTTP::Tiny](https://metacpan.org/pod/HTTP::Tiny) to make HTTP requests.

[HTTP::Tiny](https://metacpan.org/pod/HTTP::Tiny) backend is Pure-Perl only and doesn't require any
architecture specific files.

It is possible to bundle it e.g. by [App::FatPacker](https://metacpan.org/pod/App::FatPacker).

# SEE ALSO

[Plack](https://metacpan.org/pod/Plack), [Plack::App::Proxy](https://metacpan.org/pod/Plack::App::Proxy), [Plack::Middleware::Proxy::Requests](https://metacpan.org/pod/Plack::Middleware::Proxy::Requests),
[HTTP::Tiny](https://metacpan.org/pod/HTTP::Tiny).

# BUGS

This module might be incompatible with further versions of
[Plack::App::Proxy](https://metacpan.org/pod/Plack::App::Proxy) module.

If you find the bug or want to implement new features, please report it at
[https://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny/issues](https://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny/issues)

The code repository is available at
[http://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny](http://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny)

# AUTHOR

Piotr Roszatycki <dexter@cpan.org>

# LICENSE

Copyright (c) 2014-2016, 2023 Piotr Roszatycki <dexter@cpan.org>.

This is free software; you can redistribute it and/or modify it under
the same terms as perl itself.

See [http://dev.perl.org/licenses/artistic.html](http://dev.perl.org/licenses/artistic.html)
## NAME

Plack::App::Proxy::HTTP::Tiny - backend for Plack::App::Proxy

## SYNOPSIS

    # In app.psgi
    use Plack::Builder;
    use Plack::App::Proxy::Anonymous;

    builder {
        enable "Proxy::Requests";
        Plack::App::Proxy->new(backend => 'HTTP::Tiny')->to_app;
    };

## DESCRIPTION

This backend uses [HTTP::Tiny](https://metacpan.org/pod/HTTP%3A%3ATiny) to make HTTP requests.

[HTTP::Tiny](https://metacpan.org/pod/HTTP%3A%3ATiny) backend is Pure-Perl only and doesn't require any
architecture specific files.

It is possible to bundle it e.g. by [App::FatPacker](https://metacpan.org/pod/App%3A%3AFatPacker).

## SEE ALSO

[Plack](https://metacpan.org/pod/Plack), [Plack::App::Proxy](https://metacpan.org/pod/Plack%3A%3AApp%3A%3AProxy), [Plack::Middleware::Proxy::Requests](https://metacpan.org/pod/Plack%3A%3AMiddleware%3A%3AProxy%3A%3ARequests),
[HTTP::Tiny](https://metacpan.org/pod/HTTP%3A%3ATiny).

## BUGS

This module might be incompatible with further versions of
[Plack::App::Proxy](https://metacpan.org/pod/Plack%3A%3AApp%3A%3AProxy) module.

If you find the bug or want to implement new features, please report it at
[https://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny/issues](https://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny/issues)

The code repository is available at
[http://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny](http://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny)

## AUTHOR

Piotr Roszatycki <dexter@cpan.org>

## LICENSE

Copyright (c) 2014-2016, 2023 Piotr Roszatycki <dexter@cpan.org>.

This is free software; you can redistribute it and/or modify it under
the same terms as perl itself.

See [http://dev.perl.org/licenses/artistic.html](http://dev.perl.org/licenses/artistic.html)
