# Third-Party Notices

This project includes or depends on third-party software and services. The following notices are provided for transparency and compliance. You are responsible for ensuring your distribution and deployment comply with all applicable licenses and terms.

---

## FFmpeg
This project’s Docker image installs **FFmpeg** for media processing (e.g., audio extraction, probing, transcoding).

- FFmpeg is typically licensed under the **LGPL 2.1+** or **GPL 2+** depending on build configuration and enabled components.
- Some distributions enable GPL components by default, which may impose additional requirements if you redistribute binaries/containers.

You should review your FFmpeg build configuration and comply with FFmpeg’s licensing requirements.
FFmpeg project: https://ffmpeg.org/

---

## OpenAI API / ChatGPT
This project may integrate with OpenAI’s API (Responses API) for assistive analysis and report drafting.

Use of OpenAI services is governed by OpenAI’s applicable terms and policies.
OpenAI documentation: https://platform.openai.com/docs/

**Important:** AI outputs are not evidence by themselves; they must be validated against primary artifacts.

---

## Python Dependencies (PyPI)
This project depends on Python packages, typically installed from PyPI. Key dependencies include:

- FastAPI — https://fastapi.tiangolo.com/
- Uvicorn — https://www.uvicorn.org/
- APScheduler — https://apscheduler.readthedocs.io/
- ReportLab — https://www.reportlab.com/
- Requests — https://requests.readthedocs.io/
- NumPy — https://numpy.org/
- python-multipart — https://andrew-d.github.io/python-multipart/

Each dependency is licensed under its own license (commonly MIT/BSD/Apache-2.0). You should review license texts for all dependencies in your final build (e.g., `pip freeze` + `pip-licenses` output) and include them as required by your distribution method.

---

## GitHub Actions
If you enable the included GitHub Actions workflow, usage is subject to GitHub’s terms and platform policies.
GitHub Actions: https://docs.github.com/actions

---

## Trademarks
“OpenAI” and “ChatGPT” are trademarks of their respective owners. This project is not affiliated with or endorsed by OpenAI unless explicitly stated.

---

## Additional Notices
If you add plugins, detectors, models, or external services, you must update this file with:
- Name
- Purpose
- Source URL
- License/terms
- Any required attribution text
