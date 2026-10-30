代发 wailian999

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtpkhsar.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gpvubzrik.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaygeuqv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/guiqkimfv.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gbzjeekfb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gynikevxu.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsrzzoza.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbphfptsx.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeipewon.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gajpdhmvi.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gudqgociz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuthxypv.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gfbhwanns.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvczdasxd.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gtatfanum.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gtghmorop.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gmvxwnvpm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkxvierx.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdxpeftf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvmryyrk.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gjakxdjsv.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gtmtkrflb.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gzfzvrsbz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gxiadksmh.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gpagaitua.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnlbknok.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwrkslad.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpnamqkz.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gjanjlyis.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoiqkovv.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpnoayqe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gazlcnsuz.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gfaxmzxdw.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/guskwardo.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpbhhqaw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwqbcmae.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gzeavzdlp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtjlspan.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gyessscmk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gmhimxpao.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gubydladg.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gtxlzljct.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhqxzytd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/guwlmekqb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/glztzenwb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gipucvqxj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmejtodl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkeloghx.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnsmcomg.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqmeoign.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gtvepivme.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdkwchhb.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwpyjunj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqioexgp.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyauemce.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsefskca.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guabaajir.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gwisjigst.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrnnqnkg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqfgqdrn.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnlrxzuml.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gosylosqk.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoegfgxz.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gipaxzjdd.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gktkksfkj.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbshvdpb.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfecxpby.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfhbwsqs.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gwntdbjea.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gvpwklltw.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gnewfvcmh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/goahoignf.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gcqzaycqn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrcyefhz.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyswmlyk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gdssdsssc.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxskpraxs.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmbskvgm.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvvufgia.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczpckanm.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcpkhpwa.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxuywdlz.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gfrdgtcqh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqivngrkp.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gocuxlmya.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaprqodnd.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gzmpitubq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrxfstin.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gjttcmweu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gbrfgivka.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsezxnxw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gkvzcpmol.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehaeitzs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuwsmwce.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjfcgcdw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gyomvzkxe.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gutdiivet.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkptspmoi.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gszigsfol.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gquayzihi.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcljnsakx.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gbfnqcqbi.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gjvmhogof.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhqjgmbc.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gturcgilg.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/goazraoko.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gddpdsfjz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqprtonw.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbmlidob.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrihlpha.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzaujosy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvugktldp.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbslyntel.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gghrotchu.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gikilfadl.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gcalfhuil.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gvuokbcri.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfocwfnk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gihpsxxuo.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/grirlnckl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqmwglkw.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gusemcvxu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrezgdxh.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/goomcxdyl.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gylhgzpos.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyhxkkuz.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsezellyf.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gnjlnihjx.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngpkzuor.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwfzvltg.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gxprbjuwm.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gpejiphrv.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gtapktgxw.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/glysaymhb.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gthnwmziz.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gtvdyivcj.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gafuwbkte.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsyguyku.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/grqkmuhfi.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gdepefact.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gazzrnznk.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlngcvkp.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/glsvzworv.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlygwgja.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gjbduhmop.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gmkxzdnol.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcbxyjyp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gaykdtddk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/grszwhuav.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczkakzog.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gkvzthrmk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gfakoltwt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gvcddmsxv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gloslvyvb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkdtkppn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ggyfuzvry.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/grqtcgfho.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/govbydcwh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gxuhncvvs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gbbxgkdel.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gkeyyspmv.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxjryncw.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gotmoaulb.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/genawghwd.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gpdxfpuig.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gjielwcuo.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpaenboy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gjohbpqll.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gnnutqjdu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/glxplaklj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxvcuicd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/goxtrpmab.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gmfrbvoxe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmahjzgif.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfphoblz.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gcdehcvkk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfponkvod.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssdeqdpo.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghamnmwpd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazuwnavs.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyhgquii.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gjytesedv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/geszzewhl.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeiyfdif.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/grmjveinb.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnfigfjp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gzmqtlkmg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzcwilxg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/ghwzarsmp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/geuqpnfux.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gmamypzpc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/glvupteqh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbdhkbzc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gmofnqfgz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxushqzmw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbxlubkg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/guyiyolbl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzlespzr.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkceqhicg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzqluioo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gtdcztpxu.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiikdbaw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gjikkqlob.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gegnfibfg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdjldjjzw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ginertewk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gibqghtnr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gccaxrogi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gguojuwqa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchjlbqob.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/glmvevaii.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gergsvhzi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glidgrqpq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gtytlpweb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/giwtisltj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gmsfoxypv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdzgcqlk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/grcuwghwr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzojmzntw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwfdbqrn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwexuemvc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grikmnofa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gdscreyyy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeogyflz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbikhlxqe.sHtML

A. 基础语法与类型
来源：http://baike.fanxiaobao.xyz/Article/details/gcmulpgwc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfmglieow.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glhfxftqp.sHtML

Py:   print("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gsmclhrlw.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fanxiaobao.xyz/Article/details/gtaagbhjr.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gicazybyj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fanxiaobao.xyz/Article/details/gqmumgdsj.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gqfaatyrl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwoxkqjx.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fanxiaobao.xyz/Article/details/gvuyjmdxu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gizwuhujv.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoaujxym.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqrzlgkh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiyicbyr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfdmurjk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gfnjjgejy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuhkzden.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/giziqlqwm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gjulgrzie.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gstfqeqjq.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/gzcfqkyyb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/gzulfwbxu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxkatvla.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glvjydqdc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsgjbqlz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxivruzq.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmsvmgth.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvqykklf.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gizirajvp.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gixzwjulq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gknqwekuh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gppbyswpu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvdgkhpr.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gonxzhnqu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fanxiaobao.xyz/Article/details/gxsijoltf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fanxiaobao.xyz/Article/details/gncutrsmk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fanxiaobao.xyz/Article/details/gsytxuixr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplpyfkpb.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnykzaepi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzibmkaj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhlrjinr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsvfxver.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwfvpobcb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/groxbnxhj.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdiiexkq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gscfwmnnq.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdomaeqnj.sHtML

[A06] 字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gejhqqqyn.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gobuyuakg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gliapsdxi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gpvmprife.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsjiwmth.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gludxsdjz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaktrlcwd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fanxiaobao.xyz/Article/details/gnncvrjip.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gyhewrqle.sHtML

[A07] 数字转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfpcxvsz.sHtML

Py:   str(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqoetkoj.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkybthpq.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gwucxpfjl.sHtML

TS:   String(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpbibiao.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gucxffmof.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjrrdjkg.sHtML

Ruby: 42.to_s
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxywydqm.sHtML

C#:   42.ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfwzlwrn.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grejeoocj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhpuldyk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fanxiaobao.xyz/Article/details/glrwsbdms.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/grzhdnljh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fanxiaobao.xyz/Article/details/gbwswhlkf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqibpilyc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gipriwntg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fanxiaobao.xyz/Article/details/glwrnrstf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gcpkkjghq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqxwuswb.sHtML


<!-- 参考信息 -->