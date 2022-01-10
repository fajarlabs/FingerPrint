# FingerPrint web App
## FingerPrint Enrolment and Verification web App using U.are.U 4500 FingerPrint Scanner and SDK v3 in PHP

#### SDK v3 [Download](https://drive.google.com/open?id=1Hg3HAqwLuqmi9F4eUAgb5WaeLyJvPQq5)  
#### SDKPatch [Download](https://drive.google.com/file/d/1yB0oW3NtBfCBKFHSe0Blc7B7grMD854W/view?usp=sharing)

## How to instalasi dll using gacutil.exe
https://stackoverflow.com/questions/40434572/where-is-gacutil-exe-in-windows-10<br />

```
> gacutil.exe /i DPUruNet.dll
> gacutil.exe /i DPXUru.dll
> gacutil.exe /i MyBase64.dll
> gacutil.exe /i MyFPLib.dll
```

## Use PHP 7

## SQL Script

```
/*
 Navicat Premium Data Transfer

 Source Server         : fingerprint
 Source Server Type    : MySQL
 Source Server Version : 100138
 Source Host           : localhost:3306
 Source Schema         : fingerprint

 Target Server Type    : MySQL
 Target Server Version : 100138
 File Encoding         : 65001

 Date: 10/01/2022 16:50:13
*/

SET NAMES utf8mb4;
SET FOREIGN_KEY_CHECKS = 0;

-- ----------------------------
-- Table structure for users
-- ----------------------------
DROP TABLE IF EXISTS `users`;
CREATE TABLE `users`  (
  `id` int(11) NOT NULL,
  `indexfinger` text CHARACTER SET latin1 COLLATE latin1_swedish_ci NULL,
  `middlefinger` text CHARACTER SET latin1 COLLATE latin1_swedish_ci NULL,
  `username` varchar(50) CHARACTER SET latin1 COLLATE latin1_swedish_ci NULL DEFAULT NULL,
  `fullname` varchar(50) CHARACTER SET latin1 COLLATE latin1_swedish_ci NULL DEFAULT NULL,
  PRIMARY KEY (`id`) USING BTREE
) ENGINE = InnoDB CHARACTER SET = latin1 COLLATE = latin1_swedish_ci ROW_FORMAT = Compact;

SET FOREIGN_KEY_CHECKS = 1;

```
