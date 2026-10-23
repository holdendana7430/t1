代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3deedovff.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3nkyemxcu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qduftpur.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3stohllky.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zqhnskol.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3porznotg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kylgrlyq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3mefpjrkv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3zaibosba.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tkoxisoq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3fjwlgpau.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3qpzeeigv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3emvmmhxl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3kcgqqekt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rsfxrcpv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wdlyjebi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3sybafdxo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vjqsjnme.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3vigedgza.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsoxlobg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kabcmtvi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3bdnfavmv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jwhxujao.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3oihgytkw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ppvplenx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mkwzgtep.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qqajpewo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3viglgpba.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3havddszl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bvsnjkvt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ycpjmpya.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3drfmkful.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ffchyzpe.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3pftbotfl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zxluvbch.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rouwdgww.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hgaujcwr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tuckgjfr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xnoibcfv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uyygbkri.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3btmbcxlg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yjbolgjr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3cygkdaso.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3hmnaekui.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3undxtzri.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3llnrgsjw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lppovzwj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kcpyoapr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3wyepirtj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hretoipv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hnxzuxul.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3lqgciogv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3hlzdwobd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rpeyuzqa.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zgccywfc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3igyoinrg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ldoovltc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3msuduaip.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gjblwghz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3jpgwplas.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hlbsvilr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3sqmqmrvo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3vrlrxpmd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3inugltea.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gxzioczg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ozkevoji.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vywyfpis.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3mcndgmtf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kdojrslg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3lczqiyqh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lbpjywaf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3krmodjzz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ichexnxk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jonhdcno.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rimjzbby.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ofbrveof.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xlqdebdc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3cezhqcfi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dlnosmpm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3arcqjpti.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3slbwslgo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ctpjiobq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3axlsigcx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3kqsnqpcc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3otxfoodv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zpdzvheq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3awyjehdh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xdblnqpm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3layzgqha.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3heseypsl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ywtkkxxf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3umtjfrmc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qxdhqqxh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hcwiqkye.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qrgyxsvo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3rjnwbtwm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3hfamuqre.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pgnfgszz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vrqejxex.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xbnjazun.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3czryyciv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qvdxprfd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jnqgohly.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ayabrkoz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3fmqltfqf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qijunloj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3crazurop.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ngkzyken.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ekoicryh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3uiksmdaj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3uopedlgo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwvcawvt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3yclclvgu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hkvjtsyi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3abfsjmdt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3mzoovjac.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3hqgsyeyl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zmywqmtl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3kplfbwqs.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3diwnedcz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3sjeosnts.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mtarqosf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3wamebrdn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jgkqswxz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fztbuyzf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3sqlrbkzf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mddtwmyh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jrbczhlo.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3trqrxoef.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lijqumpi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cctxysue.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3gbntneni.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wlzncpau.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gcqguefq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xrrryazo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3cnlidvxn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3bihmyvge.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mqhpwljx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ghtmvtxv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3kjfebnkb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3qkttfjwo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cmsxyjzb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3vhsoxssc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wsgwbtwc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zudrhrdn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sgklyila.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bwhmtnbz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lgaxxmew.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qhybcpbu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pxgcvozr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3eyisyuky.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3whvpxhnn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jvaqmntk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ptxjxfuk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qjgfkghs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3lsokzifb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xfgwbjax.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rcocvmtl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bwgnuvtp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vaomwflj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3viednntp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3mfibnlex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhlnanyh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3klwdjpym.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wgnhtvqb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3kkvfhyfz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xnzumqhg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hphhddue.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rrvbjyax.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dfoxvqgw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3afayvavz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wvdchyph.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3dkpsrjdv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3cdcarsml.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ejlgmpdb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3njehgkpu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3dmogcgkv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hvohxffn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3udkgzodn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3yblxmdos.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3atglgjuu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mwnzsqok.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zghktilx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vsdwmzar.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vfopqjob.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ogmtmxqy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qtputdkd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3skdoxqwd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3lcnebwvc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3quujtmyf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tndqlkzd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mmxvxubi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vnqocero.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3johnwkff.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pnweudgd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3chdwhheq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3faiixgpz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3exosvggs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3puhhtjdl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3btysxvkp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ndwetiet.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mhkahcbk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3jyqdponf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3eqavznot.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3zjnnwjvv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3roftgvra.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3urffvccb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aprhzzfi.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3mhnyyaad.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ewdsaqeq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3aivvegsx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3puvmchrw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3wncqcasy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3kmhqxezj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3sbppudba.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3tpbubsrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkxpikyu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3txppfcph.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ftqavawf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igjbcfvp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3sbmoslpp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3wewkledc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3tzuvanwp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zupqjunh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3llauposp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3gffwclfa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hdvxefsn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dcllwrpl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xorhvitn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3offvdbkj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jfaeshyb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3hxuilpsg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ffuyyhnq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3bwwlxonb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3rosmceql.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3hzkhyotc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ffkjvacs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3hnsbccbc.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3kzozehps.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3cavfwxom.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ottqntqn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3lysfmwzc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qpxugyts.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iostizkm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wowxfapv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxsiehxl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3bgmsjcac.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ssazrnnm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lmceojer.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jjkaqbcn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3atsjbwwx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3aregtlrj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3yvwmknht.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dchwsxss.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3javwaeqq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wurdppuu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mwhlvkrf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qdxbhphe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3psxdaqei.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xdcgkvuy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tsgldyit.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3etenuydf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ewyjaaek.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jovzymig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slqqrceo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3frwouvjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3voscevkw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xwpcvkpz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3oariluwh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3icpzdzcm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mqsxrzck.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3bbkvhsbw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ldamzkue.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kbutkyni.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3pobpugjh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mviwqjxq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3jofshevc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3dnoyxfye.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pnwsrxyh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ueunbqlk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lkmmeyva.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pmgrpcgb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jiavjvnm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3pdgjhpsl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cygqlspn.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3nkfhwjwx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3klbxaqyj.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rsbjnswe.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aewitpob.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wtrffhze.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kkaseemx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dtlgzdfm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pxjqohai.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3npeikfqi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mucumrap.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3yzscsdfd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3noskshuq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dupwceuu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mzewxsas.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3shflwqtq.html


<!-- 参考信息 -->