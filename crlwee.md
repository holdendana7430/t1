代发 wailian999

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hwtqxoew.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3umyobwne.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3eltnlfrt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3repzeexq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rzqvajyv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3huexpxsw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vlknvtzr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hhgjuzvh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dyzrctix.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gpfhbjib.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3cyzsupcb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vqflbzaj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qahtdixa.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3asaqjoly.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wemehgwj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wrlicmmc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kwbvoban.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oxrntinp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3gqnsndeb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3oflnolff.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3otlwsdsw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3movjmsgk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3soqkvxqd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qhyrpmnp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3mwxltmsm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nffyioav.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dflfphmf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vtsvuuaq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ewdrljzo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3skapnykc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3lyuznmtt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3iqroectq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vmksewlx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lpjzwryd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3rmysofcz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3aeecmjta.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rudapulo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3gdtjqnfi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3imrhcgaf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3hsapctom.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3giuckahm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wdewmtui.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3detkssps.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3uciweyek.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3eiwjuyje.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3sjbacamb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mzwdzbbh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3awjhvkua.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3haxedaha.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3uvmldlju.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mtidyjia.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3krqvoksa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3kusiaqmz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qgqfsydq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dimtnouh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ucjgkcuw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3drivfqcd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3shzantta.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cevtoyck.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3egkzenlz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gotlzpmg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3uablhyic.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pgirmyrt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fttguvjp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3tdriglcl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gtfcuijw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3mghudwjy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3urdjsowg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3bvnlnsbd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jhncavze.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qeqepdul.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ivedxaus.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3aqlfggow.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wnpbyfek.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nlkuiqhx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ndzmssrk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3jihqbmzp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iqrqwodf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3tztkaduk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qjinrfrp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rzlxaarx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vzuklwsc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nfyyenhl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3srqwgroq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npeovijn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gzlnmnvt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wctyydvt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ihtfdiat.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3llegbzvq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rvpopygf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3chvspscr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zoofdlmu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3bwnfqnfc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nrefsyle.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xoqtzeno.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3jqdihlqg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3jzrlprfm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kvewefnv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tlezyuyi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qiuijyzi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qswuiivu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3aiwffmgt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vcuolzss.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rlchzsyu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wxbxsgpc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3aibfgmxk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jsfbjsye.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ezaohkrh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ncifzwdc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fjsakrue.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qtcbwptm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3yrvmlslt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tkamlfam.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qzgjyuoo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3trsnkbjs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3xsabugve.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tyibsihu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3eicgnror.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3shumvnpo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3kvgmwlrs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jfegznoj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3sxezcbfj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rittdjdx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ifsacdtv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3krtfqled.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oxfykslo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3sekkevyc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gvhnjyoy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nhvwqpqv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rldtdqyo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3kcvfyjdk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3djwhxlbs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xwjkncjz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3agbbbbkg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ynqmlqhk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3yujhjwwt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ulqshvmi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rncldijz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3unssgrjb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3fshllydh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrtagmmr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ivjelyru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqiirvpu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3fzjzazmh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3yrzesbhk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ijqctvep.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nwjvtydq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qzpjiivo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gsrrousq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cbpxhhne.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3evnbafqj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pvbzcdcy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3sboyyrom.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3msebbimq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3diydklib.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3mrgsywax.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3npnhybmb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3tparggbj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3klkgpkrz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pioahpol.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3fpayprky.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sqrslgyj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3eiysnqxd.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3iqevsneh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wlunqnge.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3blihcrri.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3znmbqowq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hvhttxbg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ighxolqd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fadyfogo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bklladbn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rqctqbbl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lukieyql.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nmygbriu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3twseqnot.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ntlogwtw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vvaqlpmw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3swbribrz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3wmybwnod.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lbreqjdi.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kiphcjzu.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3uyjepwqa.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kywhdxgx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3zduofoic.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3tefommam.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jvhsnpgt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3oanlcyot.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ukvudpkh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3isfcrgaw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lkiygryw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3cvxsoqhd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3zjgypwuv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3gywfctcz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ovdcdwjm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ogdxwqae.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3dwomwxxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obqibnia.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3xvsagact.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ptgwaynj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwptepcl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3oxooklga.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3adudwvpm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zelircmn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3efecssbt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3xfpltsbz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3bmfaubnt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mmxzzefu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3vcurccrd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3xmdsvpny.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3zayfdtdx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3prraxlnv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3oiavkpme.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rveymnva.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3athkbxcu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3jfoqknnc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3nwircarj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ufctybwp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3eatinwcd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3eczulesr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3fpzhjwya.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ogbwilma.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3vwiqwazt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mpsaqrwz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hucntftd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fuuuzoxl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3evxzwcbn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3djijoult.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3geyjdydb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hamryvyl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3awzkmcel.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvaxdkek.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fccvowco.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gtqgeabw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3suoiigpi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tlhfrdbr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3whkuwmzl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obfnjext.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bkxevavy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ijahmpgu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ckzmjqsf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sieorryq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3npkvmdzc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mxntqsgf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dwpocwyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdjxeiiv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ptvrijwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhdyyzjx.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hvuludwz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ycmriwdp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3symqeqll.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kyjhudjv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3tdgscfbh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mmagwdby.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3phagirzt.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bwpvpggz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rluhktdt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3bxbtryzd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3wvhjpdal.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cjlnrwos.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3adzlfqbr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3krjfnobf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3darqseae.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3swuuzgji.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ucxfslso.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tvdvltyh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3virigvbc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3yglgdnvz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nbfybjky.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qimwnzbk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nujrugwi.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fngbxgxt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3nofdezch.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3slmhqqiw.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bqsdkcqz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rgtydeqh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3gnmkuysi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3lmhdbeaq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sahqazdy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kxctamtd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3rqugfgpl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3uadnzrrk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zxqxujve.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3fyhflhjg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3xyxlbguo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3rfreblvp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aybjzfxh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gmkotbwu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mhxyllag.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jisoezov.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fhxkfogx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hietoocc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3frviqmlf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jkrubwvb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aetwdcnc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jypnovhb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wzmqbgoo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mbuiambl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cwnvqwlg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rhqxrjqg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3eecsfccx.html


<!-- 参考信息 -->