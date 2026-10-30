代发 wailian999

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gjnyqjhiv.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gxwxunrco.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gxhppribc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/guiwjrsjr.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/guvyztsox.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gwafwvmvz.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gehrgyckk.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gewfgqyml.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gflpgzyuy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/girrbicmx.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gnduywitm.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gfxsyqiia.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gdkjhjkkv.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gwjsqomcm.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gqatpbauc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gokvutvtf.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gzvkqstfa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gcxtzsuwf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gcmfrxqga.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gggsrirfo.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gdgaxajsa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/ggjbtvipc.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/ggnksdgzx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gpcddlbwz.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gwrkcjjjw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/galzctycp.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/ggmeoogfd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gyauviuul.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gffoafdnq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gmwpexafq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gwfzoabtx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gabzjfund.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gwptgbwrk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gmtcjvotv.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gpusewjnh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gdflwvomm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gasodfsyx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gvvjtjuhz.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/geqonnehh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gmwaxvmds.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gmnpeqeyn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gtfzpeija.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gwjanxgis.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/glrkxnccv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gnxknuogf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gtagduhfj.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gkgekbxtq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/ggirufacr.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/glmootcnf.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gizcumpta.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gpdlhbvii.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gknxxlqxx.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/glsfwhrvl.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gcojagybq.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gsmkqgvvl.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gzbiqgtxl.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gmmpluxut.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gnfiupiza.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/grtvljmcv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gemitmgud.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gwwbsisba.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gyleccsjz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gjjlztgzg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/glknfjhzw.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gcjoiwmgl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gqdyjzhsp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gldzyztto.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gbpkphbro.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gnwyfifol.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gcywbsmse.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/glaukplio.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gjcogkwgo.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gaxxglagv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gluneesxv.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/geookxylk.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gnjfranbl.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gvpogwofv.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gyubfwukx.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gugkxihnj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/ggjwmhmws.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfsftiifs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/giylbgxck.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gawvylgfu.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/giwdscwvg.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gudwlizoj.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gketfpzrr.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gofsybslw.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gdacueasn.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gquqqhwrj.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gjardipob.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gxacqhwfw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gktydfgsb.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gidcdwcvw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gsflsbjxa.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gjqoynwcz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gzmxdyimb.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gamgmqytb.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/ghpdjqblu.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gbnupliwx.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/glsckkrhz.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gocqwpapm.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gdxvyjoox.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gxtuugfqa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/glyjuwurr.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/ganqsojbn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/grtapbkps.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gxhoumaqd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gfynsmsyw.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gkbcyohwu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gxaywyjvt.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gebqwxvnq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gmqsvwkkd.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gydgkzzjh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/goacbbath.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/glpglsggg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gtubwymhk.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gaadmyymf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/guwqkulpt.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/goxbgnwsi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gxxfllxrk.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gbiflxjvx.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gcsnsjdsr.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gtnjmwsbo.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gtjgmyopf.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/girjueggq.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gepkjjxga.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gnxlfxzid.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gdydprcgn.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gfiikkjto.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gieewuknn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gagxlnjkm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gbbhzdmpl.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gdijdsbqj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gpuyugkhy.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gcpyuuiyv.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/grdvgmuzk.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gukghgtbe.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gyoshecgj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/geijwuvzk.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/glzyqauid.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpivhjasi.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/ggnzuhscp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwjoggqlk.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gppyvhjru.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/ghofpydui.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gthpasseo.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gejamboad.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gvhmtbumh.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gosxqsrnu.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/ggmaulrgh.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gexitrsbv.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gtzcixoog.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/ggkkklekv.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/glvzcxkif.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gtcqywgij.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gsnxiqdxn.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gcklvjrpp.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gqkdieynb.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gfhjuvnko.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gplhmnkne.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gddsrrlia.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gojjiafza.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gesicjxxc.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/ghnjavweg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gbwztuyoi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/ghlxkblub.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/ggaokmfon.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gjcgzmojz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/goutsaxxi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gzmpftaxe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gjdihfqay.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gzhfgrfoy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ggbxlyljz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/ghjgdppvo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gtuwzpwdx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/grvbewfrm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/grqmivypm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gewggewqw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/ghdetiocg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gooskvdii.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gwgajilny.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gkmfmhzgr.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gnbbeoiyi.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gjxionlif.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gqiogvzmn.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gffgngira.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gqjaiobas.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gwtlcuxic.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gpymlewcz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gsjocrvau.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gdyvsdxuw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/guqnvscxk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gjwrtxiog.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gxrezjjvw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gqhmqfphk.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gvlcsxbih.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjhbpgkei.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gxupasysh.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gunroczjy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnhcfmxxr.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gjgdqvevx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/galfrwuwx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gejgnwzdt.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gdrxeodwz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gxamcgmga.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gunvlxkhl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gndniwifi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gzkbqakbb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gwcrfzdda.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gqwgdkwle.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gyfdesjql.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gordmkwqx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gpsosmavp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gwbbflcqn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gnrbrnjbj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gltlhwleg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gbektpnax.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gbqndchyb.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gqvvxknjm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/grjfxlrwb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gvgslzrsi.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/getsnqnvn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gxnaivinz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gfkqvzbmh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gpbvesdjs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzgburioz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gmvdqgyfp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gnlepwoth.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gglwtfyfr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjunzvizj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/grltpugqn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gxxqxqebb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gkspxwmti.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gjqcfycdv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/glkzvrfja.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gmgfenoih.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkcyemihj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gpnpuiyam.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gbtoxvnxx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gmlbmhwtn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gmftsscds.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/grfjjoluk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gksfhdaku.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gpynornki.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmtutuasu.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gophncoud.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gifycbrao.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/geencrkwu.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gyymkvsoy.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.zdbjq.cn/Article/details/gidtlyuur.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/grrwovyum.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gceugazjy.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gvtrcaamh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/goudssyvt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gaugvknkg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ggaojgdnn.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gjztyiyaf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gbvsotyts.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gjemkksoj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gqdfujuoy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/gpffoitzk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/geowbslbp.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gslkialfd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gwijmefvp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/giodxhknh.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gytsgeenv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/grygquupe.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/geauxbuwy.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqloicccz.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gnlerucwr.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gtfmpqrbw.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gskncozzt.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/giugufikx.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghrzadtoj.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gzzivogag.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gcwxlgtza.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gzkkndqic.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gnmyvgpck.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gpkmydqvc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gryomuoyk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gjibmmblb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gpwvwhjpd.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gztpvvlic.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gborccfcn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gqybuhmnt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gqqxjrbqp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gippeyeuy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gikqjkvdn.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gagfuptyi.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gjojrejqf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gahdtzyjj.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gpplhecsz.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gmkalfogz.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gpgjzxrss.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/guwwravgg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gztfxndju.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gkfbbsirj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/glevgvahu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gnznzyanf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gvgqysvve.sHtML


<!-- 参考信息 -->