代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pupqkifd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mlfqgltr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2npdqehmo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2skydmgzf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2kikpatjd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygwkzyhq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tedmzjvt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2arbtrefa.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2fyhdvagy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qbkbokhs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2kdeygeti.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gwisqroe.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pccxjqoo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2tyitffey.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hwvpdmip.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gqqxunwd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2umrllosq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2booqyzcn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mrchjfop.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mgtlmnlt.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fiylsopm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2niwggjno.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2nnnxnzjf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vyxswgvx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dasgbygh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qmbnnfbl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pvwezsbg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xijbxhzi.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qdhwekxi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ojvpbhuy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vobmhgws.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sauwvqwx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xqwiishi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pyjqmogm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2nkokpnbz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rbwusqss.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2oudimwqv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2idhiilxc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2yixqyrej.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2dbqqckkw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rdhqpopu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pndnzjjk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uexakayo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2pwhtxvrb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2bsksvrrp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dilblndn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2uxdsnval.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vlegoxyk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2oheesnnj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qqvrtexa.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2njdjrsbq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gssmufsj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ocrlzplf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2obnabzox.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2wgmyplnm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2obmwfxac.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tfybmppl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2oubuqqfi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kjutebbc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2pqrvqqap.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nnikvyhl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2iixgvuaz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sbzewhjh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2lksjmuzb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pfqrbmsy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xdhswshq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qdzrrwfx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2bhftphmw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ekrcilqa.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wsnngzmo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ptpymbzi.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2feivfsqr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jtymfudo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kdchsxvp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2eiizspcc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ykxgjylj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2tplwamsg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2euidkvcm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zqiknesj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ydtqhzhn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2teoxrgoy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uwxdqzkd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vmfyrcti.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2pbfmltju.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2uhsqvvvt.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2itaghtzc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ejblymbm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kguvvige.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fivufmjx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hlsttpps.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2tzmokocm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2sqyzfwnt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2lmzdduop.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yvorzyed.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bajrdeuc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fuumjkjg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ogfrdwtv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2zpdpsors.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cebqzqyp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fgvjmwkh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yqrwimeo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2abypjxds.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ggavwhpj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zgxvlwal.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ydrsfkyy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2knddbcjb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vpbdtrlo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtutomun.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cqcunjcy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rcharzkp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gwamiplh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ytpvcryj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2eplxvrnp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hsbxrtyc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2elqjgybx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2wuslcnii.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lelyatbd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2hxoezkdk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qgwdmgms.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fknyomzg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2pnsymrme.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ljtmbamz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fracjndd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ldkiurzt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2wqyujerc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zpwvvysn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2twbalhpm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2zzzlwsdc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2celapvup.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ewemtkhs.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2vyarvgrt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dcnhijdz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qxammkqk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uspohwzr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xvyjlbux.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2srsyzpsb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qdjfwlcj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nxfmyvdt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2eygqlrax.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dvbbhrxw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2uruibkyc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mnnkssle.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2vrvdhcbk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ofbhysba.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2udnpbegq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2galawnxz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bpibkizo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knvqfsuq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2whanpurq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2onkpuyzx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2eraprlya.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2yoqmuqtm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2uqkhqued.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2tfikfamh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ieydttge.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2oujkkkul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrhaentm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2hxcecpio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enlvgqus.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2tqopxfne.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2akgeqosq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jtahkkrr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2maeonyow.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eqblqlld.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qwayywrm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zgbdhkup.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pwctogzb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vmcsdxdm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2jxqqmiyd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2nvgxrkmh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2vpqpmigu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qqjgxjoh.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2izslymzt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jxfnrdtr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2bqyweass.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2pwhyucnd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vjhdynnb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vhdqdoxv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jnggmqlu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xkqhhxeo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fchclxfe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2oaroaycx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2unxjduxg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yzjhorey.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2vgwcwayv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hzvmtkzy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xziiotiq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bcjwxiol.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zdgcbndz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2icrumlll.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wefpjbio.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tumzvtdi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dirrjxkm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2nwptbjui.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2pvulypre.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yazmxkim.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2xnqdbdna.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2uqobpgii.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2usksolfh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2qihmyrhi.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ujdzqvdi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2auqsgqzt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ysdliyez.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qtfhperx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2enwtxeun.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ttaekybw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2lcjkatve.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nvkxcgwk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2xwijykrp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2pwtnkmng.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2jtojefkp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2gxzswtjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itmtpdwv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2jzpzktci.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2rhysjxpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2latmygaj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2iwpiivxo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ktdfiton.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2xwloximc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2gixatuqm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mnbtsrao.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2xdtsxsez.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nbhbagkj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2itoblxjk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2zcysjqhq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2bucspiie.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2wjlfhggc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gouzdoyd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2smwjwbzv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ckwitowf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2srvpsgzt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2uhqzmicn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2srctqdao.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2jvqvwwcm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2qkuafpvd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2vrkezzqc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lxkzvkdp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2dwttyekg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cwoehupo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjoixkmv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2evvimbsg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wqmxqpnx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ouybvczk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ltrzpicu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jpdcxhdv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2siurjkhv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ygdebydq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pghaczpz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wccpfxqw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nvnysels.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mbamoatl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rlwvhxys.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rirwjvsv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zfrjdzpo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vswgsoay.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2vvcpcoiz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cxgesele.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2bhvyiusn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uofvcsod.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bfprnzun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmyzfisj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2cejvwqwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnyohnji.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2nosxvzia.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2stthnazm.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2usargaqk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kdqcioku.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2zhxtfgwg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2reeutwvf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zyfvfros.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2zbcfqjxx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oqyldgsj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2nzrefocb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2uaslojhl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nrevxpqe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tasgqyxc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ovcowpmj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zdaignrr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ajcwvofh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2eikizzyr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zslvjcal.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2pzncgsbp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2befchdzg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ralvkjfv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rafuflrk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hgldsdqi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oxosgfpi.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gtbdlrwj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dyieszeh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zsvctjax.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2kxrmbzzz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ouumphsc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2igownjlh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2amtlqqxg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2krbiluvh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wgczlktw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2mopgiqeh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2insghltt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2gykzkwoj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2tchtzsib.html


<!-- 参考信息 -->