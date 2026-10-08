# MedConnect frontend

A Next.js/TypeScript frontend for patient appointments and medical-analysis uploads. The application includes doctor/time selection, appointment details, patient account views, and analysis pages.

This repository is a fork of [the upstream MedConnect project](https://github.com/LucaStefan112/MedConnect). Upstream history and contributor attribution remain part of the project; hosting this fork does not imply sole authorship.

The companion API is [MedConnect-Server](https://github.com/omerdikyol/MedConnect-Server).

## Run locally

```sh
git clone https://github.com/omerdikyol/MedConnect.git
cd MedConnect
npm install
npm run dev
```

The development script uses [localhost:3003](http://localhost:3003). Configure the backend address using the existing `SERVER` configuration in [next.config.js](next.config.js) and [the service layer](services/app.service.ts). The appointment and analysis flows require the companion backend; the frontend alone is not a complete demo.

## Code map

- [Appointment pages](pages/appointments): scheduling and appointment detail views.
- [Analysis pages](pages/analyses): medical-analysis lists and detail views.
- [Scheduler](components/Scheduler/Scheduler.tsx): time-selection UI.
- [Services](services): API calls and response types.

## Development

```sh
npm run build
npm run lint
```

Use synthetic patient details and documents when exploring the application.
