# Plack::App::Proxy::HTTP::Tiny

[![CI](https://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny/actions/workflows/ci.yaml/badge.svg)](https://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny/actions/workflows/ci.yaml)
[![Trunk Check](https://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny/actions/workflows/trunk.yaml/badge.svg)](https://github.com/dex4er/perl-Plack-App-Proxy-Backend-HTTP-Tiny/actions/workflows/trunk.yaml)
[![CPAN](https://img.shields.io/cpan/v/Plack-App-Proxy-Backend-HTTP-Tiny)](https://metacpan.org/dist/Plack-App-Proxy-Backend-HTTP-Tiny)

## NAME

Plack::App::Proxy::HTTP::Tiny - backend for Plack::App::Proxy

## SYNOPSIS

```perl

    # In app.psgi
    use Plack::Builder;
    use Plack::App::Proxy::Anonymous;

    builder {
        enable "Proxy::Requests";
        Plack::App::Proxy->new(backend => 'HTTP::Tiny')->to_app;
    };

```

## DESCRIPTION

This backend uses [HTTP::Tiny::PreserveHostHeader](https://metacpan.org/pod/HTTP%3A%3ATiny%3A%3APreserveHostHeader) to make HTTP requests.

[HTTP::Tiny::PreserveHostHeader](https://metacpan.org/pod/HTTP%3A%3ATiny%3A%3APreserveHostHeader) is a wrapper for [HTTP::Tiny](https://metacpan.org/pod/HTTP%3A%3ATiny) which is
Pure-Perl only and doesn't require any architecture specific files.

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
