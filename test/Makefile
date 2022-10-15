.POSIX:
.PHONY: *

filter = .

default: smoke contract integration e2e


smoke contract integration e2e:
	gotestsum --format testname -- -timeout 30m ./$@ -run "${filter}"
