# its-just-between-us.com

Static marketing site for the Just Between Us iOS app (couples-ios / couples-api).
Plain HTML + one stylesheet, no build step. Hosted on GitHub Pages; `CNAME` pins
the custom domain.

- `index.html` — landing page
- `privacy.html` — privacy policy (App Store Connect "Privacy Policy URL").
  Text must match couples-api `app/static/privacy.html` and couples-ios
  `Sources/PrivacyPolicyView.swift` word for word.
- `support.html` — support page (App Store Connect "Support URL")
- `styles.css` — palette mirrors couples-ios `Sources/Theme.swift`

Preview locally: `python3 -m http.server 8080` then open http://localhost:8080

When the app is live, replace the "Coming soon" badge in `index.html` with the
App Store link (there's a commented-out line ready).
