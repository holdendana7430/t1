代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dnknxqwa.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3tcejfhgs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wfwxtdgw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3popgcwfu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xttisxta.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjpcyyzd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ttejxszi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3rfkbgxud.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3unzvjbpv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pvxntqoy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3avfdvdcm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzaqajph.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3xinvilvj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xrqwuhkv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3eviibwux.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzxyghlr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3suxuynlp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3njjgngll.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3uifcoyil.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yenrrmif.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wumhzona.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xbuvsqmj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gvekgerl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3igayjrtw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3moszdqai.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ngyznsgr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3migkilgx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rblxprbe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rgbaqztm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hkjrxkci.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3stfmvfrj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ojqiwafl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mpnpjouw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ntjxdlrq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3sbhsacku.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3rfcefhop.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jmrhuwpw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vguufcjt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3azkanzaa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3yusxwrqd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3jkdguxxo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ioywtaqf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3cjbiacsb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3lsyizyfb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zxugeqfa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ujovxbvt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3nhndvdyz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ifdrvppl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pixyexjk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3yvntyrxx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3cxlmuvvo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3gqzvloxu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3uvzmfici.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jthgsoix.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ygcpvrak.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qbbusemu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kqwjgnzy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ntmowvia.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vgqrpiij.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yjmonscm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jzgfbitc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3miygbxqw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3thrjuepf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3daptdcgy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rfdatwff.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xqolmdxq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3svuvevji.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ffsjphbm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3xrctrziw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xofwzxie.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ppuqqqay.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hjkmkaiw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3asnhjmvs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3nqgutezj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3esorjule.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ruiuklmx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3apvyxzgv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zlmepeox.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3twxshrxn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dphvuhmm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ibyeafme.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vlkgdhit.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3zektzjbw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xnvklxia.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qswpvkwq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3fgoczkln.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3uegnoxmi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3kzjdveul.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3naspjxhr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kwyasibs.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wzpbvhln.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3djzyqrte.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3fpwqulxm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yjdkhkop.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3banidycd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gymlvybw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jizdxvlj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3sllhucoy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gpcerxwp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cojvqbmy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3bqdkbvrf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vddgokvo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mjqgvfeu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ngzflaow.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ppdrvhuc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3pkayzpdt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hrglxubo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdkehyxd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3mktsgbaw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kazbfhsv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3kmwmevww.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ypxqhzvh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3iwtestfa.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qjjhnuei.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rnyxnlsb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3utkflzoj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ahcqqeym.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3zkwysiio.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xbbstszx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zpegjold.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3kbbuwqnp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ipyzbmos.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3bwdcpsac.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nescidsr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ivpgvvkt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nlelrfvs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xclczmrt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bzfynbbc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vqfywwhb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rkmfuxsd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3fjjfxfbz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3exqrwkbl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3uakcitrh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tfdzxxpc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bgltcfrb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rotlerlv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ietilwum.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ysvvalzg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3pigerxkn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mireeqlk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3hawwakhg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eubmgxld.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bvgauvzb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uqidijdw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hhfdcqnw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hqjtyzlr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3bkurlpqd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzweongp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3taycahpk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3pjamjulk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ndpqdbnh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3cmcgpghf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vhzaapxh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ctounebs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3cruqfwnm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3srdfjrik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fihykjkv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3jdfsrmgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bojkvuqp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3xnumlhdx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vfugsyjn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ogfnpiii.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3inbmswws.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3arykkqub.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wpzfdsow.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ppicewag.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ecyzzgtj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fneutzhj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ijpryepe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3kqxwdkea.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3rgzosswl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3cqumlrtb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3qrkvczmx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ropjazbb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3yfnsclcm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3btvlyyst.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gpgtppew.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rwyohmma.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wsgpbxux.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3haqwlvor.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hniwcftt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lizknhby.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sckbvokc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lqrfqquk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3nzjuprgm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dgfhzyuw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xoyrgpnv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kxdvvimq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gwfbtmdp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3oaowyonl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jujvrokd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ohnmnyxx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xpczpyzy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3alcpahfj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3qjrhqiqy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jdqirsuy.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rvqddyvf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3hgqmzket.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wavvddyl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nxbjifas.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ggcrgutx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kmbaxvvm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3lrypbqtl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fymwkwqq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3burlrrsu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rdlurmcc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lzaarnls.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3hukoqdos.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ijkhoncp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3eylctmxm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3fphdemhr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xdpatoym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clasbkoi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3gurhruck.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3oujtvjrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwxpaaet.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3tzsvtzta.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3hzfjwcec.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3koravtil.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3faohhxqc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3xmnkhafp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3twhwbklv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ltmwomtq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3klgtzgqj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3mlfvhewx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cromwhqv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qpujcqca.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xliqfejv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3kfbrxdsq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ztygndlg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3bbvzrrnp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3zktmcurj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3vgzvbrjm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ybbzxllt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3xkbkbnxn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3tkbkfejy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oaxrnubo.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3bmszyvah.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bnxabegc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yfgbdsbr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3chnvunrl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yrvmnrdb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yukqifot.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nogqssbr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tekkuxrk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3eeynzxbt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3omqlfbgn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lmafseuu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wdtzarru.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fvmbbwwp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bqcxtbcn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esyyhcnw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yhvecheo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3mcxezias.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ryjellgc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ewimwmjp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3yhepcprd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3hrkllqpr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yuvrutuu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3snssgyqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojybgqdx.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3tbmnrtwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhlsreuj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3weausotx.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3claanerj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3phfexfyb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ohmaywrc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3iqwhxkfl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bbmpynif.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xyqoqxwp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3uoionlie.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wvumluld.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3dejekgkk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3frxqjchb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3abvjruqf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rcaxgisv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mfybdjle.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zvxxqovn.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3hbfqzato.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3qagjeqmx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vpnylccz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3pofasvhr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3iaqybkld.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jgltmivg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tzwempoo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dcoxuofm.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3asxiiegj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tdlamjmk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hvssqpgm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zzaxdohl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pptzcucv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3nkibmbbi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pmezyoyl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nrvwaosa.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hwaccfcc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3cbhfzkrh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ksiysgqu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3gwjhrpuf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3oeawkwcm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3fjhedymr.html


<!-- 参考信息 -->