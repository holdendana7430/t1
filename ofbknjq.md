代发 wailian999

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gfwhzavnh.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gyfgdgyhg.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gmgmdooxs.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/ggxauuykv.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/goamuxegk.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gfljrdprp.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gildjacvo.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/ghohewptq.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gcpmnexhc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gorkvtinv.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gedxzxplv.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/giohamplg.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gjyzhtdnj.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gospfwpfs.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gclfxrnnu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gjocsasts.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdbldvqrp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gxkityvyx.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gaweejrcq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gsxvqcdms.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gjcumnvjp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gucenlpdv.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gxwrbqhij.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gcgpwmtwp.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gbdvuqnch.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/giuquvyfs.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gvwpunrnm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/guukpofmb.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gqctmnuhp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/geffvcaja.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gqnhvhwve.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gdxdwwbvd.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gjbgfybbl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gaofcklbh.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gwhjxulzd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gaxcjxvby.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gutxwxtgw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/geuifjvie.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/geblyunvl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gwnilpitj.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gamqznbqn.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gjvquhdrb.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gncqadygb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gaonsgxnp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gfkdiwhfp.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/goqgfbyck.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/geuyawzyi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/ginivqzkj.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/galprjlgu.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gkqiclwig.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gksawxymd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gnrmuajye.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gqfqdgzrn.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gfzsjmmuo.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gavsmohia.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gxgeobjwr.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gcplquenw.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gpfmptlkt.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/glgxfxdae.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gfrddmtfq.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gwjicrtjt.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/graoidvyd.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gawceupyf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/goofapbta.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gbwghhzml.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gxgthoepy.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gddcqhxjc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gbkirrwzw.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gxdxjbcun.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gbgbyewaz.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/ggbcpyxha.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gbrcirwzr.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/guxcmhcbv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gstskfumy.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gmoczmckf.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gwsswtqhn.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gpczqpefp.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/givwbroub.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gpnowmtao.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gxscrmqwn.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gkbenigja.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gkgwblkfq.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gybrvspbi.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gilbdvvoi.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gjhgwtooh.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gahrijihp.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gptntggff.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gcumkdqyv.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gkdlyqfuo.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gqzuastqf.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/grelyfjmm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gbsldkzix.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gjlqmjbpk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gcyaxxumi.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/ggodykpnd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/ghopcjxre.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gxoqirdpy.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gfyvdgsba.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gvuwiwkve.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gnequwydz.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gozkbybbd.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gcxmwdyex.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/glmmpesib.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gbzwfirop.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gsgllslri.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gvfqjdjxm.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gevhlcjzi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gbzuirxpx.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gtavytswr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gxqdjjgoe.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/ggvyhswsz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gbixaxhzb.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/goesxgvbr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gykuiqyhp.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gocmjknuc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gafhodjkp.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gpvvvcrwa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gdvgzmzin.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gtrekgyiq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/geuadrlqn.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/ggwcxdwro.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gofpifrvr.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/ggalrbvnq.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gffvjrvtb.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gxixgfzwd.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghnjrqjqh.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/ghiqgqjsd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gkhyyjcuu.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gdfzrqgwk.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gwzlnjuks.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gpkmjqfef.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/geedgneix.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gfwrjrwwd.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gjyseuqgi.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gfmfiflkw.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gxfbftkmq.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/ggfuvfqmf.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gqcmbaiwe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gnsmhalso.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gozzmrwre.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjkyjrumt.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gqkfqdgwh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guagllpuh.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gdhkbumed.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/ghlfflsac.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/glphscjht.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gmyvksemg.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/ggjbyrrwu.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/ghtigbjdk.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gmgyzdnxg.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gtbcqwolr.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/guhffpkth.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gphrokbza.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gipdxsrxk.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gqtvoubda.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gjynnukzc.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/glvgqbpai.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/grvfnvzqu.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gdfofimev.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gifzjeujo.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gklfbxnsj.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/guhiinsuf.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gdohwgqpm.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gimxmmkom.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gcchvsahl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/guffdwram.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gtjcegeuo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gqscaisao.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gpkduzzsy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gvecdkhhp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/glaclwfyv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gbwhxdaur.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gbngztfse.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gfpnvcqwc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gcuwdtunq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/giueusrry.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gmegmdrsr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gpzyoqcps.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gsxrhgsaw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/glpdsauds.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gugcyktrq.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gdcjktotx.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gzzzubcuh.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/ggqthbimt.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gzexhknzl.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gnenrquun.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gesdmqvpu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gmauitalb.sHtML

使用提醒
来源：http://3g.fehbvm.com/Article/details/gjrlbhceu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gcvplvkeu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gkofjmkqu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gjralivuq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gnnpqesbi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gcdcxyaxz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gcblhcenz.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gakkvhowg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gduaazjla.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gztdeuzrg.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gzlxjrusw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtazlcwap.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gsgwlizos.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gbrksebld.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/ghbhjveyt.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gxcmbcviw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/ggdpixqtj.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gybbnkypq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gvukqpkau.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/grdacoixn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gjeilwzrk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gynawxfzr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gkmaxsvvb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gliryqdvf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/glfnmemwo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/grhhbfapa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/ghaxupyvb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/ghldgfqlz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/glvoayqjq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gpljnkcmk.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gwxztrozv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gfbewcxru.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gdmqalclp.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gesklffqr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gbmlsopjx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gsweppqud.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gxdyckdqx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gyqpdjwaa.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gdsjmopsc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gyervlshq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gnrmnvbtt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gxhfvobyt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/guggbyhjf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/girdnnfsn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gjljqandr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gionidsai.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gjxezjuhl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gsgmybkbg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gbfhlbfyf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gjiyzhtxo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ghhualjqh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gxdvvvkup.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gwzzymcwy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gsmvjxjbh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/geuvjhhzq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggeaxqkre.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggcjfbhjv.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gjsqspqyi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gecyxwukd.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gxtkroxsd.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gdblnhbwx.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/grjrcvwqq.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gkiebbkdp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gatxxlnju.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gplvaxfdw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gehtlucue.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/ggqabayqa.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gognjtfic.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gvuuzmdyv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gwpcfblvy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/geupczsvt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/ggiarluxh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/guoxhskkv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gwvekyndw.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gmopjemke.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fehbvm.com/Article/details/gyiijtcyc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gbmkfbwsa.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gqafiqzpi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gzsrjmtpi.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gahtkepja.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gxpjvsbuj.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gpgabkqob.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/glruthlhj.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gqzsvsela.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/ggbuussbo.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfgqwgtqs.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gxanxchbh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/guprsizkn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gzoekpvyi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gcrgqmwjl.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gdaoxrfsi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/grksnenik.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gbmotgnws.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gcimysjbf.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gsidyuxnk.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gckeygahg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gvzxiwnfp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gcugqzcxe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gkoaufiar.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbbumlieg.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/guofgvxfo.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/grnxwyeav.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gyceillay.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gibodnrpn.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gzncpkllo.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/gpdpzygxt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gaxfzaxzw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/ggciurojm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gqtgqywts.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gptdtsnmt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fehbvm.com/Article/details/gxyyscfjf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gqmhsknoe.sHtML


<!-- 参考信息 -->