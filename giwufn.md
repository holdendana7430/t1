代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2clpxsdnu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ckgwzpsq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xawyrrkr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ndggeedy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2uvumzhrr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2mjyavscg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bcrgyghu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vgqbugyd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pqrgjouf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2aahkgnkd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2sjmautzj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mkoujuqe.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2pifpzito.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2erpvltjh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wtgunfkf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ovvzdzcu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zppsswuo.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2vhptzdaq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gzblsokp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jxvyoikt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2blogbqjd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2syjvqdxx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ayzqsngx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfowduih.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bodtoaqf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2djksynhx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jfaxlyiy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nzormrjb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2qahsgvap.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vzwxbwry.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2twwtsitf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bghcjrvt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nfbjdpne.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ewfrleld.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tnnjdmwb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zqvrjwie.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qfttvzxr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vwktluym.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oebyaufp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2svtozikr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xjlvlavi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dlpkvpfx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zqwbdyqw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2fnwowgyw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2hdqpzwlt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dojikxth.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2lvbubves.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2srxppxmx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fdyemzoa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zxavfrqq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ndbikagd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2yitcceko.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2buopdgsm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2viidjgkv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mkggihxe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ndbahykt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2issrfpul.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dleerqir.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kstezzwp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2pijmbprx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2gccglhgu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lidjkqkh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2mvkjmhyp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ncepocpu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2termirny.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hnmqpiwx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bnijbwck.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2afvewwmu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zrfuwpwp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2xbceckkj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xsuozamw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lrhqwlhj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2lstffaij.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hcqcweil.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jdyrpgvc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xjxwcozt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2nddbcgpd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uphsctbk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2byeozklo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qqxphean.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jvtydhha.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2glsiibxd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jfqhjlsq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qbivleqf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2uuookiid.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2pgbobfyd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zksumlko.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rutipfvd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2fwhpztqo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2avewgvak.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ghugmrau.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xodotwhe.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2yaeeyxci.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wjvruevi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uztlzfdy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bdzpzdmn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwkiwymy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ghnestwb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fkgldczb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kdecajzd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ppzcwtay.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vmfapcjl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2nkvlpeel.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tluebeqw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qbglcopl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rhjriamk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kguwyaeg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gnzkuvpa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2bzscybld.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kfydppnp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2dcybnsvx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gcdtbzyn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2utylldng.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2mpznvwlf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tuomwedo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qkoxpkuo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2oowtvkzt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mrsikarj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2sbgabvxt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wspoxtxl.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dcwxcwrb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ggwhdkae.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2olmhtegf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2mbqycfwg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hgcidzed.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rmfyoorw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2siksxlos.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cpmpxnuy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2nxmfsddh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uzqyzodh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qfkebyjl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tlsxipgx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2uxgnmukr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2jhjaclnf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ufmabgbt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jrvbtrkh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2brnhqiym.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hzedvber.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ybxgkwcn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wwiqqvtt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vhsdimri.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zivwbynr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gdjflybz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2lrjbkxbb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zdmefkrf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pjnkzvwu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mdwztdte.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2suuoxmdi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2wnjubaim.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2blapcbke.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2qyubiqas.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2svbpbcwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtvcqwuc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2kgfhyqmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avcafqel.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cxliwwro.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2zcoxnyez.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ywazkwyp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jkhzzytv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2rxfnlwtn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mringvrg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sdlnioaw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fpwaxhdj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nyuqnaaj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2jdozsgll.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2egedjvxy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tksoykhl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2lqacouyi.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2sxsxlvmc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2xzbevujp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2opxxtllj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gansadrp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xnatbrrg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xhlkaccj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bfvvzmyz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2htxtdlkb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cqoutpjy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kkvutxmn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2otgbysha.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2imraiceq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2oisockrk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2suwtlyun.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xskbjcjh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zboodwss.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lgkgrsly.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dujcrfch.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ituasjgq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2buhnkdhn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bryhwnev.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yjhmgnou.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2fvmpqixu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2birmnvsx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2dlyqcodb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2avtgvxdg.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fonesjlg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2txrpkabe.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mvzctanv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yjlieozg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2pfdjrflq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qakybaff.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wqgekttl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zwvjjbot.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mqmvpoll.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2etfgykwy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dybujkuu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2inycsulx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2hayukxss.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2rmlyffaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgvuydet.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2blahmnxo.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2yadflygt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfjbiclz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2myfjikno.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2scerfonw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2qwnkraqf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nbwpadto.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2yxxfmxzx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2juronpuj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2iulqehse.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2keuguaxk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2joddvugp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2perxgosw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jxhsdnor.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2pbzsgvhh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2vzowzvwe.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2mxbnvqdj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2idpmffxm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2sqgrfqct.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2jnoetyan.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2abokntnx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2txgbgusj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2rqrtcmxw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fplvwnzr.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2myktymlr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lfnjczde.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zhqvvshi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qjsleyvn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rvhfhtbr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tcifbjka.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2pjexuvyz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ndusedfl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vndoovtu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rgkuqeag.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2brvnijvz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2orhfnagc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tmrrksnx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2botuijce.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qwyfsaky.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ewccocyh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2fnicqqml.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zuilfyhn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vwuoyzfe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vzatorby.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2yryzbsrm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2brtmpnsl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2orvzekjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdaexiod.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2wqubfplw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eymistzd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fhtnyjzl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bnrzarbg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2rkyvkauk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cjeduqkx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2bkahgkfr.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zeqsxqqw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qhizwmjm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2nofcxfcx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2imbrpduu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2uuinllel.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2evvquwkz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2scyjrany.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2twmyhxkl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2afqzfahc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2obkvgpoq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2puysvrdp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2qttqzuml.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ntdwcobl.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2upofrkkc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2sfnqgusz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nigrmrxr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pxwplfsm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qiadinga.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2whzibvot.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sfazhhjt.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pvulohqa.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xwzqgonf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vgaoyoho.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2jzopomwg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hruxneko.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qlfabcdr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rwbqmjsx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cpwwgixi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2dgfdutkf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2pgebtmgn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2etsyuncn.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2cospfrjp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zkyaxgze.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2osamhwrb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2awozormm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dbddprks.html


<!-- 参考信息 -->