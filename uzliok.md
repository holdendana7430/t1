代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gvtkxdga.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3qzypucya.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3uxawdbyf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jtyaipjv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3djtlxhge.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3dqrqlvzl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ntuxdtng.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3zzutevpk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ssgyszfo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jkhlhaai.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xeezvara.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3imgporaw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3lixyicea.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3sqbwgifh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nrjhguiy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3yuuisirp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3gdfesddj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3iqjptdkd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3mrzneqip.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3belnxgbg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hpaeyqgh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fzgemfau.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vaedcdzn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ecsqqjfr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bbftobpv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3nfgnzpmr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ixsrctta.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wwkkuahu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rfdpoilx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dorfoiop.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3odcqbebw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ecybpqyp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jclvqjcc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qxofnkie.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pubofgeq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tmdzntmx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3sqqluwzd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nndomkzx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rqwaqrqo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dcjvxaah.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3wnxpxhzs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xinyetzq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3lxbeqfto.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wdnasaof.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hcnbeehk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3oslwuznw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zbjkfmtb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3glaxwwea.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3iuwmrbky.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cqoruxkw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wmgdtbzj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3amtqvlon.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3sydathth.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fhpywmvu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3sszdhsxt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hmrebcog.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3jhcgmqln.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3nkhcddwg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3fpbfeelh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ildskegx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rjceljob.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pkraowao.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3urmyrdmc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hkkkizzw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zkyjnbot.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3sjwsebtp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uacfvcjz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3voqjlnhj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hrjgsllv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3yfmvomhz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3rrstttwx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3tjvcymiu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3zezcrkoi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3zqnpllrk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lqviovun.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3arlydsge.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3yfnluwbq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3istmdurd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ydgsrnwg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pkzqlcnl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3xzforfvi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3fqsusjyj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3lilsnunx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jhivzfti.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zfrldahq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3muaruluv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3lvdaqacq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3glvxzwuf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fqshfujd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3rejeqejt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3sbgnogku.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cyvxwcdn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3zznryqjj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xmamygli.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3hpqzsojg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3frgtshzz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wawzhzmg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qxpjspro.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kgjyweew.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pfacnzgf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3icobcrbt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xuwycsqo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zgepdorj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zqezyydg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iznujhid.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3fvrmofjg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sokdskvh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xrdalesg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3vzjpname.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mbcegjhi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3quqlaymr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nmtglpjo.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3sutwvuqf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vlpoqzor.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3cmkdpyhh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3gmraofzl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3uvpigaiw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zdbbvkyc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ajyuxttv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ecenubyi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bvkxfaxn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3beyjhqvq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3kdmwncjd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3abfqgrrr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3tgmzdqic.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3wgwxfsvt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3yklexqrg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3huabkgue.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3eoeexowe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3veqvxipq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3imqwupiy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mqoeazdl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3biunvfgn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hyantzmk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3rulflkmg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3upvxpadk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3lukhfdon.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mmibuxho.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kkpwnjdo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3wanchthb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ztgaqzzp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nqlsaycm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ydlidnfe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dasjrlpr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3bwlbfzag.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xqzghzib.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3glgomqfu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wszxubma.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fdctjyfj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aylvbbfl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nkqsiffg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3quknrmxx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rupppehl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3bwktffqr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3fpvzupcg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3efkpoxmb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3gibgjplf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fgvurvxu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ysryubra.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3cparxznb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuceklah.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3dogfhpbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hghrelrp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3herwjoop.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3onfngtwv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yhnzloaj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wpqdmgjr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3uzrgyfke.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3henubfro.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3snwooewc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uilaclok.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zbygtgal.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3yrdhgyps.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3cmmxtcze.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ganlaxpi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lwifzyhx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3fpdpsugv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lncvbzqw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3svkounfg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mtubmska.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ycifomvn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3naczwzcn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wzgueyvz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3netfevqz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lixyafnv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dwhlgbpn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ueixjiwx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3elhuwlqz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3zvwqvbhx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rvqqlfuv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kuxezzoi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3umhzbyef.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3txzsehpp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vjvqrrbu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oudyrywu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hmfcqjul.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3imyyfbsw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zecmsjip.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3rzgpoxyc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vfftzwlb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3yoghxpor.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3vmltpfeo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dotoyuza.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3krzoymsg.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ntgpwwev.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rjicuhiy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3gnrksfwe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ibevvafg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dnycygmm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3njgqmtzm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3hfqctipc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ehldaqgd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3znlhuryx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3bokhtdmi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bsdwfqed.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3rlnequfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hieuvgep.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ohqyyxow.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3eoprnetv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgdmrnoy.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3salbzvay.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3bwqaezrg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cnhiopmn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3fmnqsxik.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3soccrigp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3tclciucn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3mlvdaclm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3rifulthx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3lkpfzknx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jmedchou.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3xzsjobbt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lsaettdj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3eshkxvfp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3cyifhuit.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3xpkorjar.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3gljelusb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3xbdiwsdv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3xmitwumz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3vtwvtalg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lgifgeze.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iihwnrts.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3itqsvqqv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lxijjlyv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sxtfoyxt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pxyrbdqo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fpostewd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qvmywyen.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3fimuargu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mbmscmvm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3orvuebjy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ggyzilev.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sxpcmlvs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tycvhnfw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kplvkvja.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eieevkfl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vsdiluzi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hcugdtbz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3acxuzokn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dskcibgl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3kdrtbpbx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wywtznff.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uuuzvkim.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rdutjatg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zywoyyjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oeomtspe.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3szusksvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nobrzhui.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dsxeiusl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3urbbukrl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ezmueouq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3puslyais.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3dqnujddy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3sdkwjoov.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3uirnqabo.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3iopoftfb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qyttgype.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ryhuhqlh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3jiatbsuq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dwrxuewz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ebsecfit.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zfoibabu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bxoiqiwc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ljxaffgw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3alukxzkm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3itocbvtg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3zvgerukr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3zeojcjzq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fpekroil.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pplzwfti.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ajmflapn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pzegnpiw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ndlhnrei.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vrtufyxf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pcrsjbdd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ryhwhkho.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ktbrjcqe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3mflwjqci.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3lfemhbyt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3uptctnyt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jyxengnj.html


<!-- 参考信息 -->