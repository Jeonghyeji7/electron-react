# 실행
    "react-start": "react-scripts start",

    "react-build": "react-scripts build",

    "test": "react-scripts test",

    "eject": "react-scripts eject",

    "start": "concurrently \"cross-env NODE_ENV=development BROWSER=none npm run react-start\" \"wait-on http://localhost:3000 && electron .\"",

    "build": "npm run react-build && electron-builder",

    "release": "npm run react-build && electron-builder --publish=always"