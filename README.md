# dome_voice_msgs

Message-only package for DOME speech.

- `msg/Announcement.msg`: what goes on `/announcement`. `dome_voice`'s
  `speech_output` speaks `text`; `priority` uses the `PRIORITY_*` constants
  (0 = safety ... 5 = chitchat).

It used to live in `dome_control` (`dome_control/msg/Announcement`). It moved
here (dome_nav F38) so that dome_nav can publish announcements without
depending on dome_control.
