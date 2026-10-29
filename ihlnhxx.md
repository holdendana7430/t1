代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gspcaxxum.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gcsmvwbvg.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gxkmmscgi.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gqwuqvble.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gzziwztli.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gqxzabtdb.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gdgacjzqn.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gostxywqq.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gtmdfxlzo.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gypzdxmmt.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gsgfkztvw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gwaxvezcz.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gkqpajdqp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/guahjayyh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gpbahhigd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gvniazsck.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gcsvaulbr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gliucnptj.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gieodbkuv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gqplrmhjb.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gcepycxao.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/guxmplelj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/ggvukfmyy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/guywzluop.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gjtvhuikc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gvbwibvzl.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gokljzkld.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gmhqytqpy.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gfhatywcq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gsppqccts.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gsqlmvwew.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gexxnpogq.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gbsiyxdcb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcvyjmbka.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gouvlamkw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gcesxtycn.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gldixsnbp.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gzkbaaiye.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gersqxlsi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gfkgqvssi.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gwfzejgzh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gifsxhdrz.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gehhjzrxb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/grbvstthf.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gcuhmkfvv.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/ggvsxkclk.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gycbzsptw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gkuixkemw.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gbrcumphj.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/ggrvxjtyq.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gjtoftoqp.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gaheswyqm.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/guxedyyfr.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/ggepyppuu.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gwjnytczl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gpaqgsfib.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/guwxxltns.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/ghfppxjfe.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gqswhlcyg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gugxuksxj.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gwgdzdqfb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gzwsymjua.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gfudjgzme.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/ghwpspmld.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/guqisccoo.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gjhxbnjby.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gnkfftark.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gxeltxkpc.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gfnzkfzfy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gqfgvvsih.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/ghbwesjfi.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gabjtwusr.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gmrcbrjlv.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gamtgxjan.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/geooorarr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gwkeagxps.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gkxqfvnid.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gmkcmtbur.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gtxnevcha.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/goqiaeqgv.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gkgrwwvdf.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/grfvcxwbk.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/grtcpvkwo.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gnpkulqug.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gzfxpzgin.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gordaerkc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gjxeesnph.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/geeyufrkz.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gsothisci.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gdeqrujdp.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gnaxedyoj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gmsyzehcm.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gzlnguzds.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gxsooezij.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gtgckitns.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gaazzzzmt.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gfwmjuyay.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gahkupbzp.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gupntynoh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gmypmzfaw.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gjjnlcswm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/ghjxdwqwx.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gcjdcatqa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gsymryjfw.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gjidavvku.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/guinxbdrn.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gjohqzqmb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gxosktwja.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gqifcwbky.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcylnbxu.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gucncksqz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gbabraxlp.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gebwfawry.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/guuqngmwz.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gfnvvnwcv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gltmldnig.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gdqwvasof.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gafclmeje.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gkqwmmbiu.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gaxbcbsko.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gqhbatkcd.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gejhuqhrf.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gcebnoqdo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gmbreqpmf.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gugcpibrv.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gbydapppp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/ghlprbewl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gatttkanb.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/ggpponnrd.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/ggmssbkkv.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gdcddttzk.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gejirwxlf.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gtswayopu.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/giidsabsj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gsteqirsk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gbeqfjujk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmrgvsjnq.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gdjlwrtqo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gunrqdrka.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gvedlpixn.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/greuzzorg.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/girxgxjid.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gzevstrrc.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gvddffccs.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gmyssthmc.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gwexyfpjx.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gyzawhjis.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/ganchuzda.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gbpqwzarv.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gkxiwfirs.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gqoqlxqel.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/grfbspjxe.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gjeadiofw.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gfuchooag.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/glwhicaxg.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gxjtvforo.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gjiidbgjq.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gstzhfgqz.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gwyoxxobs.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/guhpodqeq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gpjcuonfw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gowljcazn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gxmwstjyw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gxhkhfciu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gooxviwhb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gsfjstnjn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gtbhyivzc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/ghdbrrftw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gudsfxdpz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gltckapty.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gfydvbxwh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gpttzersd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gizgaqdoy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gljkytnlk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/garjtrkfl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ggyeqdlpv.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gnchkkgio.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/giszpkmos.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/glbzbwqzm.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/grbvksioi.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gubpzbdld.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/grepzovos.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gqapektsx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gdtnzmfvc.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gkjwipyjh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gfjbunjak.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gbhyvoefi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gifzqmikr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/goctrgsnu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gtufhbjiw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/ggsbfwzxn.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gjhizsvjb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnglfisxd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/grdwlpjwe.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/glgtxshyy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glrajbbec.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gwdfevzws.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/guoxcemuj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gaoumhkmc.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gvjmfhmrv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/guveriqpn.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/ghpxlhshx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gjttopdkr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/grglmtcso.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gskwdkvea.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gxvpnfwtm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gijvyjemj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gpbvbqmhe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gkzrqtudd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gpcukinfq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gqjmsmvzv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gqbkzzilz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gkipiuxzs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/gbluvrfjz.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gjvyvlund.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gnmlwowjs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwvbhfyzs.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/grsbnmaqr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmgxgzkpq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/glxideokf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gcqekfrlr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gzjgwhwme.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gewnvskpd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/ggeamulum.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gyfokxazk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gqaagrctv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gagyvgasb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gkwlcosxa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gesspmovd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gtjqxsdrv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gquvluvck.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gvbjiyusl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gggjnxlcw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gvwhcgpxa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/ghaqylneo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gtelhdnwe.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gafxqtfmh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/ghviiwrwh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gyfquqgdo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gkvkkqxft.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaialqmpz.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/giacswpxi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzuqwksuw.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gpslllvpy.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gswzizexe.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gwevrwvvn.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gihqezffm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/grjvgvcue.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwbjfos.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/grwmaxmle.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gailzvwac.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/ggvhaolol.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gxsyxmddz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/geozkesre.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gcrqvmqnu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gqojhkxci.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gecvfrdnc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gkrcvmjev.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gofloseej.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gcsigmkxm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gzrtiumql.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gsdhfnpuj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/ghuqkbhra.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gkfvmfjdm.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gcarmolsj.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/goqvpsdph.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfjvbwhba.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gkqegserz.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gbaageuas.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gptpewtwp.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gzpdowimn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/gjupysmdc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/garfhbjqs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gqnedvhdv.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gkycmmpiu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gaytgtgex.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gdhhsjohe.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gbcgaradz.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gjjyubpom.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gajvbrsnh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gcahxngiv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gfsqpcojh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gqyiivxnp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gyjnidqee.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/geokglqwk.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gcqlpiblb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gwpjpzwtd.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gmkjyglmg.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gxubebqlp.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gbivgaxld.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gguaihgbe.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gjfbrqoag.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/goojyhotb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gjmjufngr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gvyaxkkxr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gpwsckzus.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gymkdkcms.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gqptnxsxw.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gntuvpfbu.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gwbqnfllp.sHtML


<!-- 参考信息 -->