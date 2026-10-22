代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qyazaigq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjmatmug.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2xqzuxscn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2eyjtckqo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2exjyymtp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2odrdabna.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hbsjjsmy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2qgbqodof.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2eeoylmrq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2pzmgfydq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2dzolmxgr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vtphjsdd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ksjzuosr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2authhjbr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2iugkztew.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hfqbzzdr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jhqungzv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2pvccfaqm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2tzhoolrk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2lxyfsaeo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dtqrsnhm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jlyksyuu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2evlrrupt.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iwzrhvcc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2emkypawh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kpdkncoc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vyxumwfq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mwljvffc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2nlhdsdbt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2trqhcefv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2incnytza.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xyybpwtd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2bortiupt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ttztvkov.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tijpzlhg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2uepqegzi.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2zvzpehso.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2gylegdkd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xbrcsnou.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2aoiuygmk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2spyjrkbv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2aavqlxow.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wspsvmtp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jorplkgj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tariunyo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2awyjbdoy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fsaiysjq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xclbmxwu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xkkursin.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2bodwlghk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2uhqkyfmw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2agmfdfia.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2begfetdr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kknkofce.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2oxfbwokm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2vsfemyqw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2zmjnkqek.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfhvxju.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qbfsoswq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2fveqddwl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2soklxmol.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rkmvgfrn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dcsjivbe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2cwlljilu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vtizssxf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2euxaxyyj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2waughjqz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2gtrzgcby.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kflmopfd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lujbitag.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ijjeesbf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2acjrlnwm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ccghswlu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2gcdxphct.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vddnklki.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2beetgetl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2odskiokg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gwwjspbm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rtbosgmx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ojmphsng.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xkzcvjke.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2fyqyfkao.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2oksygqvb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2sjwpnpkp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wvszursu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xnszftcp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wdiwnijs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2yyndwfvq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2yffebrfg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2johlddcz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dixcppjb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zgfzxejg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2alngeuye.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ipwboeyi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2nveefqvd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hsxqpgwc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tuzotudv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jxaiqbvk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xxazznbv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2sbcudgap.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ahznolwr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2apqtmlqe.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2mdwqkkoj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yzqibjgj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2fcwagakd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2llwxfwpp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ygagdhas.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jftdsdmi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2nhuomays.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2veymjqcp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ccruacfc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2xfslnbmy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2bdyebtif.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2gaihgyxs.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vwpfeskt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2heyihbsa.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2unmzeguv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2iqpitynm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2btcarqgv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jetklchc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ocqpdihb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2anpkmdas.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qqjjjhvd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rtlomfmt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jrhdatnq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjmgzqq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fdbazbrv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tiqosgnl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ahmairat.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2sotaslod.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2reozdfab.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2fyjeztqw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zilaykgu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ktiyhcfc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2jzalwxyz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zmtamjym.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2iezppylk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xdjcvzzy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pexeszid.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bhezojfv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vqgseepu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xxiiylbo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2sifzfupa.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkywofrm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bnrjvabs.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nvgamdqm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tacckkno.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rlktqdji.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xmthxdii.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vrrzlhgr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vzsyuqww.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ncnhqwpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocyfegfa.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2uyjpuvpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlsiqlmc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jpxzztwn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ttbqwana.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2bnpmmbaz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2rrkldpyd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dfnvpfpg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nbqgospd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2trxyopjk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2adaqwfaw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ctefbvdq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2cicmrtox.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ryhzaogp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2gwuihvsa.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rnnopngs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2omnedwbq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hfvaxhrv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2seljmsjt.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2oszbkbsz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2eswjpuhl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fgeobsst.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2pstlerkm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2bdetfvhf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2girzcerc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jbqrhxvg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wtjexuqo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lujlnjdc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lmmgjtvd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pvenvxjy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cspzrect.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gkqcjsss.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2soxedsmz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2oehghgqt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mkadosjt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2milbqgyt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bejechji.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hihuscda.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2dwiduxaf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2htkfquqp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2rjtlaxgo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ymrqjlow.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ejadkkke.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pzxkpsbt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xvvnigld.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2acqewsfe.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dgjntamv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kacwukwh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2jwazxvrs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yocmfsxb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2kcazpmdi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bcgintml.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ggmwydmq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2lvvfeugs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2swkopjtw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2cnzalljv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tawsvpke.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2smpvccao.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2sovueonr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgieklqe.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2vphpfjom.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2bsgbeyac.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2lwjbdxks.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2fphuoain.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bhvhqwen.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ggkdllag.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2vkpeplhx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2sbokpzlf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2kbeedqxv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rswhjkny.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2pnxfiqgx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2mskfqsor.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2onswlxrq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2czoaatzs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2inqagqnz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2vekopakc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2rzcgdqqn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2kvmdgofn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2chehvcob.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2tvjoxicj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mfrufvqu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ckojzshx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qtyeyfxu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2locsbche.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hvdytfiu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2suhmajyt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nhwlveci.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2trgzaykd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2nrxzxojg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qivqwkkk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tvsatiou.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ncrykcrb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mgxevufx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2whehzloq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2urghtivc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2heocdwko.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fbnstipm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2rmcedgwl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xiwhvsgz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2kyijhwxg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2uwdrdyoi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iwipofgg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vhwucnba.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ejwjqbrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wodvmaqm.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2grqufrvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwozenpr.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fhwtsari.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2srndxgiq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2yrjpktar.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zxdiamjs.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2sfmdjddf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xytgkrkw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wzejcrea.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2pjjpdxon.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mgqgrned.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2mllofoqg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2djwbmagr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lwukkcsp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qglolhec.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qvarlxkc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2svdzkdsu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2wanngogy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2kjxoldda.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2irxjrvyw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2hloueouw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2xdxzfnqn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kgnhtymn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fbltgyvo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uaxxdgbk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zmrpgrpa.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lnkzgwjq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2scbtefoo.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fjmzkbie.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xfgzdxzj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2qqgctova.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptptwmro.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2fahvzuvi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ihljqgxo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2erxxovnl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2eutjdefc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2gtocqoqm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2wuukqyof.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2lphaukmz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nepdqbhv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fnckrjwh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nszxhkik.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2neihzmhu.html


<!-- 参考信息 -->