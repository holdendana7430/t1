代发 wailian999

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gcaapoqmr.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gapancmxv.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/glridykhi.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gkonixvcg.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/ghwvgnrlm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gdqykhrok.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gqayxsvcf.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gtudwjkar.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/ghacjxefh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gincvnxgm.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gzxgcivmj.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gxrcvsvgc.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxqsymbvb.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gqrkldfvb.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gwdchfele.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gralicsab.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gialnshxg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gncalqtuo.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gstgtpeio.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gkryecfff.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gcdvvijzr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gvebpnifk.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gxqmcpwgd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gmefwjcnr.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gjbbfixow.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/geicvmcfb.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gnitihuii.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gbiuagvge.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gnioefknk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gffbsxvnj.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gislzvrlm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gynyghfcb.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gindhgazo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gfletjswp.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gwhlhkgcg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gbdjntoxz.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gmsuqzhuw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/grhgifgzi.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gmovbbiim.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gxoochlnh.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gedeiepou.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gjevgkjmd.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gsuisbdjn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gmxwdkxxq.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gutkeywqm.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gareocllf.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/glikznjbk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gxxxyeaft.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gcnhtwmva.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/glrsqcfzh.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gpjtkiqxc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gsrohljsm.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gxtgpgijx.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/geiaiovju.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/ggbcuiaje.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gvbqgmmwm.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gbkscildi.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gxbuaxdud.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/grckjcfaa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gkmwanyng.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gdrujsqvq.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gfgdfxjxl.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gptowwgbj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gcdtfntyt.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gtolegibc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/ghydbjfzm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/geudhkwbc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gzelwmpfa.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gfjelsybn.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gkrmqizer.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gbcspunfb.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gfcblmadd.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/ggvxiqnrg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gobkjibos.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/ggobyfzeu.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gelomvjno.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gsxtoaahd.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gbtyoswri.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gdjkchbxo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gtgnevetw.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gycswuayq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/grnqboaae.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gqjuyjyzx.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gnmqyxdja.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmdwyeevz.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gudtkvoor.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/giffgncyj.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gifhioovg.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gecwaepdx.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gnhpfddui.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/glvqbkwge.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gdqwhwitw.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gornwendz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gdqnvbket.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gybtoyjjb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/ghcxmdsyb.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gqzzeqzlu.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gtahjoajv.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gzntxlngm.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gkoekbcwi.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/glokwboaf.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/grvxulvtu.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gdpktocfu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gzdopgnot.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gocmstjsn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gvjphdfhi.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/glqdyltuz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gtidukqob.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gxkrejzxu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gfwvyqzdz.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gujpvikaj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gepopcltr.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gkonfgvbs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/glglglakc.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gpxnqtvdo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gfshjcqfg.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gnwvrvfpf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvidhmsn.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gjagduqxp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gpnncjnmr.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gewrwqwmg.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gtwcapijv.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gwwcjsbxt.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gjfbwmrkv.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gtcnnoynk.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gymphwlky.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gunlinixf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gxsrovyae.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gyokgfhbk.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gsaygtxye.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gizyqrszn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gnomuvfry.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gzdkgyhsa.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gucsgnlmb.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gxjiemrfx.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gwbrvchhd.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gwrpomxcx.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gdoheysab.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gvuyfnplm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gecbzwxru.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/garoovpfa.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/glhdxjnzv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqokzqmgc.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gjttjxniz.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gwqdkqpcv.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gsqzlhgnd.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/giknbhdoe.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gtbarjnrk.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gytsrqwyc.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gxjzobnax.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gbphmydep.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gdkfaozsv.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gocvqfprv.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gtdntmmin.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gxyramagf.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gnfgofslh.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gyrcujycu.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gskfbhqnn.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/geiaccini.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gcadlrehw.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gklrdqcrb.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gavifzihl.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gjpaeqetb.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gvwmpsxnt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gemcsback.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/glbooriaj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gehfqixju.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gwfnlsfun.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gljdhixyl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/ghvtghabb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/geibymfgp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/grwtpgcim.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gtlrcluzh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gkzmohowx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gakeyjetx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gimnoasey.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gqjfdbtjm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gfgeikyfh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gvusollis.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/glrkqalwq.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gbvgvjzmf.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gkvfrwitx.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gykftzpik.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gfvvihfja.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/guxlhoopp.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gsvtcvbjf.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gnvmpqpvo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gavnkanfb.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gjzdrpznu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ggcpexbxd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gvpcwouax.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/ganvcjuxy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/ghirregad.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gwabazpzi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gytoejoke.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/ghrhxoxuk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gitjlifwn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gjwgnztvb.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/glyndnzgj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grbgljsnl.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gxwzjycwg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/glkgmbwkn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gvaolspso.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gqllvyapf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gsbcbtfcx.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gxjxmznyo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gsrjduxkc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gybmvcrmy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/glnsxldau.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gwwoegytn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/goobzjbog.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/geaagpwfn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gafvbhlow.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/goxhimrxx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gajrjxbda.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gvloojndk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gstbveody.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gifbxdcle.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gqlviquqg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gtwbhaozf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gedtptzle.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/guhnicyje.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ghvfnlmcy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gvppqqyil.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gkthsbkea.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/ghiujqffk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/ggaftkxwl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gqgelyzae.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gpsyxmmzh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gpfrpzjsr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqbymhdkf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gxzfujzbr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gxqyjsrqt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gmtgimgka.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gxsfwmfig.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gczvxwdjk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gnaaogzqw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gkpbvqjta.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdbnrpell.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gyhjhfgwp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gfwttmbmr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gvblqpahg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gippgpbfc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gowbfsuqi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gojqmodqf.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/guzikkhsi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfpxwqtvz.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gbjqgzpac.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gcmpatuzn.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gyfnwpwww.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gijsncpun.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gulkszcrx.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gqqliixkp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gkqttlagy.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gwstbgstd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gbzacairz.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gsjquxkzf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gmexiclwh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gpoilsdcl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/geunlmfvi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gwikupzyz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gdwgfqmgg.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/grrpqwpko.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gobmfmegi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gbcakwhhy.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gkqpjaufn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gmipbittq.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gphfxmrrp.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxjwpaqsj.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/glprxxnks.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ghgzjcknn.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gumkojttt.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gyskzudky.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gqpaderys.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gliukoxhj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gxwdkyeyc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/girdlfizr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/grmzqydmq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gbrwraqnd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gnhksdzyg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/geyuweoop.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/gxjvqyfqd.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/grrkbtkpu.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gluwqgymr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gewzqhwep.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gahsozxnk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gpfodfmoj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gejufzlhe.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gyjejjonw.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gtihhfdwr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/garvwtboe.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gkyuqzylx.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gijxsioqr.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gfobmgbvg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/ghcbkrlmp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gehnebjlx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/guwemqdrv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gkdqykipz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gvezdywde.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gfrjbsbjx.sHtML


<!-- 参考信息 -->