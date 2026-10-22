代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zzrrmtrx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wnmeqebg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2elruywos.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2abovrvjh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2lqojktst.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2srsgwqvs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mxxugtps.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xrqltegy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2adeizufo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2judkuioz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dqnxxcas.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2dyeykqwc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zwhjmwes.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2chapslqn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ysqyhqpa.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuyrskxx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fbwvymsy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jruwlnbs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2udhfqhgr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rbdgnpes.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gxteqqlc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mqzggfxm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rzfxahjb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vnyfhqmu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ohpdgefw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qapjpttn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2igiixmgf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjoajvcc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cjhgfzat.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2tzerszkq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lgktrwry.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rvmqqcav.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2sspmebly.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nckihixq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gciqktiw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2vctcvpjo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2anwpwlee.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2uxxgxcbx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ommswnmm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2nmjzftkf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2yksholmd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cycoxftj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vezcojox.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zhjpzqry.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tnotybtz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2syrdpyuv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2vqqlwdod.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2opfxbpbh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2afrwgogt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2siilhahx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2gfjlljtu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2akmnmwfz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2cjbhwenj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2wnpnrmev.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2kpiretrv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2htrfpjjj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pzuxnefo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ydkrphyn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2gxfdgxcs.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2rgapnhpi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2pjikusbw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ibpuzvjn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uzothqgu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2pwlsywzu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2psscksbj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zpntvtsj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2tiqgjapo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2kkyuausl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gbcldxxi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2gzimlyyv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cudajhxf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2swotnrwx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2crugkqlf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ovypaefm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2usnsckuz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2xsswrtzh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2amjpdzoe.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vahvkzka.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2opkkuxah.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2eevocjpp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2fjrkogxx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wrpbkdga.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2kijqnqnm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tgfpwtas.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2btqwvhdp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2tgbltuqj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2iqfqinup.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ammvvomn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2cswmayft.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xdlwlayo.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2fxkxrnwn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2edazzqij.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qjfnkcms.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dkaksyae.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2gehlqcyk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2licpnqkl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2vhqtjrdp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2thvilvnn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gernblkg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yjesrfzh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jzoxmvtl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2nwarojyx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2btdizcja.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dpvancya.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vaoflnee.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2meiodwbs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wzrrdmex.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bypfflje.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2dsbvzmjx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mmhbfqqz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2holldvyh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2frwlmauh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2rwkajghi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rsnfgwac.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xgaoytag.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2koxuqecj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2oflkgqmr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2bfvsnazy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2irahxswf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2shfmmpxu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hdbacazx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mtrtvltl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jrfipgin.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fzqcezpt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zaelwnja.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2mullsstt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qdimoeen.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2tpjtntip.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fsnztdvc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dtldzhsd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2kictjhpd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xytkdqpa.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2smcxatvo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2axorrgom.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2dgrfpeoe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2uzqoxurq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gxhnvxva.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wwjvtqaw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2lwrievpm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dtlvvcxa.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2mrtyrtot.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ltzxskbr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wdrpoocm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ngirfmxy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ffkjvrrp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lgcwmalv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ibwokjxl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2oqloqecm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bweghjsz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2hrmwzrvg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2jjtgwvgq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nvghlbpo.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ugwthnze.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dziwvfqh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vsrmmlxk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2opsjgtdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ouitvilr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qnveujhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lybwobsy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2tpgfmtpg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hawbhihq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xxuuydbz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bjkqstiv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ckygrjuw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bkbtuyin.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hsmmqzsr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cwtmyrsu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jyppmpfs.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vtfnndgb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ntyylnpi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mvbypgtl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tuiexlfa.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2llmjuehs.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jyjrqdgr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2wqvgfpai.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2okxssdbj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vcqvskbm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mgbwvpif.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ujhpbywh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2zfpkjgvt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2olflequr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dhtgucfo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2priongck.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gsgqkrtl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2dzxcekxt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ftqyigft.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bfdkkryr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gnnyikjm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2afcqmnnk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ymgfshrk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fvfnlrmv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ziynusai.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vjmzlrsg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2dzezjogl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jecdmkmb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2akwzzjoa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2tjfpncnb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2roedrkvb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qjdvnfmr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ckyihpzu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2fjsokvcb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jkksynar.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2iehqqolm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eoelshyn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wfxvtjsj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iscefhsh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2nmufdmrh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2exxyzhtj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2etqywmvv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2fgcnfeek.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2uiltwmji.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2yyboadvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2miiwvnvv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2nlfefrhg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jfhlqhhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruthpbih.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2elnzhkta.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2hguramkn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2lqqvttvv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2enummvdt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2yasmawqh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2iwumrkdk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2shoiqzfd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2cxccekif.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2cofyhxel.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ucfsggqa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2pkovoinz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2jpqyyaiv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2azbonigm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2mttvznwp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2hhdakofu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ebnhluyo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2rfarznym.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2dqzmcxha.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2pjhwztom.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2bglazqao.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vmabpwli.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2zuchozgw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2txznmxdx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qflaizyd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yftbfucm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xkxerpbe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vliplfmc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2usxokxhy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2lwzgksye.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kujijxds.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vicyyxmy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ijsagtql.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2uukrvlef.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mfxtdztq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xrhszmff.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pgzjcpzd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cnaxnopp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2afncxsmv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jgjxtlbt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2dfjewmyt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ugtlfmla.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kkwadpkv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wqqaldcr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gclqiagp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvdlyngp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2xmowbzjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjhygxwe.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gblwtosp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2eveslrqa.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ekqjkxbv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pbmsomti.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2zywaoxgc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ochtaewg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mfgtanhk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qgpocxug.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lvcqsmby.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2gvxiabgn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2uggcpgpx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iklwmfry.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vyjvtdus.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ispqideo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vahjkpbz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2crbwtjjn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bcugmgzx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rfzuoqat.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2jxmsgvst.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2krvujhcl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uabtfsmy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2igxyzquw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bytwozvh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hkopprgv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hpwxdhia.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qqzqqtoc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aauntook.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jollmday.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2tfqtktdo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzarkufx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ngvjthtj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jufqzmvn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2undkqvtg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2zutakpkm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2lgilsiay.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hibcqlfy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2pmiwugbt.html


<!-- 参考信息 -->