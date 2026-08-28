# Email Signup and Beta Download

- [x] Inspect the existing landing-page signup flow and identify the Lemon Squeezy integration boundary.
- [x] Replace the placeholder signup handler with a Lemon Squeezy subscriber POST.
- [x] Redirect successful subscribers to the Mythos GitHub Releases page.
- [x] Add accessible loading, success, and failure states without exposing credentials.
- [x] Set `LEMON_SQUEEZY_STORE` in `landing.html` to the store slug from Lemon Squeezy.
- [x] Replace the CORS-blocked AJAX submission with Lemon Squeezy's native HTML form POST.
- [x] Add a direct GitHub Releases link below the beta signup form.
- [ ] Test one real signup in production after setting the store slug.

## Review

- Lemon Squeezy's documented external signup endpoint accepts `email` via POST and stores submissions as Subscribers.
- The redirect is intentionally performed only after a successful response from Lemon Squeezy.
- No Lemon Squeezy API key or secret is needed in the GitHub Pages site.
- The native form POST avoids the cross-origin response-header failure observed on the live endpoint.
