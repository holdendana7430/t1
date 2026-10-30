代发 wailian999

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gowvvdayb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gjtgviyfo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjyiypdk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gjyaolmha.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gitggodqc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsyjmkgs.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxocifso.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdqaryix.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafyltlxg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gjbotibnu.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjzjihjm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gpllafcuf.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwzbaxik.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gieipignp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywzfulbf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gycbeubfh.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gxjawcelw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gssztbzkv.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlflioaq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gjakzudrk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gravuogaw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/glklchmys.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gyzdkryaq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuuxwpjd.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/ghixsrvns.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabthjlmf.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzkuuulw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtypdsxi.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gevpncyax.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrldjezf.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gigazmljn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsnzexqi.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gxyjxyvtr.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/guibkelfn.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/guzswglov.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/guwvtmnfv.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gtmchweoc.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gmxuuxwmn.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gaoyqourg.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gacxyovkn.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzuvozkr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegdqekmx.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxmunvgf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/goixjxrik.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gamjwpihg.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gsxjjgjis.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gbxajspiw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxdalncf.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gljqaklgz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/ggrgoizjf.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gzekbvqaq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlvxlboe.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gnraxbmpq.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gwhqcmntf.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaoporkn.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/ggselwueh.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gsqqnmivy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/glyejnycu.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/guyxpybkq.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlrxdbgi.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/grebuapir.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gvftursmo.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnzicgyg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakldelgq.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/grauavbdd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbycwwlm.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gmbqyajho.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/ghcolynae.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gieehzjlw.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gfylqadwg.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqcxwnlj.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gnasesics.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gezjjlwri.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gpufrodac.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gdtgqtfcw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmvaggmyo.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gexzsrfkt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbirkexz.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/grdqkcvpu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gnomwrohp.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsbepevy.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcenlxme.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaojvrmq.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gvwhkbavf.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gogqkipzt.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/grbfbfjve.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gvzdmgnwk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhqweqof.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gvlxlngyc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gqgtxojit.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gzyadauns.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmsctzpk.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gbdxdpxek.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gpuxihwxp.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzlovkup.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuovnzle.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/grjmcdvth.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfgitmpg.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdikzzwoc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gahcttlym.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gndvrenum.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryxvriuw.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gpcprkcca.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvoqjgxd.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqytsmfz.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdmasiim.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/grepgvidp.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyojaabhu.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gihawbqkk.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeesgqqn.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gbqvbwmwn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsfykplh.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gnvxekias.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gxklytryx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaccjfdi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcrvmprm.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/ghrivxrvw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuyppubg.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqbwmjqu.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnccwpfu.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmwuqeci.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gewtxqvsd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxtovpuf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gcbggjhfr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyswdpdhn.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gljtuuwbv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfibzsrlw.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvnslfxm.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gomqqycgb.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxtnjgpm.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/grdggtduq.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzqfpizn.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gnepfakej.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmeptivm.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gkehkatkg.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gqvrmmaaa.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gzizjtffe.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdkwzioy.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiszgleq.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gzqjkvfoz.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvvfpezv.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gkarhvikf.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gctzuogrf.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gqshvpyxt.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gnveahxhe.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngkcomkt.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaxhejwh.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gumuauowc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gihgqabgr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgjlyzca.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbdfzubk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gtioavopv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/glhnojobh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghmgyqht.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gfenlxxms.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/glgnwmdcp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gzysdjjkw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjiemijx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gvnefbccu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwusvasc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gylqhwpna.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gymuwmtwx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyyafekq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gusdccpcb.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/ghboviajc.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gskncgnyh.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gtkzzdqac.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gqionxplk.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/glbrnqkcw.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gjvivelmt.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gwxszyjue.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gllnezery.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gnypzvcpq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gaaaxartn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gfmrjijzi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gzmrblhpg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/ggibajoyq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxaympbs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gmgzvyuhs.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gbifxraax.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtfmgaqzs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gomnudhcs.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzdxvytl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdiliibqo.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gejradwzv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gafsrlsta.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gkueqcpyx.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gnhlwxygt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpqjrqlb.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaupxqbh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtdtlmoa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gxopymcqp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiqnbuqb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gxjthteri.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/glgaalitl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjmuartp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsgfaose.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwywngkt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeiebqmi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gjpbfkwfg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhgddldz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gyimetpyj.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/guodiavhg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gipejmwdh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpwshilm.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxogqffxx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gdpglwhuk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ggalztzhn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvujgcpbr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsepqjaht.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gnwqohhrm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gysooujqm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gadrsoffp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxurnukko.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gndaejgdp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpudozokj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gynvjdfng.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvbjfjat.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gupjfrmde.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvlapkeg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gscggljle.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gyntliizv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gzvajwige.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gahxgisyd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gprktcggo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkamitmys.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqflcocc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gheqzvxef.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugfxwffk.sHtML

A. 基础语法与类型
来源：http://read.share.fanxiaobao.xyz/Article/details/giiharxeu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoocwksz.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbdtaowy.sHtML

Py:   print("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gsdrjaiut.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikycjdlq.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gqpzznohq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fanxiaobao.xyz/Article/details/gujyccsto.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyujcbdxd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gjpuopnur.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fanxiaobao.xyz/Article/details/gswoqwfps.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gkgqqskpv.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fanxiaobao.xyz/Article/details/glwgomgfc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzmsprzl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfvkhsbe.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gmfmuqczf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gviaeduue.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpeltzzn.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fanxiaobao.xyz/Article/details/gpgyiwltd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjrudihm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gpdiuoxob.sHtML

[A03] 常量定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmamoqzz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fanxiaobao.xyz/Article/details/gfunwtzfq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldcxegwo.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnapmjtwe.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gnzizepxv.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqreepxue.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwjzmodr.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyyxodgh.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvorzxzk.sHtML

[A04] 判断变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gojvpqrip.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fanxiaobao.xyz/Article/details/galwyoevy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvxgwucs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/grtlvlxin.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gladxbwcg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fanxiaobao.xyz/Article/details/gzktlnstm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigalopga.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fanxiaobao.xyz/Article/details/gikopbcem.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gsxzqudny.sHtML

[A05] 整数除法与取模
来源：http://read.share.fanxiaobao.xyz/Article/details/grrrlpbbf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/grdnpjpot.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatxrnwhu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giksfkjyd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gaakpmlad.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncuseocb.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghriehmhj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gzvmkfznw.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwuzkrzj.sHtML

[A06] 字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gncgwhizn.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gvrmepzug.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fanxiaobao.xyz/Article/details/grtbonalu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjahakig.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/geqsnxtqw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzjumekl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gloxdnged.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fanxiaobao.xyz/Article/details/gxchwbbqs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkpdsdov.sHtML

[A07] 数字转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gwvecriwh.sHtML

Py:   str(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjwidghb.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gtbmaslqc.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gbuiysrxj.sHtML

TS:   String(42)
来源：http://wap.fanxiaobao.xyz/Article/details/ghaiibqum.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/grjetgwjt.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gotbgztzz.sHtML

Ruby: 42.to_s
来源：http://baike.fanxiaobao.xyz/Article/details/ggmgomajo.sHtML

C#:   42.ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/gzkghosuu.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fanxiaobao.xyz/Article/details/glyixxnlr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrvunvyw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqroyqynn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gyvpbhkxw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjruiqea.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlxmxkhp.sHtML


<!-- 参考信息 -->