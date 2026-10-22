代发 wailian999

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2tknhgtyj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bgedlgoz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tzkeqyil.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mnhfclce.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nzkzanka.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2niojctck.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tqoujudi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wucxolva.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2gntaqpzq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2bnhpcxeh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xloqfaik.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yyiahrtc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2uaphvpsg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2owyyckff.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zgpywrnl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hokgnxgr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2gsvpwkos.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iyotsulj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ognbtkon.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ggrrlvuz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zwmhonal.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ujtmfxdq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2dwfaumqj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fjixnjoq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gbfuylpc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pqixqxtc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2zmhlnwpb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hgdvkojs.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ljwiiixd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vocdzskr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2byndxcub.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2xotpknpi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2pcujgkke.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qihobwwz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2wikjasih.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2dvpkbugo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2tgglqrgl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sehmrong.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rnicqebm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ucuvdsqi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2kgzqrtcw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2khztaxfj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2rpszodgx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kwdtvyoq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bkhszfdt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2upbfbxpb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ifwkfoub.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2pdhofjay.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ggyuwvyv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pmqhjrjm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2sunzngna.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2sromdbih.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ilevhgrj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyppwht.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fzighjjm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2tjtjqzrt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ijcstsfs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2skvbqgig.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2kvuvhadv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2mjblfktx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2kbdapcvp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2nvtndnje.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gbtvlolv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2sldzcxts.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ihogzxct.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2wtsfhwly.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qkyneouq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2hvoycbik.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fqmmgwdp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2htoekjql.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2nxweghxr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ehjxvlli.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2mixqsgej.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zronoilv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ngejgfit.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vnygrrdf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pnyczvtj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2sjzhlwqx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2znfmgrtv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2uhxejscv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2dtlawpgs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2cqvhtece.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2kwfrcduq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2xphrigup.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xjmolcyg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oagvatxh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dnkstxse.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hbqijghi.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2cajebkad.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2jnhznerm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2lfyhtujg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gqhlqqnc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ehwihsgq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mibidzec.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rpezyify.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2srlsnelk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2blmxrcjy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dsondbmp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2cjoqvzfe.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcophjmi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2svtbsvjs.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yllfauev.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wvjxjjml.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dkzaegxo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2dbozrkko.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2onwzcuzu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zbngqdnp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2xweopbnw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2jclkkpyo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2rtgllpvl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2slvlcekw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2hphgxjey.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xaxhsjjo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2cujrdetw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ryruabon.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2abcznodc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tzmrmwyy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hdwsndci.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bnawfjxs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2riuyubvd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jldrwkgl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hzsqnbxq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2yfzjlfrk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gdpwojpu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tzrwdylt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bkavzgzv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2nezrzzva.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2icdffqdo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2hvwhcrfd.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mktcxhon.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2duqgvfvd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mzmrfgvp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2shmzireu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gckcsitv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2lfvmyemb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fiplvrng.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2itprdjzk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mnywmduo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2mdruevkn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqbwufdu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jjikeeom.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2jwodkwqi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ainlasuj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gybuwmci.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2eyrkyubm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2riudoflh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zgnuekjo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wntpywdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjsmfieh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ksrfslch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxepqgta.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2eomnfxxm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hsnmhmiv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2drmoyrqy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2paujhipr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ediixbks.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2evjxxsna.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dwelfrqn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bgtbxnov.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yrmvnmug.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mrvgawvk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2wkscjcly.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2juskoewe.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jmeazwdh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2grmhstej.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gqnawdcg.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bfhcjvmp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2miomfkmi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dkohrabd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aweqipif.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2idrttmut.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2yhblgbkx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2thrlijvo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ucyiogvs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jndkdjfw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zxuctfqk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2knsuxcdo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bvbhwgtq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aaudmsqk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bxuetmiw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2azophiew.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ryjmkrbp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uteqrbhs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2klzqehtk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bdzlurra.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2iegkxqnn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jkktrpvn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ibykhutw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bqmqvzdo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2rigdtzmg.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zdqmaoau.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2udebiqjt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2kkkqsdxl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2psgwkvym.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tiwjkken.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2osarvvni.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ygeqxdch.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kkuzkwlm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dhaefwhu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2lsksdtpi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2glkapeyg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2glydjxok.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2lxtwctlh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pmkomowq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pozidcyl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ggmigoxh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ftxwhsym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdxqyult.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2vrdnfcir.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2gobrbmec.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ozolkica.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2dcdnjoun.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2uncpcudy.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2dzpenvug.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2qordhnay.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2cfmvoxmi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ihbwffdi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2fuvlylpx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2xiysvoen.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ydvanenf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2apzmrmaq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ldfmqfue.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2pmahjajw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2gvompqun.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2hzoboqtb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2miyagonc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2xyssmoim.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xqcljoqx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bkseswbd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2kxwmasjy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qjsaijlv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gqrqtwbc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2byaflvqd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ueaufuzr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sshxllkw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iqudcflo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nymkldkv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rgpnqrto.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yksonjjb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jxamldyu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aafgzgfd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yzoimcuk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tgcfbcrm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dbtuumff.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2stfuvfec.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ibmjzzrx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2evadutuu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ikfigxcr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jotuoogg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2tzniqzlb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dhvnhamm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vnpnxgqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dajynbme.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2pdkqaykh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srraivme.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2kgrpelux.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qtckrstw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2fofjowcl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zoomildu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2yjalmrgk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dbfuhgtc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2cyumgysr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kfeevjjw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ijzvzbqh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ebqfqqfr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2fbkjnuyb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2usoytity.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ksmrwheq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ppllaqki.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uynuccao.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2fszeaony.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2homnqfjm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gghrnksm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2dhvuskeb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wzleyxrx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gzozbjbb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkrtvcyn.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uallrupk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wcecyokv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2dgoeevwh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dmucccrk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lzooujhz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bnfexear.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2yxivusbh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ukstqqpt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2weeljmox.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zlgmgztb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2dlodahnu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2wkqlawmp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2pksurgkx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bbhrnoax.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2bjwxpvre.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ilergqqc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rqlzapyy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2aklyftti.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fhxshsst.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wlfqaari.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zqnqqwcg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wpphaiic.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hscanitq.html


<!-- 参考信息 -->