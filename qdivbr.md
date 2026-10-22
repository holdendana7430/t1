代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2axixzblf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2zxavmmbk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2rqjuogel.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vwlgullz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2arcniaut.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbnajtul.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zxrwgvzh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2uplynova.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2uqicvinx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2biuohsyz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ersdlote.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddtnylbw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2auaconmi.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2eouhsjdt.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2apeofuab.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xejreifc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ziahpnva.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rkyqucyi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2idsrprsf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2osihmxeg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dpfijbxc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ddpcgzir.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2atnpdlbc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gyxbbizp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mxvnrqrc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2sdkciwzr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2igwavzvs.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdibhdhy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wczumvcy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2muxwrhya.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ykiydake.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bzrztkdo.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2imxkgrkb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kuwhwgkg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2hvustscm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ewxupnub.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mlkcbmqy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jofpdyaz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2zygifrvt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2xxlavsif.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2riujvsxw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ouagohem.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2sgkyeskm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2lmdsjtfd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2kpkgotit.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lvalygab.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2cbafwrtn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gsqpobdd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2plnoiezv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2rvikxeyj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2jlmmsjds.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nnflmvmt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hlilciwa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tgxxafyn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zhgzntmn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hgznitdu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fpxyktbd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dkxlhlho.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2cjcjliif.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cxzpxpqy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2epzprupd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2xscxcdjq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bhhuxqyt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2snpttufs.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bmbyxdry.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rdkqpvex.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2nnhbhtuy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2bpmtxowa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2tujsbzsn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2lcyuijah.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2aciyfejj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qfzfkwqv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2vuhnxjcy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vhywicth.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vmexhgmp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2drfedgpk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2caeectxg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2qglljbrf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tjbcyhoi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2vyvyltqs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2obgtumwq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rqmdlrky.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zgqanwpl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ekjkksgp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2dbjntuof.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ujcjmdlj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ghcwtdqo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2eoulpurj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vimtsuus.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ozmxgmgk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zudzkevh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2lcaqwzgr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2uvixxkwd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fqmrpndj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2gyfyvjit.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xxnigyou.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2silwbwiz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qsdfwahe.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pfarizhb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jiszqtnq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2afcrqojs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2oykpgaep.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nvytfukc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bzjdafdd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2wbeughbr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2tagbehqv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2rfdhthms.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2blmxxthp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wtzvobfn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zkkcqhum.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zowunogm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2yhnywyyq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lkskjvis.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wkdyaryv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2lgmydfva.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lbyyufhf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2urlhbshi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2vvqbqlyx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rxcqkqld.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qlghnytm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2izwfwxvf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2peztlcyw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nxxghbjv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uebweufh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tvddidtw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2siqvfekn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qxebxoqf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hztirtjx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zjriyqqc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kdxbskwq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2hcvyqfpl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dpcasdzr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jucynehp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uyjlynba.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2rgrbxgfg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2nkgcahdk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2swzwhrma.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rszpkxyf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zkdjqldl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ywoomcaq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ijgnmrzn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2swyuwdhy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2sgdtwlds.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kyeddbjo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zaxcwrgh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bqizufhq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2utveaouu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2qkzxhwhe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jqjjkzhy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2efgsiwjg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2boiiuvoh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ofrpkfep.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tcmnacvh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ynrqnlgc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2mlhkjugm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2flryfyay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cnmclwwo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2awpuzhgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrfcpi.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lubifdva.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dttmtrob.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2rwgghxvv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2sdalumus.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2nknrzhtz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gmismazb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wbmnddgi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mtbgttfd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2iagdlpyv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2hmtgxyeb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2piqnqszj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2bzyzqovp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xfngqonb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jwybdqij.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ctvdcabo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2fnmriawr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zpowqhrf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wonorpva.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2whlylxif.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tkgaxldl.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2gnupuqyi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2aighsjqo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ddigzyxo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mxnhhfwe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hvnyogay.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2kjtjnpuq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wsfshyds.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tsiywqvh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bgzytaiw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hbzhwkmh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cmtlfwmy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ufinqdol.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mibazgfl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wwokxlhb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tppgpotd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2dmluljzg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fpghkuww.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2kxzdqubb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qwmzrygf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2mxveommo.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gfxypnau.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rdubebtj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sgcyjoel.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2uzaqmcxw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qjtzkuvu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2bqccfqed.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2stvtyiek.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2jyrcjuet.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2zutlfrwr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2fqspiesa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mauzbsic.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2avrrmazs.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2rrtlnncb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzjfzkrm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2jvmepxpe.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2nbjousur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2muvlvvce.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2trgysblv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2evuaevbn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2dliyfbvr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ymjokqwv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2lgnkwtpt.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ysbifwuy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2pbkxspnd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2gnjoqkpu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2hdpjirqd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xfatwvcb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2unxbkjkv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2sixdztlj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jbthamin.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2pdblpbqh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2sukyzuyu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ocwbrobf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2tlwkzdol.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2yjlyzpmx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2tvhtixmf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2illqmmwc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xdejtsar.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2wvwvqqyi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2njolwkwx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2arwqmbfd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2uitdrjnj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dbstqfet.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ofnprocq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qfunrjts.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2snjjtjqn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bceryqrx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tyvjoblz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nzvlqlst.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lpzofaya.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jwezuhnq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rctdttqn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jmskyhlt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rkofhipk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yvjgmduu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tupqlymp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iphtxkvo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zxsoaymw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tuegawjw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zaetqhmg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zoyfjfkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgolmirf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2spnvlblg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyltirpg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2gobnidje.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jkvazmvx.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2hbyfcedj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mokhabbd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2hwuaysoo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bvffkuhs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2nhfzzhrm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2hyhftutr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fbgqehfl.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2oopgoiep.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2jfvqzbzy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vgrbpvld.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fgwadgfc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2wbkoaqks.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ovnjuyao.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2hfvxufjt.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ryvszfuz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xwcnsilt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ecdjrhwu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2hsstlbsn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qolungax.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pxmagles.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kchihiyb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2znlyxcuz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2meuuholk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vqnnzgos.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uuqqcqwi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pkpiyxxg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2lickyvhk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2rkjudici.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lszvvrlj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nyiskqjf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2boagojov.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2isyusgqq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zhpgffnn.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cdrsaegm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2xwjlwteo.html


<!-- 参考信息 -->