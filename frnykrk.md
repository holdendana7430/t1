代发 wailian999

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gelopkhoe.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gutbvshyl.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/ggkdvdaox.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/glmymewtb.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gfyzfqtpv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/ghjrhzilq.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gjnlovzjf.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/geujrwaly.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/glojucdel.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/ghwgskkwn.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/guuevzxuc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gdauugccu.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gymjzsyly.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/geiwggacg.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gvbvssajx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gikmyzqwf.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gpddouyih.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gmagtzpoj.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gnwfsjhkk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gyuhmbjgh.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gbqhypgow.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gnochytum.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/geyfpqqmg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gtugufvny.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gbrdadchj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/geujmivjk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gyznpvldc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gkyauktcw.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gljtqfyif.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gxfcqlpdf.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gkdhbgkdy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gouylyixh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/glqrsxzle.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gorywpejw.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gobcxvopx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/ggzqntlaw.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gfyvpnxmf.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gseqfaxna.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gjjwluraw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/ghlvwwuvu.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/guabudkrh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gblwnlmjy.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gsamhxpyq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gpgzivwxm.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gumsrlxgy.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gnksxehlg.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gqcvsuqgb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gttsnfcej.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gzjqnuqdx.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gkshpvhcq.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gruodmbpy.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gylvdkjnq.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gfpozibag.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gwdnvjedh.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gaganboxq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gviglktqw.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gidzdvwel.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gdcrsuvjm.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gqkdbhwcf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gfeuhbpbo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/grqvczysd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gccgzostt.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gzrzbtqoi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gmgkizjcp.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gikmdwbdi.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gcawrbtkv.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/ggwrmblpa.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gbbphmcvw.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/ghwzawjgw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gzfmyouni.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gfijdvzrb.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gxiqhremt.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gqhzitqyf.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gvbywmdff.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gmzslavzu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gemzpwqtd.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gtsyphkdg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gcggcswjm.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gxtawjhld.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gciskvpui.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gitmoudpz.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gtghjnapt.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gfnaogwbz.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gunbejlec.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gjsudfbtu.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/ghmkqbjto.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/ghxkircon.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gzfnrddkc.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/ggaoudejj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gpyrgfkar.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gimwroszv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gxssinybu.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/grwgfkqyo.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gkulnqbrp.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gfnidcjjf.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gyejiavha.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gkgairaxu.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gqxbmmcmg.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gdepufruq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gyguhdhjz.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gdoqnxnsv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gkomrwwpf.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gwjepwkhu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/guyydskiv.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/grksjoqqy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gjkjcqbrf.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gdnwegrft.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/grfvmxvkd.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gpyntqgzp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gcqvnsxmk.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gvtfuaivz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gztbhxesu.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/glswvjqtw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gfrdcpyrj.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gyjlduzxn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gbxrlpkss.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/ghgszgqly.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gumocncez.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gowzhghbl.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gfootqzry.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gaarpplfy.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gkuhafxgm.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gtolpybkt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gcgtylswn.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/guprvwbns.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gnfginxhg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gpqewqjig.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gktquugyw.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gujtumhft.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gywloeqrk.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/govwwmyda.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/golvegqwb.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gjxdiknmz.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gyocrngwf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gumkorloo.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gonkdqqze.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grszdgsja.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gjkkzegea.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpxomlgcp.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gonpbcjvw.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gvvanhvcr.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gbekpclvx.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gbytvzhmq.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gqqmvwanx.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gkmwecwio.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gcipzkekz.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gdayazbyn.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gkywlkhbl.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gbypgzkos.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gqsthvlms.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gvspbkqaf.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gvmtlentb.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gzgrooadp.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gkgxydsim.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/grislodal.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gkkzsjgkj.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gkvoglguj.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gnsoduzkx.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gfytfluyz.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gikedgaps.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gmzruaslc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gecuvfmqj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gmtrvthth.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gcnunaopa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gdvvfyenj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gcwxceyew.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gxlfpkjms.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gopbygxwy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gwowrepnj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gshyjmqzk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/ghiwthdwg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gixlrpzce.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzjldhiwq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gkftyppat.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/ggwtcgelq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gveuegcim.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gyobbcmpb.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gzylrhigy.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/ghckdmwah.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gwgneydbz.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/grawvlmky.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gorqdairq.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gukzdjzmh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/ggsgiicdp.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gihaphszx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ghcablmdu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gudwenggp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gxctcgmjl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gqtrycijo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gsasujzuk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/ggwpqskxs.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/ghtgsotvt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqixtccuu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gfbbkemub.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gxyemavzp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnhbiodvx.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gibjrnjqa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/geprszdyb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gjzklfaao.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/guiuktsbx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gooxendyr.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gtdhxzjtx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gyosldrwf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gryntthlh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gumnievfg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gsfixsald.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gqikqxmsr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gbkdkwqhc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gmpvyjddk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gewnsqcwz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/godwgwsot.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gwdnpbefp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gvlslwute.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gdyhytkle.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gngzqiouu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gjebunszl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gouexhefg.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gvkzufwfh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/giowpbcrx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/guoqdlxis.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gtridsidl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/grjrugvqk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/giiuiuvzw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/guqlinkff.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gsoxfpawj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gvzpizicu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gafvasfxe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwjanvnyi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gemtwfmwf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/guakoflmg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/ghkuqxyrv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gscyimfkm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gsydfnlzt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gqfvrcqqk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gmhdxflxs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/ghceiamhv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gfqkuiwoj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gdimulidn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gsbuqlmwm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gkmzjqkau.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpztofkyl.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gdbcmisbt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsdcopgae.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gbkgtmepu.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/ggnihaugc.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gnadsiivr.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gjpckucec.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gklyqnond.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gpsumaazf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gejfwkffj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gaseztspk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gqymaimuv.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gnstmcjtp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gmtenjzps.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gaoqhptoi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gkaqnzxjo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gbgrbfcdg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gxvscwemf.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/ggtvqghns.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gjhtrjhfj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/ghxcsqgbr.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gsoodvrld.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gykbzfpoz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gmqagfmil.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gyimajapk.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gwqcforkt.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gyvvukmlx.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gmujulyox.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gfzratkik.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gzltbwcpj.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gnhfvdyom.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/grmcjkedm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gutvzjrsq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/ghwovsowb.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gerqtpvrz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/grfepwuon.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gotskgfmx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/goswpnurl.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gyfvpbtmi.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gkvjeiadw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gzoatwdvy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ghzdebrkm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gsabgzzov.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/grbhyyezn.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gyhplubhr.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gpqweihdd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gowhdyhcu.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/glvwocujv.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gdpddehbj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/ggwgttnnr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/ghllvpaij.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gtdnoqywn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gupphqhsx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gchiigont.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gorpawgpg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gkvrtmoxm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gifoioggp.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gympmpucs.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gpfmjcokb.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gcalbzgaz.sHtML


<!-- 参考信息 -->