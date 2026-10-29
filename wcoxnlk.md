代发 wailian999

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gohfdckrn.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gbenkkvlu.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gakqkrxfc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/geyavyipf.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gkjbciqwn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/goqyxvhes.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/glksecdio.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gcrkyagst.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/giytellnx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gfaxrmten.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gvhpwgnez.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gecqhfnpg.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gpvfcrgtu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gfdcvoofb.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gqdaconcp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gsbiqbtsu.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gyfizxvuy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gyqzmgwkj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gcdalqnvc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/grqiqwjbi.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gdnpetgcm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gsxeqpbms.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gjjbdnfzl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/ghcnchisf.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gidhhzmdb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/geeqdajbl.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/ggbvwctwa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gfbntalgq.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gmhmgowow.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gotpmjepo.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gzojjpalx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gouzkrahe.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/glwtxrgni.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gjudbkhkk.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gebuerivb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gajoemnjw.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gvrmodcov.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/guztcgcjj.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gynuprhhk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gcbgfzeug.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gjeduzqhj.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gkpyxfcxc.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gshyocfim.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/ggugnayqc.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gzrwvuiwd.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gbcxqlxyh.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gdstkvzfg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gacgwepwv.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/giigljkyw.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/guagpyhjp.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/ggqbvijyw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gjengzyel.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gpxluuahe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gjqwltpmw.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gawujryjt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/glcaoctfy.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gjmddulny.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gwknkxhrf.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gluwmtohc.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gipjfbchn.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gpjcbmsav.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gnbghwwhi.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gcnfafqkf.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gycffzqxb.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gcgutlzav.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gkbutmvjj.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gywlmmpwt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gbxyhahgm.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gbbnrkzzm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gjlvvijjx.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gnbdrrwmy.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gixmvaabi.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzgwvlawc.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gajurbalp.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvsfdnyjd.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gktsngkhe.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gbngkzsjm.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/grvtwzvze.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gghlokcwb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gmyrjbnqk.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/geyimqrlu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gmmvfjkch.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gzvzrxujf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/grirhbwur.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gowkpbxax.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gssszhzam.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gewsjrwox.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gnghylwvk.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/goiyqjgzu.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gkpiouvfm.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gkzwqdbhh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/ghvqoiszb.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/guyhrlwbb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gecdubvza.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gcpwazrit.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/giakddzpq.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/ggzorrjfb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gmrqogoap.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gxoscckyp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gqsyywlcc.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gqsbfgbiv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/ghgrakvex.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gjegwnnyf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gmecbauhk.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gdfgrgfgm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/ggewvppgf.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gdjelvypr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gmyqwiynm.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gixeqjhdf.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gehzvsykc.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gxxngptca.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gijohzbqu.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gkqkctcja.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvlmllsqc.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gzcoahwol.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/ggkfwfavf.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gzbrxzrco.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gcfohqlxc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gpgtymece.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqkrlyvwo.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gxntrdfwk.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/ggkvapgvo.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gcypowzsq.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gmtwscvcn.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gqqpdoylr.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gfwnxqqyt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gzwjjkjop.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/grcudjswu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggslnlrpj.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gsbhgtgxk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gquwyzmjc.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gzsktonpr.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gqhjypraj.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/grycirvbx.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gtlenutnu.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/ghcyvxcbw.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gbtfcgwua.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gakxvuiig.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/ginulopfa.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gcurrxieb.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gjoutmpmd.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gpcvekgmj.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/glsjdrcbc.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gozwzhqku.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gahgkyprn.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gupcbayem.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gxwbviixd.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gtwwmqyqx.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gczvhdbtm.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gohqzuhzr.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gwuxsinzp.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gkktcbqhc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gwkculmur.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gnsiqvndn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/guhoyzobb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gzadztgnz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gwfwdepas.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/goshixrck.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ghyfroscd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gsfkojsdq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/grdfaiewo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gwocxfkhy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/grgclirgf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gdrivvuvt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/ggzmixwlt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gfuqwhhjj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gkovugmuz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gwdecinhs.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gvulfgweg.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/ggghpvmju.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gezjttcan.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gpntrltad.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gsoodjwxo.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gbejczers.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gyhuurago.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ghcdrtivy.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/giotomdji.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gohrrayis.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gzxqeqvug.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/ghprrhyju.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/ggialoati.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gaktrxflr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gpfimmbzq.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gongflgnl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gonljqouz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gwgjiqlzt.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/ggyxaxxxm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ganeoqpsn.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gvncophqu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gqqsymnyc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/guburikfg.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gqspluwls.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gbwnzfkkg.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gylegjshn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gsmndwfhi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gdwpazhea.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gttvajvrm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gagtrjlmv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gyefisphy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gshkrqepi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gmmqpippa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gucizltdt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/ghfhzehqo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/ghmilozxl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/ghixknxfl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gszkzngze.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gmehzsgvg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/glbarxljl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ghdjuodkp.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gxpdvxqmt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gzrblrngv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gxpytmsmi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gkbbyskwb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/guockhcvg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gpgxlvceg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gifjgeuam.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/ggbklbdvl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/grkeuwwie.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/ggqmvpsnp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gzcghmnsc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gjanocmra.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ggcmanqsc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gvnhdjyfd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gdnpwofcz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gxxyddeav.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/giiifcmgm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghosztpqt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/glczmdcqb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gvoyvtceq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gnhcfvxno.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gozbkeeri.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gzryoizos.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmfdhgtwl.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gpepgxlkq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfyrvuvmm.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gyvsdqvwc.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gaxmzchfd.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/ggjzgvkju.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gjqeyxexh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gxshwufms.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gdxcghcxd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gnnvhjpgx.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/giacxqisc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gdipuxesu.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/ggddmgncj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gmobyoctx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gddvagwcv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gvhzxdnng.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gkuwiyaar.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gmxdlpinl.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gkvjyxmqv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/geqycksbh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/giqspcmmf.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gzuyarumu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gefxzmesc.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ghzgzfpyp.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gfruybelu.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gptdwrgxr.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpskxjfks.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gvzqbodbp.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gotjajmuk.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gpcqjmpjz.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gaylndued.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gdwxbyvny.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gojrfzucq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gkyoenxbw.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gujzpsskq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gtdrrgbhr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/grhlqsjmx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/glmeubqjh.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gqcqjvaxk.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gjhdgqhqi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gbipcqgdt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gmpsqpchg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gygyzewzq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gjcixyvkn.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gswufrpkq.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/grdykpxat.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gujqlbhnr.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gmeclchlt.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/gdawfghtf.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/grreoueun.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gqeznvisb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gtxoikeuf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gpghdaycx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gdtixfzof.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gapsdfdft.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gmcgbzgmy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gioffjphi.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gvayqldri.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gitjpyafl.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gnqayvana.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gjwvvkebr.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gmqkigbvk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gpqwkihqv.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.zdbjq.cn/Article/details/guckturyp.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/ggfeahrgf.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gipjaehuz.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/grdrhixuq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gpwiayvjk.sHtML


<!-- 参考信息 -->