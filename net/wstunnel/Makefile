PORTNAME=	wstunnel
DISTVERSIONPREFIX=	v
DISTVERSION=	10.1.5
CATEGORIES=	net

MAINTAINER=	yuri@FreeBSD.org
COMMENT=	Traffic tunnel over Websocket or HTTP2 to bypass firewalls/DPI
WWW=		https://github.com/erebe/wstunnel

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		cargo

USE_GITHUB=	yes
GH_ACCOUNT=	erebe

RUSTFLAGS=	${ARCH:S/i386/YES/:C/^[a-z].*//:S/YES/-C target-feature=+sse,+sse2/} # add sse sse2 target-features only on i386

CARGO_CRATES=	addr2line-0.24.2 \
		adler2-2.0.0 \
		ahash-0.8.11 \
		aho-corasick-1.1.3 \
		android-tzdata-0.1.1 \
		android_system_properties-0.1.5 \
		anstream-0.6.15 \
		anstyle-1.0.8 \
		anstyle-parse-0.2.5 \
		anstyle-query-1.1.1 \
		anstyle-wincon-3.0.4 \
		anyhow-1.0.89 \
		arc-swap-1.7.1 \
		asn1-rs-0.6.2 \
		asn1-rs-derive-0.5.1 \
		asn1-rs-impl-0.2.0 \
		async-channel-2.3.1 \
		async-trait-0.1.83 \
		atomic-waker-1.1.2 \
		autocfg-1.4.0 \
		aws-lc-rs-1.10.0 \
		aws-lc-sys-0.22.0 \
		backtrace-0.3.74 \
		base64-0.21.7 \
		base64-0.22.1 \
		bb8-0.8.5 \
		bindgen-0.69.5 \
		bitflags-1.3.2 \
		bitflags-2.6.0 \
		block-buffer-0.10.4 \
		bollard-0.17.1 \
		bollard-stubs-1.45.0-rc.26.0.1 \
		bumpalo-3.16.0 \
		byteorder-1.5.0 \
		bytes-1.7.2 \
		cc-1.1.30 \
		cexpr-0.6.0 \
		cfg-if-1.0.0 \
		cfg_aliases-0.2.1 \
		chrono-0.4.38 \
		clang-sys-1.8.1 \
		clap-4.5.20 \
		clap_builder-4.5.20 \
		clap_derive-4.5.18 \
		clap_lex-0.7.2 \
		cmake-0.1.51 \
		colorchoice-1.0.2 \
		concurrent-queue-2.5.0 \
		core-foundation-0.9.4 \
		core-foundation-sys-0.8.7 \
		cpufeatures-0.2.14 \
		crossbeam-channel-0.5.13 \
		crossbeam-utils-0.8.20 \
		crossterm-0.28.1 \
		crossterm_winapi-0.9.1 \
		crypto-common-0.1.6 \
		darling-0.20.10 \
		darling_core-0.20.10 \
		darling_macro-0.20.10 \
		data-encoding-2.6.0 \
		der-parser-9.0.0 \
		deranged-0.3.11 \
		digest-0.10.7 \
		displaydoc-0.2.5 \
		docker_credential-1.3.1 \
		dunce-1.0.5 \
		either-1.13.0 \
		enum-as-inner-0.6.1 \
		equivalent-1.0.1 \
		errno-0.3.9 \
		etcetera-0.8.0 \
		event-listener-5.3.1 \
		event-listener-strategy-0.5.2 \
		fast-socks5-0.9.6 \
		filetime-0.2.25 \
		fnv-1.0.7 \
		form_urlencoded-1.2.1 \
		fs_extra-1.3.0 \
		fsevent-sys-4.1.0 \
		futures-0.3.31 \
		futures-channel-0.3.31 \
		futures-core-0.3.31 \
		futures-executor-0.3.31 \
		futures-io-0.3.31 \
		futures-macro-0.3.31 \
		futures-sink-0.3.31 \
		futures-task-0.3.31 \
		futures-util-0.3.31 \
		generic-array-0.14.7 \
		getrandom-0.2.15 \
		gimli-0.31.1 \
		glob-0.3.1 \
		h2-0.3.26 \
		h2-0.4.6 \
		hashbrown-0.12.3 \
		hashbrown-0.15.0 \
		heck-0.5.0 \
		hermit-abi-0.3.9 \
		hex-0.4.3 \
		hickory-proto-0.24.1 \
		hickory-resolver-0.24.1 \
		home-0.5.9 \
		hostname-0.3.1 \
		http-0.2.12 \
		http-1.1.0 \
		http-body-1.0.1 \
		http-body-util-0.1.2 \
		httparse-1.9.5 \
		httpdate-1.0.3 \
		hyper-1.4.1 \
		hyper-named-pipe-0.1.0 \
		hyper-rustls-0.27.3 \
		hyper-util-0.1.9 \
		hyperlocal-0.9.1 \
		iana-time-zone-0.1.61 \
		iana-time-zone-haiku-0.1.2 \
		ident_case-1.0.1 \
		idna-0.4.0 \
		idna-0.5.0 \
		indexmap-1.9.3 \
		indexmap-2.6.0 \
		inotify-0.9.6 \
		inotify-sys-0.1.5 \
		ipconfig-0.3.2 \
		ipnet-2.10.1 \
		is_terminal_polyfill-1.70.1 \
		itertools-0.12.1 \
		itoa-1.0.11 \
		jobserver-0.1.32 \
		js-sys-0.3.72 \
		jsonwebtoken-9.3.0 \
		kqueue-1.0.8 \
		kqueue-sys-1.0.4 \
		lazy_static-1.5.0 \
		lazycell-1.3.0 \
		libc-0.2.159 \
		libloading-0.8.5 \
		libredox-0.1.3 \
		linked-hash-map-0.5.6 \
		linux-raw-sys-0.4.14 \
		lock_api-0.4.12 \
		log-0.4.22 \
		lru-cache-0.1.2 \
		match_cfg-0.1.0 \
		matchers-0.1.0 \
		memchr-2.7.4 \
		memoffset-0.9.1 \
		minimal-lexical-0.2.1 \
		miniz_oxide-0.8.0 \
		mio-0.8.11 \
		mio-1.0.2 \
		mirai-annotations-1.12.0 \
		nix-0.29.0 \
		nom-7.1.3 \
		notify-6.1.1 \
		nu-ansi-term-0.46.0 \
		num-bigint-0.4.6 \
		num-conv-0.1.0 \
		num-integer-0.1.46 \
		num-traits-0.2.19 \
		num_threads-0.1.7 \
		object-0.36.5 \
		oid-registry-0.7.1 \
		once_cell-1.20.2 \
		openssl-probe-0.1.5 \
		overload-0.1.1 \
		parking-2.2.1 \
		parking_lot-0.12.3 \
		parking_lot_core-0.9.10 \
		parse-display-0.9.1 \
		parse-display-derive-0.9.1 \
		paste-1.0.15 \
		percent-encoding-2.3.1 \
		pin-project-1.1.6 \
		pin-project-internal-1.1.6 \
		pin-project-lite-0.2.14 \
		pin-utils-0.1.0 \
		powerfmt-0.2.0 \
		ppp-2.2.0 \
		ppv-lite86-0.2.20 \
		prettyplease-0.2.22 \
		proc-macro2-1.0.87 \
		quick-error-1.2.3 \
		quote-1.0.37 \
		rand-0.8.5 \
		rand_chacha-0.3.1 \
		rand_core-0.6.4 \
		rcgen-0.13.1 \
		redox_syscall-0.3.5 \
		redox_syscall-0.5.7 \
		regex-1.11.0 \
		regex-automata-0.1.10 \
		regex-automata-0.4.8 \
		regex-syntax-0.6.29 \
		regex-syntax-0.8.5 \
		resolv-conf-0.7.0 \
		ring-0.17.8 \
		rustc-demangle-0.1.24 \
		rustc-hash-1.1.0 \
		rusticata-macros-4.1.0 \
		rustix-0.38.37 \
		rustls-0.21.12 \
		rustls-0.23.14 \
		rustls-native-certs-0.6.3 \
		rustls-native-certs-0.7.3 \
		rustls-native-certs-0.8.0 \
		rustls-pemfile-1.0.4 \
		rustls-pemfile-2.2.0 \
		rustls-pki-types-1.9.0 \
		rustls-webpki-0.101.7 \
		rustls-webpki-0.102.8 \
		ryu-1.0.18 \
		same-file-1.0.6 \
		schannel-0.1.26 \
		scopeguard-1.2.0 \
		sct-0.7.1 \
		security-framework-2.11.1 \
		security-framework-sys-2.12.0 \
		serde-1.0.210 \
		serde_derive-1.0.210 \
		serde_json-1.0.128 \
		serde_regex-1.1.0 \
		serde_repr-0.1.19 \
		serde_urlencoded-0.7.1 \
		serde_with-3.11.0 \
		serde_with_macros-3.11.0 \
		serde_yaml-0.9.34+deprecated \
		sha1-0.10.6 \
		sharded-slab-0.1.7 \
		shlex-1.3.0 \
		signal-hook-0.3.17 \
		signal-hook-mio-0.2.4 \
		signal-hook-registry-1.4.2 \
		simdutf8-0.1.5 \
		slab-0.4.9 \
		smallvec-1.13.2 \
		socket2-0.5.7 \
		spin-0.9.8 \
		strsim-0.11.1 \
		structmeta-0.3.0 \
		structmeta-derive-0.3.0 \
		subtle-2.6.1 \
		syn-2.0.79 \
		synstructure-0.13.1 \
		testcontainers-0.23.1 \
		thiserror-1.0.64 \
		thiserror-impl-1.0.64 \
		thread_local-1.1.8 \
		time-0.3.36 \
		time-core-0.1.2 \
		time-macros-0.2.18 \
		tinyvec-1.8.0 \
		tinyvec_macros-0.1.1 \
		tokio-1.40.0 \
		tokio-fd-0.3.0 \
		tokio-macros-2.4.0 \
		tokio-rustls-0.24.1 \
		tokio-rustls-0.26.0 \
		tokio-stream-0.1.16 \
		tokio-tar-0.3.1 \
		tokio-util-0.7.12 \
		tower-service-0.3.3 \
		tracing-0.1.40 \
		tracing-attributes-0.1.27 \
		tracing-core-0.1.32 \
		tracing-log-0.2.0 \
		tracing-subscriber-0.3.18 \
		try-lock-0.2.5 \
		typenum-1.17.0 \
		unicode-bidi-0.3.17 \
		unicode-ident-1.0.13 \
		unicode-normalization-0.1.24 \
		unsafe-libyaml-0.2.11 \
		untrusted-0.7.1 \
		untrusted-0.9.0 \
		url-2.5.2 \
		urlencoding-2.1.3 \
		utf-8-0.7.6 \
		utf8parse-0.2.2 \
		uuid-1.10.0 \
		valuable-0.1.0 \
		version_check-0.9.5 \
		walkdir-2.5.0 \
		want-0.3.1 \
		wasi-0.11.0+wasi-snapshot-preview1 \
		wasm-bindgen-0.2.95 \
		wasm-bindgen-backend-0.2.95 \
		wasm-bindgen-macro-0.2.95 \
		wasm-bindgen-macro-support-0.2.95 \
		wasm-bindgen-shared-0.2.95 \
		which-4.4.2 \
		widestring-1.1.0 \
		winapi-0.3.9 \
		winapi-i686-pc-windows-gnu-0.4.0 \
		winapi-util-0.1.9 \
		winapi-x86_64-pc-windows-gnu-0.4.0 \
		windows-core-0.52.0 \
		windows-sys-0.48.0 \
		windows-sys-0.52.0 \
		windows-sys-0.59.0 \
		windows-targets-0.48.5 \
		windows-targets-0.52.6 \
		windows_aarch64_gnullvm-0.48.5 \
		windows_aarch64_gnullvm-0.52.6 \
		windows_aarch64_msvc-0.48.5 \
		windows_aarch64_msvc-0.52.6 \
		windows_i686_gnu-0.48.5 \
		windows_i686_gnu-0.52.6 \
		windows_i686_gnullvm-0.52.6 \
		windows_i686_msvc-0.48.5 \
		windows_i686_msvc-0.52.6 \
		windows_x86_64_gnu-0.48.5 \
		windows_x86_64_gnu-0.52.6 \
		windows_x86_64_gnullvm-0.48.5 \
		windows_x86_64_gnullvm-0.52.6 \
		windows_x86_64_msvc-0.48.5 \
		windows_x86_64_msvc-0.52.6 \
		winreg-0.50.0 \
		x509-parser-0.16.0 \
		xattr-1.3.1 \
		yasna-0.5.2 \
		zerocopy-0.7.35 \
		zerocopy-derive-0.7.35 \
		zeroize-1.8.1 \
		fastwebsockets@git+https://github.com/erebe/fastwebsockets.git\#ef904598ec168d7748b28d77ec1803ba721932d8

PLIST_FILES=	bin/${PORTNAME}

.include <bsd.port.mk>
