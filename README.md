# its-just-between-us.com

Static marketing site for the Between Us iOS app (betweenus-ios / betweenus-api, in ~/betweenus).
Plain HTML + one stylesheet, no build step. Hosted on GitHub Pages; `CNAME` pins
the custom domain.

- `index.html` — landing page
- `privacy.html` — privacy policy (App Store Connect "Privacy Policy URL").
  Text must match betweenus-api `app/static/privacy.html` and betweenus-ios
  `Sources/PrivacyPolicyView.swift` word for word.
- `support.html` — support page (App Store Connect "Support URL")
- `styles.css` — palette mirrors betweenus-ios `Sources/Theme.swift`

Preview locally: `python3 -m http.server 8080` then open http://localhost:8080

The hero links to the App Store listing (id6820863760, "Just Between Us"), and an
`apple-itunes-app` meta tag shows Safari's "Open in App Store" banner on iPhone.
