Why a Cloud Is Perfect for Interactive Dashboards
=================================================

**Slide 2 — about 100 seconds.**

- A Dash app is a **long-running web process** — it needs a machine that stays
  on and answers browsers
- One VM per person: ``pip install dash`` → ``dash run --port 8050`` → share
  the URL
- Public IP (or a free DNS name, e.g.
  ``name.ALLOCATION.projects.jetstream-cloud.org``) — anyone can open your
  dashboard in a browser
- Security groups control *who* can reach your dashboard's port
- Production polish when you're ready: automatic HTTPS (Caddy + Let's
  Encrypt) and your own domain via a CNAME record
- Block and S3-compatible object storage for datasets; shelve the VM when idle
  to save credits

.. note:: Speaker notes (~100 s)

   "Here's why this workshop happens on a cloud and not on your laptop. A
   Plotly Dash app is a *live web application*: it's a process that runs
   continuously and talks back and forth with every browser that touches it —
   sliders, callbacks, filters. That means it needs three things: a machine
   that stays on, a network address the internet can reach, and a place to put
   your data. Jetstream2 gives you all three in about two minutes. You launch a
   virtual machine, SSH in, install Dash, run your app on port 8050 — and you
   now have a URL that any collaborator, anywhere, can open in a browser. That's
   the whole trick: your analysis goes from a static PDF figure to something a
   co-author can actually *poke at*. You control access with security groups —
   open the port to your lab, or to the world. If a dashboard graduates into a
   real service later, you can put automatic HTTPS in front of it and point
   your own domain at it. Your data lives on block storage or in S3-compatible
   object storage, and when you're done for the day you can shelve the machine
   — shelved VMs cost nothing, so your allocation stretches further."
