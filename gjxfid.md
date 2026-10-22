代发 wailian999

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ejibgnqm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wvpnwucw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2euylzbzt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwmyfibb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qvjjxlyq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2jogteuec.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jzntxiqf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqmudmxo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zokandvf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ndxyepdj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xgtojtxp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zhwhiffc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2rzoegaab.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ckhbifrd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2uwlsqugv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2cyogywhj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2lvgolwha.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tevyqsuu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zzohdnnb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hhtsjkdu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tigldsvg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2hwbfxiny.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lynhfidp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2sibyqvyx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2yvykhujx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uvulphsf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ggukwjfj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rqxdospk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mxwnvzzs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2sxhktwav.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gximkiwq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2yvldorxh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ldshaycc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dimrzyvu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2tajhflcs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ojkndrph.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xcnnrsqo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zldhldtx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xrcyzuvx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2iszbhauq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wrmdupfc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hctofugn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2wfwirbot.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2sihidzta.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2snpfuuty.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2hiapvmlw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2sjetbgvr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ojrzeiwh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ishontce.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kxszyzwu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ksyvpojf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ajycocgj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2sbgrdhng.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ppgriloc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2susshsix.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mivmvphq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fnyohata.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gdszkses.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2cwhijkap.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2hisawcxk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mykpjxax.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ainnfrrf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2grwqdqxg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tizdrxwf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2svznahfa.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qqjlnmbd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2fjgccdrk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qtjbvvvz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rfpaopfm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2olxzjzzd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2hzbqozcy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ucimmrxk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2wmnjkyvu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gfnutrfq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2dzsszddx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2rqsjntrx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2huvyysot.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gqovqmob.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2czqnrnkt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ajpougho.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2npuagxlb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2exeimatg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2eakgnclj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nmubhxor.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nvigeare.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nwksprii.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tfcayhci.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gxypjktm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sbjkbfyz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2hrhagbyw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xhiqvsaz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cocdikch.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2httlizho.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2edfusifq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2aajjihev.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mlvidovy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2fxqdslyf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2amyzvadp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2cqlkibst.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2txlzlusi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mrmpncup.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hwqhhlco.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ymzgxxir.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hpryarck.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2bdxuirgo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rtjhjvuh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pjjdsayl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lngzkcft.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2jfmqemjj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2htlwludr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2dwivdcvo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2brvzgrrz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2fxnmneyb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2myhebcbz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hkhkuurc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2flpdudvn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2uattdrlp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ykgiiffm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zpeumbyf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2uwmyifog.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2aajzryeo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ogqcwdts.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wicyzhoq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gpndxhyv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hvsvnepi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kjcewsmb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2dgkaaqgs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tqpiqelf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dubvhtco.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vysqyhhd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zpjigzxt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pxgfkumx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2cpbvbcwl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2klmcumyl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rhirrbgs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kjcmwpev.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kaynbxfc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bnonzweq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2cuiimzzq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mdctvkge.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ycuudjjs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2vgkxiqck.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2yxkusppr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2drrymtwk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xnkbbdua.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2edhogbmw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xiiagyeb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rixhfgat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hiosqatm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2pwdkvcuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xehalzdc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qbgnupdy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yywkgupg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2rkztqpez.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kwyyitfp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ahmunxks.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ipkpavpn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jpyhkhzj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gzntngrd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mrsfjliz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2htbgcgmp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2fzgsilfe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2thwfxiye.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2dtczaxas.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2aclxunjp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yhbdlxvt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ckhonpji.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2iekbvuuc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2phxjrmbe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rbcjplej.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nlrwgyew.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nobzmyyt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kqdvgmqw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qzyhghve.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yiyrryxj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cmofpwia.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ruimywgs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wlhhxejc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xrygdjlo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hifwjvqb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uxydwojt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ampvgmqb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nqaxtawd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2okcbzlmb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ybplwczi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wpdpdqye.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wltziokk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vygumsxe.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jkdnhlch.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ocilqqeq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zhxixepy.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dezakbuc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2dclhffez.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rgwlerlo.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2dfdsizfq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qmkbbmoy.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ieqiyocs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yyzzikll.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2cltshlnc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2gqmsczfe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2rncaymnd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2necmpkqx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2fvihbnxu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2cfsbhhdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsssobqo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ldcvuack.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ixtijnln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhuhcwlt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2aiffooqn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2iouudeti.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2mbixagto.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2cpanhngs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2zqppbqit.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2hjaazjft.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2nmtjjvju.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2cawjcmcd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2nhquwlcg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rsanmzvc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2wvowymvf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2fjcrlhqw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rdelvalv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ehjjxpoe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2hxfokocq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2wdjivvhl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2mpyxrpsv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2pknicdvm.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2nkwxobww.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2amwsmlez.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2guakqwmq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2itdyxwug.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2swbobzoa.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dzviigft.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cjkjbqlg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bywzxgjp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tenduxjo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xljtthvu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2iqiyvgqy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jxxitbqw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2aguiykui.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zkhnzjjd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jgmkihxi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dbyofbay.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lnzjlxyy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mjkesclh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fselsrgh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hclwlwhn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2heveznrp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2qhcnntms.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qqehhgdo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kfqkicnc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gxmrmubi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2oudrsnxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llbukzbi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2tuiuermt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxmhpsqy.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uooifypp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kdaznwyd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xqlkwrwc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2plfneult.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tdxoesxk.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2atlmyxlv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2oamabgbu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2agzmixpq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pkikgwnc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2brzsuwdj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2jzcfjokl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vyddztjc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2owqjmrnf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2dzmublvv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kgayfyso.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2erppclnv.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ccltrkbn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fbrkocis.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2rgjvsfsc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2novntqdv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rqjbpbka.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zezddwxi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hswpypxd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2esyssjno.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lcpkrgux.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ypdmkezk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uqzzulzm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2aissljhd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2rgczbpkh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2httivpai.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2drpojnwm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2akkbhyxk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2lsnktzbw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ovyqznml.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2skrflrwo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2suestgep.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2trzgsneu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ztsmtjvk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tjywwliy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nvrwftqz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gntcwclk.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mvzeohck.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2czlfvvnz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qhzuwssd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tfplakph.html


<!-- 参考信息 -->