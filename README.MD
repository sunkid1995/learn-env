# Set ENV NodeJS with cross-env
## step 1
* npm install cross-env or yarn add cross-env.  
## step 2
1. ở cửa sổ dòng lệnh ta có thể chạy. 
 * npx cross-env NODE_ENV=development || production PORT=3000 TEST=SAYHI node server.js
2. ở cửa sổ dòng lệnh ta có thể chạy
 * NODE_ENV=development PORT=3000 TEST=SAYHI node server.js
3. ở trong scripts của package tạo thêm 2 scrip -> start:dev - start:prd.
 * yarn run start:dev - start:prd
4. chạy với eval và cat file.
 * tạo file .env, etc
 * ở trong scripts của package tạo thêm scrip -> eval
 * yarn eval
5. dùng export
 * ở trong commandline
      - export NODE_ENV=development PORT=3000
      - node server.js
 * export và cat file
      - tạo file .env, etc
      - export cat $(cat .env) && node server.js
