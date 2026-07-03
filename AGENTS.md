Comprehensive tests for open-link-confirmation -- a sanitization contract, a Qt
rich-text differential, and a static display-pipeline audit -- are too
high-volume for human review and live in the AI-maintained dist-ai repo, not
here:

  https://github.com/org-ai-assisted/dist-ai -> usr/share/open-link-confirmation-tests/

Run them against this checkout (sanitize-string is supplied by helper-scripts):

    OPEN_LINK_CONFIRMATION_BIN="$PWD/usr/libexec/open-link-confirmation/open-link-confirmation" \
      open-link-confirmation-tests
