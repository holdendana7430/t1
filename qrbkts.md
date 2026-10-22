代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2gydnbtbp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2jhcggdmr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ryivtimz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rubflagv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2csedtbya.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tzwuaupf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bnriwepa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bicchdfu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bldqwtyb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2afgwquto.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nykvixts.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pmdpcupd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2fabxlsqw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2aqwjbcmk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hdjzffbi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2scsovven.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2earsptet.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2cwyhokds.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2pwmtzndd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hbazxwiy.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2frnvtefm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mvjjvpdi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2srsqpncj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hrtnabnu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ojarslip.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrgcmjoc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ngerqqmz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zzhduaba.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2blpfxiie.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2gdkdjnmk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2csydfvkq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2uyhehwrz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2euticjbn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vtxtoqyw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2sgvuedzn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2hwysjblq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ltbovkve.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2brhbfbwi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2vdbhjhym.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2edumzsiu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ddawkkme.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uneqaedt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rdehvadz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2anzixexf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jgxbllwm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2cltldqok.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zsnlkiad.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2iuaouqwr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lfjgixhb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2pmlmlhyv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uhfglygk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hkuhzrly.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2gmkjkmpe.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qccppnlc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xskegkin.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ifgmjevd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2rdrqbrcm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2rrupoodg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hpkzprge.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gkuillbm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kwuuttgj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rdghscna.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2gdgknxnj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vpzxvica.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2djgqxnuj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2olhqczgy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ysmpajzl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2scouqoud.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2oueartty.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jjbosyrj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2tviomzjx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bjfndevt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2zquogbvg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ybgaxfwe.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wsopyued.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cbbvaisw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pgocycnc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2upiuxahe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ztqwvgqj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2slnvxyyv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jxagyamy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mbsdeokl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2eazcngnt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2swkpcspe.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lmxxqpui.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wwfayiam.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hwtggvnj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zglcumfg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vmiwsxre.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jhnlpyei.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ayfougzp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rvnyxeqp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2nrgdygro.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ykdfuwdz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2udmfkzhs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zxieonbj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2bwjltrle.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yrxkyxzv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vkmthjud.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zpgzxwlv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rhmtaody.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2cmhxtfmc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jsnfoyup.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2mcglbtjm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2czzgibch.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2krlruunr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2bzctebyu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2hvtztvnq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dayzpvux.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hlcthxrk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2mpraqkud.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gixxadzv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ngwtmrrn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qxkpfzbf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hzhjfhle.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2crbnkvmq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2linesezn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vdedeesw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2nvvyiseq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2nmqfjywg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wjkssqsd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxpaveb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kzyfndon.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rpoqnlkh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fvodmqhp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2clvwtuai.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2clnfpkyp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wkdcahti.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2egnqncxu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2okiufwah.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gchibxiw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dbiuaygn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ynbossam.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2efsupbpw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wmkgfauu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtqtdqem.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2twqietfe.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2apsofihc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nftswsqh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2veiyqyde.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2jlntjypk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2oqxifids.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rvddlvub.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ihfwwxfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zinvhazt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2sulawpmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmqcjhrv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kfbkxnnc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vumaiptm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ifzfzbqg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wvvvhcgs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2okkuprsw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2sdgvxyjm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zpgajwmv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2reyujkft.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2drrdkark.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2enpzfjha.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2iplfrycz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rzgnasib.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2mndywlrl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2mhnecfld.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gbmyurtt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2mxmgmqyi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2wpzuzygh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2truvbifu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sisqwknx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2suqfbtba.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ymqifqjr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yinrsxjg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lpehalgr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bvkxhdor.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2nlpegexz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hpqxfkwg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2htfnvwqn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xhwqnqte.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2igpzozvw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2brfshpss.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gjbrhfok.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aickowqp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bsrryhkt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qgxejwix.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ebliwrzf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bdymlarw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ntoyynpj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2lcmfkuzc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2hdbkmubf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yuezdnxq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ikggyfbm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ovpguhxz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mynrpfcd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2bdjqcbci.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2plpasyyv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2exvqfcuw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gghjnrvb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2uhoatdnp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2autgemhv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2swmibtbi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ycprkdpy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2valikxfq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ltahodgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yndtvzge.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2povojknx.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2hxdlhovj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgttubnt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jhqokjzp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dsuhduxc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2cykolenp.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2uojfpmtg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ochhadau.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2lrxuxqsf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2cblasysl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ylfekgiy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2yytahcuw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hpqhirrf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2fbajpqhs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2syavzjjc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2riqexdjd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ngoiyygz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2duhainwi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2phjjgwxj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2amvrozwp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2kkgmoejw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2uykuoqfh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qdrfvzfe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vdlqjjfo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2olhltwhb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tjlipfqz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ptfcutop.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jdkrnpgq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2forunaiq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nnmxllnf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2iamuwhky.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2mcgbxrtb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2oavjbdcd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2riskeavg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fmobzcnb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qslwtdpy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nbeghubv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yrypdgtn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mbxyhign.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eyhiseja.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gmfmfxez.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sikzuvik.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cjyubnzq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xnuvgvqi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2rrdvapxf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2argpqccx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2culmwjjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxdkpybb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2iybddeym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aukeykgl.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2wjqwouvj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2scmtpfxx.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qfntvgyt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vvfpfrdd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2kpwlurhs.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tvpkfotf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2obqxztwe.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wxxdjfxc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2plfqoroh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2rlksvjfr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2oogkylpo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2oxcdhavh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tvalxykz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2xvvanzqj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hxmrtgym.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2hszronwf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2yjjgblhq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ivfjpdvz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2opckfsxp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2pcmzlyrk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2whjohekh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pjdvoxfp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dlivdaqh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lbwngxey.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ztepggkc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2nyjzsaze.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hsmgzqoy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vsfeakat.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2fybqzzub.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2cwqlwxtk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xctzpfuj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wugwqsei.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2wxswqggn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2fvzagdpn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ccpgeivh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2majljscl.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2kpsxcqrv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2odujptgt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xsqwaihg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2srhnjbtb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lyixomjv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kzuhijxy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2perxvsdf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xijnrmkd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lslmpkmu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kivvkpsu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nqzaapuw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2epurcjfq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rfoxugaj.html


<!-- 参考信息 -->