代发 wailian999

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgpigbbr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvddviui.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhuziaxg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqrduwhn.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gmwgmdddr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gbposwhzm.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrgyibqu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gznmjnwak.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gljawawbl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzibjjmh.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gcbxlhytu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gadrmpsvk.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gutgyloyg.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gmsugpqfx.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajxoguat.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/grfejzpbb.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/guqbslwls.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcpydmpp.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcweeispr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmkapzpz.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrsamhly.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gpoemaysl.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gymfmzgye.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gbegdadcz.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gsualrzen.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrtxcayf.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gldepcmfa.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpyonysz.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gjbyhwxsb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgqhojru.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gxanqgcui.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gscfaxpzw.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppfduacs.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gjlgihhhk.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gfqtcqbko.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpfemwos.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxjrdkkj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/goybmhpji.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gwheozpqk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/guziuzztc.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gximajrqk.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlolzjgn.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihlbjteq.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gndpcvpms.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjpqnfzs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gahrtnnkr.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gxjiuebik.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gdwqwtfss.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gmursicqm.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykgjwfqj.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqikydudn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/grqjesryb.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gycowjiqh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gmadmutop.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gzbfutpik.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/getebkfvp.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gexngvdzq.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtkibjqh.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmulodvbc.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/glzdxtqgz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrycfeug.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzuzqzwb.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkrdcbjw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/ggkeunwmz.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gflvmdngm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvroophkt.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvficfsbj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpvxurmw.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gfflvkrjz.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gtezsfptj.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gheimgmsr.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjkedyan.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gvukaxxwm.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkrabhtf.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeythajk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoygogxy.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfdzeict.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbkrhgdr.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gfntdvwby.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwpwcvyc.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwtkuzhg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmoxqjth.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjxoworq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnmuifrc.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gfyvqszex.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaabuvaf.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gwjrwlxkz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gjszgvicn.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrsechrk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnhccvjg.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gmglpbbxe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjiuxorj.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/germrvymz.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gqhvahlen.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzyidbvn.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlqzisiv.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggllkdebz.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gktssdyhz.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqjgnabw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkekrbwba.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gsycrfevo.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmepdpgk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gzxeknrkl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/galicbzgs.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gwcwnmjrf.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/glnmfflzu.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/guwkfhlak.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gmffhhfva.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfcnbyuh.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gizznaiwn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsawfkhdx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gsznvgmxq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gofmxeywo.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gwglcjcsl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzpcigqo.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gokzxuhle.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gvvtcyusd.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gadquwedo.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gkecnycfh.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gylikquhi.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/garxtsimm.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvwlbbnl.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatuelaus.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzgfzbyo.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gtcasexes.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/geykvilcl.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/glnnozoqy.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gyerpuagn.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerahlzux.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujqkgkku.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gafpnuald.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gesvoqgbg.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gpdqddaww.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkoyaigu.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrwtakci.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gaxrmnrpk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gxphkvhwr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsxtioww.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqbugkdo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gvyddsoym.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gwgvlyzbi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/ggjlmujml.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gnzkutgoz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gisybyalb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/giorkabzv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiwmykuc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gxflucjly.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gcxrmswdj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpdngvmk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gaqttpbfe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/godnfxdnm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gnzssmefa.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepbudqty.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqhrbxxr.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdlfxtzd.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gkpgpizqe.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyzgypku.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfloqqiu.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/giessvsua.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsnkvurb.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/grsejhfoa.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeoeobfp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/getlspcmn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmmdkmiu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnacahag.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbipcnji.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjaeubcf.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gydteuacv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glnjaumhh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzwzblwm.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwmdwxlm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzofamlu.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/grqwlcjyw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gpfzmrhei.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuvhazvs.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkyrjjtj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmweqaol.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/govknhgow.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfecdybzd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/glxfjrtgk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmqzawmk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gopxrukdd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/grmwxqyck.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqciuzfe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gwegucfru.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gjwjovybk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gkovdpvry.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gsghxvqry.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gmjkzvtav.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgqekemv.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/goitkkhbc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbjhsqaz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnebouehm.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gncbmwpss.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwmkbxpv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpwklifs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gjgfiifbo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/glpxlddwe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjeegcjb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/guslpmpaw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gexwhnuvj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnirmvpcy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqxaplbek.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gedktqkpc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlehpwwq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfzykvyz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gibopansm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gyxaphuyb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvagexbfj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gjowvkrqy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gwugeynku.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gufhwlppy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxtxqknhl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfnwtlpi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/glsbpeepm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbujnngmc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gobvtznwg.sHtML

A. 基础语法与类型
来源：http://wap.fanxiaobao.xyz/Article/details/gkksmwejs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsddyxwa.sHtML

[A01] Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbekduex.sHtML

Py:   print("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gwoyfdsty.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfatgahx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gansptrkd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fanxiaobao.xyz/Article/details/gomfotcsh.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/giarhjerk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gpufxdnpm.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gctdowwht.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gtduwrgnf.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfyizoly.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxqkorqm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnesambe.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/glcfyxirv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gpmbyksli.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcogsmfv.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fanxiaobao.xyz/Article/details/gidtacoys.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fanxiaobao.xyz/Article/details/ghfcxhcvt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/ghicidzeq.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/gyrillurt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fanxiaobao.xyz/Article/details/gpymdgzms.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaippbses.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gsvknwqbp.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gonjskckc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzouoippl.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gadmpalzp.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/geuljdpxa.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/goeyifyhm.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedhjvtlw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/ghtxplygj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gpybcgwgs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/ghqxvjeov.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejohqfcu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fanxiaobao.xyz/Article/details/grtpxxgaj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcpxoqmc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwwvfiwk.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/gettkedii.sHtML

[A05] 整数除法与取模
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwapfcel.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fanxiaobao.xyz/Article/details/glwwdqpjo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdprgygvm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdirgieq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmvhnwlx.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqjapcxqn.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggysxnsjf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grarkhqxq.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghezsyocq.sHtML

[A06] 字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhuiqjps.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfqgcyvz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeifzzws.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnagbitwx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/grqkphlva.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/ghvtwoutc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fanxiaobao.xyz/Article/details/gibbuetdi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjveurfn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwdvtcrv.sHtML

[A07] 数字转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjlzxxivd.sHtML

Py:   str(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtltylbzk.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gcadoouak.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gvuxohhfc.sHtML

TS:   String(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxgzqrgp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpobtsuv.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grytpskkk.sHtML

Ruby: 42.to_s
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsgnpuyn.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcohqjomx.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyetyvgd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/grchcmiqg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgrrymvs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gxkncftug.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gophcufbv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpcclqbw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gpqpjvlej.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpfgshcy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gqyqnqfqx.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrwjcjpx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gurgebbhc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/guaeqejfe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjphhtfkk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gimamnzxm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzozmidq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fanxiaobao.xyz/Article/details/gyshuirmc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fanxiaobao.xyz/Article/details/gbqrlafnx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gchuhfcum.sHtML


<!-- 参考信息 -->