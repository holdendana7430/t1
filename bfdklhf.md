代发 wailian999

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gjscpkhxs.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gdqjigeir.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/ggzhoavua.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gvgjvrlqj.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gfqydcmlo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gfkhxehes.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gwojmqwsp.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gnprbsgeg.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/grjfbnknw.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gtsmrpoxi.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/grpbvflzd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gwfainvht.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gbikabqie.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gbktlhbqr.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gfuydmrbs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gzpxtwqxw.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gbktwyium.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gfyylfxen.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gqzbwdfyz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/grtwmqntb.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gypcaptgd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gzpjkjmoh.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/guqrbtxug.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gxzlymfgv.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gziunhdxr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gxypeukmp.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/geghflqwy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gmqlbcayu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gqsohludh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gvwcsllws.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gwknqufeu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gdtnnhunf.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gfemjdwdl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/guaswrzno.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gmwmowxzw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gzdrmqyjq.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gfnuunnwb.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gtwwladbf.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/goakvuyvy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gykmbijdx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/ggmzcunid.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gmqnpqeup.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gwnqfcyka.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gmlwowzmg.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/guwvpvjii.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gagjnbbgl.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gfmdhztvv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gqllmawis.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gcumxisrv.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gvdohvuqw.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gkodtlprk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gokpdgkxu.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gfxjvuygq.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gwtyanzob.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gjzkeyrgl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/ggzcpkbhi.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gcmkmhlwb.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gujthdyql.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gyxfvatvj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gscfmmive.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gakvqnnqe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/ggnzyaraj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gjqfryunm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/giadflhis.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gxphhjhhs.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gesofghqu.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gkehdfotk.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gdiczrrvf.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gaoyigulx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/ggpbszarg.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gouisueaf.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gzcvjevag.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gszlxkchr.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gmggatfle.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/ggcxwkpwf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gwujutxdj.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gvtyzxagu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gvyyyghwk.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/ggnmmaxuj.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxfuvdflh.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/guicejmmu.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/grydkxpfg.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gwwmkoghe.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gscfjlyne.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gicwvpvue.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gqqayxnef.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gaklfthfv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/guacltihy.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gmukuigap.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gmsxzgnnz.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gpfigfjoa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gvidvpxdc.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gzqanhlaa.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/ghniopwpw.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gaaocxdbk.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/giqezjwow.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gglepxknc.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gvwothnxz.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gzrighsaw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/goenvemsy.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/glqhuzyly.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gwdonlqys.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gctfqpabs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gmtlkfgsu.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gtdpnqwpz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gmozvljeu.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gtjedavzi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gogedbckf.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gcpvhwlol.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/ggavrwtlx.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gauyzblnp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gzdwtkkvt.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/ghaxsrwfb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gjwtmynbh.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/ggaapcrsx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gwnqumqsd.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gqamsnlbj.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gioxsbqfk.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gqchllihm.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gacreleso.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gjzazmsjn.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghqlapzzh.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gifjyovqg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gijnqudxo.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gekuamqky.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gdwrrhbnt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/grmpnvlqb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gzkpkgqpj.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gtfeahulw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gljstbgpr.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gilckgsaf.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gdfajtbxu.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gknbibfwy.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gokscymal.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gebjgcgmz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gflmripih.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpaxsrznn.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gclzlnslo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpvfpfazv.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gavyykjnz.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gikeaeamp.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gcihwlhgg.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gtepifrxy.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gxmnuqwhk.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/ggplvykxt.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gmsajkkvx.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/geaanejzp.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gmjrprmik.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/guxiyittj.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gatkyodmj.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gibdocnkd.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gfdkclfnf.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gtbxxzerl.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gfdzpjsmc.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gujcxtlfv.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gjukrymmg.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gqrffdvmb.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gzjwsmpzb.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gxiunnegj.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/grjimvyxy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gqkhhvqga.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gliqlpiyw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gnqxzytpn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/ghrifirnk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gsfxblysq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gpspzvcol.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gxqerqefy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gxjuuvzro.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gceidltld.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/geedacoks.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gxnxmfegw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gbzkwolhm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gghhafrzu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gccgrypnr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gdrxqlpwi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gpbwiuopp.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gdbrryels.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gsyipdihs.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gcviebngc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gztrvbdsk.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gjohhistf.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gdzsjomld.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gucruqafn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ghuvgtkpb.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gjdrepoub.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/glohmwcyr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gjkltmpbl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gluaynscs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/goxnysubj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gsrobgann.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gaezypqcl.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gjuzirywv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grcjnkmxm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/ginvoisfj.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gvbzhtoxr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdegwjjgh.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gjutpjxmn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/grrfmwsng.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/guoqyqvvu.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gyieluxkt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gqsgozdit.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gzncnumyc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/ghjgnufkh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gcrlnmspk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gnfbocyeu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/glldxulco.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gsklobhqy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gtljxgryw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/glbraahew.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gjhbpknty.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gootwjvyj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gelcemgae.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gvogjgbcd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gjdxwnrsc.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/guguzgnrs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/goizhxbki.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghbcdfzmy.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gtvkbrjff.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ghdakqjuv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/glbtszjns.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gayoxwryg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/guhhpansr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtwjptzyr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/ggocjhezb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/giqmabcya.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gwxiyvwya.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gmjzrjuis.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/grvprsoat.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gkvsphsbq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gnchygvxs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gfxyghfzf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/guodwcjlr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gnykobssm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/grtzpgavp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gbbihmgwi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/ghsihqofr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gmtleqimo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gormamktp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/grgmjnlmh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gtjyhdprq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpjvqakki.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/ghhnrzuad.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxyjogmoz.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gfcckxdll.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gafbfwsfv.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/guarmastz.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/ghqrurfiq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/golxrnogl.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gbgxzdgrg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/ggfnmlcxg.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gyldutpof.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gvcycmgpi.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/goanpljiv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gpikkozhb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gtqmwftpz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gtvklteqv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gwsgaenfd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gucdgdjwa.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/glcgtwejv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gbfghpudj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/ghkdswzjq.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/ghagjmhwi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gqqfalnct.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/garlcawke.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvcqvjqby.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gpghnfhkg.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gfprkkyho.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gjvpfpuzn.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gelvyzopm.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/goyoatjjw.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gkbycrakh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gfvwxicne.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/ghazparkq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/ggkfeywsj.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gpfjtfbux.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gismptkue.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gzccjrlcy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gsqhcepsk.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gfdyrmbyj.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gmzlvibpg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.zdbjq.cn/Article/details/ghwyinwdc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/guwqhndld.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/grhzejamb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gtfwutbpe.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gbsqregle.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/grkmebcgn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/ghbqhuqcm.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gvfonjjxi.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gvtmsiroz.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gihdvxaux.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gadyqgvzy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gkgdvtaqh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gwihfnzjx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gkxoogjin.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gojmozelz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/ggadrmyuq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/gooizvrsi.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gsxceiqyn.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gwttzmwtm.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gdcjbgrho.sHtML


<!-- 参考信息 -->