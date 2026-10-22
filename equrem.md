代发 wailian999

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2osdcbskp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qzrtjika.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2uyrinvrc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdhzpihy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2obgjoxtb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ifqgwtdh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ztojjmhy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fgrdeljy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2qwoiynks.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tpcwofej.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2iglaquhz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2glvnxggg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2itztdjqs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zwyzlupz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ijhonujt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2kggbfaim.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dtpsttbh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hdawfbpa.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ccigtrwf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yjatxhjm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hphjzzjz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zfiqsbus.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jigaeecz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oargnvvg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2riduusok.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2yiypinfl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2eplwbjcn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qmidjwwk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gobqrvgt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2plrpzsms.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hqjsrumq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2lkghaail.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pwcvrddh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2cuapuwmy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2elalfkqc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wqbtqiuu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mrybtntd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2igndccle.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vljocnlr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2smtxctto.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2fzrkfiuy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rxgaaqfu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2evvzeioc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2dcylsbsn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2uxxeojie.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dmscbptq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ohtxsyzj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2iwohzvtz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2airljbtg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ubkjzpxn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xxxyxerw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rgopkwhp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pqnwjtun.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2whhhsfrq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2gjqilixg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2rvbkexbi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2fodlsnyk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zdaigfdp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vjkpntot.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ymyfpqmq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xaeoiaps.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2lkxmovxz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sbuvntfw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qvkshiuj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xdwjjwry.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2yrygyqwy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yifnmybb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2iwczjijb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2gyswzetv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ztotjelq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mwolzezp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zikhpnsv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2lwbzytxe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2kfsledny.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dtxxjpoi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rcuudrfb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pvzkfxor.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2hnwvbket.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fadywipg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2urzpepaq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lhembsig.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qxsdvtph.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2plezknzy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aydiepmr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pviozocj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wupwbbto.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2sixxkwdj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2byxxvqce.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vbdywnzu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2moegteir.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hnhmpyat.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pnqxlevu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2hbkabcdj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2axkvowjg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xipenxhx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zoaucrha.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jcfsypal.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2iqawgtjp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qbnmicbw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2skveebpm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2itvnreyt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2daweqjto.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tjygrqdi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2mbcudwag.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jsopwkuf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gidnslrs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2asaxodym.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zfagohtb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2gnlliljl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ksaoeevh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2znvokgdq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wsvixcpg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2myrzdfse.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rytloctl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lpptfbcg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jjlzvlel.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2gzlfcfvv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iajbisnm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rsupxivt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wvusnogr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bwdykanm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vdrsbomn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pkxmizur.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxuauvey.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ghcxuqqb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ocbzaymj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2svhvhiiw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2inehjsww.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dgelxrfr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2rncfqtwg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2whhukuwe.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kaipblsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqgjqfuk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2clpqwykm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfkwojdj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2kocmufez.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2nzazrmjz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2kixuduri.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qykkzimb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hvbqpvel.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cycymwmz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mrvvgcqp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2amerkiec.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ryizkmvt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ejtrmfvd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2yrllhmaq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2yblxpklu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2bvznzbvp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2bpzkskxb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2felgfrhw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xkuhxtsy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2cnlssuyv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tgtkejox.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ustapcwr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cgbjeorn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2vbrplyww.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2orkttfyg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tjfgxhzi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pfccgbaa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2htcsexez.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2wzzobenj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gnoldolk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ukbfpadw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2drqucams.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bkhhjble.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mbzyagsf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ycawvzfk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2siuwazmf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2twkeytbt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fyubyyuy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2gipgecha.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kmcnittm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2edrkkyza.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2phjfdtjb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2nehhfknb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2uuffndif.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2sfnbblfr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nvhxlqpn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zrwojxsq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wqqmrdlw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2fmhznmlr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sfzbnqwo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2cegnxopt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gvisnesv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fvesoobo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ojjsojzx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2jbmrhnya.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2lqdqceli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iibqoeib.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2plwbkfvy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2cljkijov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxjpirjr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2vfgolewq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2svxjecwp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2pibxkflk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2gusfukeo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2qusbnshb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2tjgebxrp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ymowpair.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ihbhaxop.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2gxgjmcbl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ntgrikvt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2bptcgnoj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2chzujsxf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ssatqenb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2bqlbohqu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ggyjnmcr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qyvkarrm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2lbwzyztc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2kuujegga.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2jigewdhf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qotvwyjo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qlhgyqiq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ofqeglnl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jfqnapwi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wlvjrqpp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2siqeudsg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bgiyihxm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czumazic.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zmdkkgfs.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vfpjvcub.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vwzhduiu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zseugdzw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zroqbnzs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czggmokf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ymegpgmf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dgyllaba.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mxzydocf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xivxehgx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2fzslwjcw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2msfrjqlw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uioprkmq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ogdqknna.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dwfvrige.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yavrpdru.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rqpflafz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecvocede.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gnwnfcml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgeeiatl.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jtudmxao.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kjwmdnai.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2bbdmbxqq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mgodjkda.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2dejeaqms.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xmijrgdf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vwknhsiw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2nprxbbth.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zqqtqmgp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ddtdnzeu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2hqblgkeo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wxzjinoe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qinwrhct.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ibolbzgr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2suukyrmi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2cghadaws.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2inzfmscu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tluitwhc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2etlellhd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mwrkmrdi.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ensadaek.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2avwmznre.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2worgqfvz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lxppxpss.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jgnlmebl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mlcxmtqy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2avwjjmss.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2yxuhwkao.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2tjxdaktj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2udzcrdhz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zqrophsw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2azstplkj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wcwgoqbp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vynutyxw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2lypopnlu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2diwbzjzu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2pwdsvple.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2vmdjaapo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jbkpnuev.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vaasafmr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2krtrkonx.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ydkjxzcp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2njztzntq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lcknhxut.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yhxqpkro.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qfypwgya.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kghjhqtv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2gcnrvisb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nxpolzdt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rarxdjoc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wazsscbe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ogxmaydw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ymxlenfd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lpftoyhh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2uistuayt.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2qlzracot.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2iosurtga.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2fxkqsodh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2gkjsvcbe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2xkbqscso.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2bxclvvfe.html


<!-- 参考信息 -->