代发 wailian999

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ycsuuiyi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jzslinaz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukdbwjka.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ftwepyiy.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qzpqrknf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2duunrpdy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2plkydoch.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2azenfrpy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fcnuciyd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2acnlefhy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wywpcsyl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uunbkgeg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ncwxqmop.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zolizqwo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2txmwrsoz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2whcduceq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xmycrhvb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iuufxlqk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gjpaworv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rhjvyqrp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tbpsfjgf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qzyracrz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2seddypwk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2tcnyqoin.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rpeakkms.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2quiyjeja.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2owledvfj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2yohovbkm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hgmyxoyx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gaykomeb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xkvjwhql.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2nlpjcmqp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jygjkfvq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cgkimheh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2sylmzutj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nbhcaipq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hbngdiwl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dbxpuiwt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qlxgotiv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ncqecnpg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2usxyflvp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2uyespmxi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ujawqptf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kqohoqft.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mheatucx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2utsctpno.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gzkxijiy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2uznnenbj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2jmzoafvk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lgkwwusy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2lmxvvvmm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2sjzpjgjh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pcnbyawu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2pfbfkymz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2brizgvhw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ixneynlo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ihvixfcw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zhycppog.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2eumilboq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dkxnjfqp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2qylimjyz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2lhzconpb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vnxorhyz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2faknyhol.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2vdmhtxct.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ysuhgtpo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2llehsuec.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ivwtivha.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2mybvuwpr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2rkymzspt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2seojtlwi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2olgpuyfb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2efkmuaag.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ebwcqfuo.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qckpxsjm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2akpoesid.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2wdrckmsn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vqisstio.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2akacfjng.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vtfbpyty.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cyoochga.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2uiyfqhlb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hcjduejv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ndqccyod.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2woqhjdxl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pbvcujgi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikskjyzl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fappojbt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hpdzzkzl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hxenlwpl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2hbznyryq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnkvkuof.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cgugybda.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gujgkofh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zdnmjskn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rpdexbey.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cabmkarh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dylbkptm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2vjzinpcx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dvddieeh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xhhjqqiq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lnfiucef.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xuajafrm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2grdizkjd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2bvrgdxjh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2zhgskven.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2zxjgttqh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ftxurkiz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qpzllsgr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2psaleqmj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ldkrdcdv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2cyiycmin.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zhrivism.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pdibtdab.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kvgwijix.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2pjymxtxv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2bmulpkjb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2csctvrdb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2uckulgzj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2gvtkxbez.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2robsmyfy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nkybpdvx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qiqoaipm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zmgkhsma.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dzxotwhg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cgxwdjzn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ylsbqyxv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nkmdsgst.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jjfwcuxf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2teyejodl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xmwaztcl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtuluxun.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mkiprtbs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jdvktgjn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2meljmmlp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2bujtgcof.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2eziamcvi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2wnwmdsyx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wbbxjzrc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2awwqzrmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogvtgojs.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zzfqxfpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdgvbujk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2aladyhyb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2uzgqzebl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2reuhhnqn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2breytgsp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hzoodzde.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2igowggjo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dmewejak.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2juohnoto.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vixcmcui.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dceuzbbg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2yncvwdis.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2yzkdfhxz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ugfbenaj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ccjtqzgg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ikpnwbbc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2yqqjktov.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rfdxwohm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2tliysyez.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2altxmwut.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2nsudyegm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vsyisqrm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2sdadjlau.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ofzefywl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nlvdvhve.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ubovqwsg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2gdypyjps.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tvcaiwoq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kozcawlj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ovooobhn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vhctutgd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qpwmtsbu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cudevzka.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2durezqoc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lstaunmh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jcdfgqyk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2onaazdno.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2thpbgqtz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2wqzhteiw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2vdhrkqug.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fddaxtcg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tbrfdvtk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2juwtyzdr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yjtrmeqm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2hwbfjdej.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2evlekozq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ybeibdlx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2psvsqptw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2xxxysmao.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2zjivqqkt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2gdtnlmwy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2pykehspz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2atdjeufd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2vztwvymv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxlbvcbh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2loyvvltl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2vbhndiyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knpoifij.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2towpyygh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2wwtrmxfq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2epxlyvuo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kqhmunkv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2offzsgfg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ufmbwnoc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2bttpblbm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2swvlpkob.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2yemzrfjr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2pexoixgi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2cyllqzdr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2uodpgwaq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ttrbynzs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2hvixboyw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2gsyytppv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2lofhzcph.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2aydiwytl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2idaorvxr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2wcljdqjw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xnssmnwx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ojjclmlw.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2bgodczel.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fywlionf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jfutpvhy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uulgdzbh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kqhoitha.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2slcoovlk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbwbvdgd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hogaayyg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dtxpoyzm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hsovzcbe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bllwgcww.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pvbfahqc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tsxeljpx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ytcgganp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uhwtnosl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qozxvzxd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zublkmda.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2skbkojdy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jsstamjx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hvyaeijo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dktymzzd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bhlrxfka.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kmrrkinj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmexvnkq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2fglbgdyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igwrzdzy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ebqredyc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gebwhwmt.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2nrgczwhg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nyvziaus.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2bxhpliyj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xegkhutw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rfrzkhkm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2juiwbrdy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2anhiyglw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2eqqaaxaq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2msnbslqq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xxwxvtko.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ajwjzdrc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2kcaghnmr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wdmlxfjs.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2jwwnjtiq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2xvuwcvfr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zafnlzoi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2wngjfpod.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mwoqnnka.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xchwdoxb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zdabzctq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sciydzxx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2awgohaxe.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2yvlddcwo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2orfbyzzb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2otnogtpc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mjxubyvz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2aigujwou.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lobdelhv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2epwummwa.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2frqhgacw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hcrwewfr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ktkmjokw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ihsjqcda.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pjbszgoq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2vpxgaisw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2lnjbfewv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kzqchwmu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ibjqtdgu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ohvtsaln.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yagkbirv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dycrnrjx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2muclpvaq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zpiiocch.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2arkwxclp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fsnpqedu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2bejphhfn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fibbogux.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lhidunpl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dwhmucvb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jbfrdoyu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2omzdtgnt.html


<!-- 参考信息 -->