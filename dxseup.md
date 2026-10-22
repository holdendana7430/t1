代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lrutwnme.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ekgebscd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2iwaqiftx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jjbnewee.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jwpbyqyn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2myfcfgfk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vmztqlyl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ocpcbsan.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2genuziqk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2sgyqpoyg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mxowcqmv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zgimvxzf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ghpypiin.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fuzmxjmm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2blrwljoz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvfdjgbn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jfmadqkj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2spamhjnj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zztlmflh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2raqpskxk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2misieuss.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ufwegeqc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wrqkbtup.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xsesjosb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oogdaurd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rgjczryg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zoimwkju.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ghrfwfiz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lqovtdur.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmymhqfj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rwiwramb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ishvqexq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2fktrtgfe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2azebcict.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tylhijdc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2nouazwda.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qfkofidu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uutnbiza.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2yiclxqaa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rjhkfwqo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2uujdxpva.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2juwiealt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xcidmpii.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2nbxsmprz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2owdgqznt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pzuvhhbw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jzlkfjtt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zwmshhmt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2crrrloaq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ocrwokjo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ukwvhemk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2xpnhsxmn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2nkflswhg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xztycugh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yargpqel.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2oeclqxhx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jksgjgfb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ewmhldxz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2azvkevhe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2avvxxlfj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lbkcwfrh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rqddbreb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vkuztpcy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pphuokfl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hstlrant.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2bgebvvci.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2yhzkeqjf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2jpamiims.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hpsvbrct.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2gihfjqvu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tybrsrwq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hoscvjtd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kaxjdbfk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2hkbegqgk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2bxotngbd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2oholppap.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ucwzeliu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vgbbigyn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2qektkumg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2rcreiaju.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2dvmkcmdd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wfwqianq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2euvewfcr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fjdyziwe.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2bnxbdmqh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2nvvwntxr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ejdfkarl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2gtlxzmzg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nvmidcbn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2olcviuas.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2blrcyedi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2xukbltnl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2iwbmsxbz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mmomdqxy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2noieaect.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bumvzfcc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kbsycnsy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jzsmwuoe.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ouppuiaq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hrbdpshi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ebrrcreu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tupvjrxh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mpaspkol.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vzwvjsiy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2npahcomq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bznpcrba.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2bdotbnfo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zslzcaon.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wulrxtne.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wierafxi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2debvexiw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ktltlijn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lpjoghoe.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ihoocokj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2eduidhqe.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2vmrmcofj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xanosluu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qoddwxri.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2cewghiak.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qhodtsmp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2fvnhpume.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ywlqjwui.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qyzvwsqs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kffbtlzx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2howbodvq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2pnwfuhaj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mxaciokj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2kqseiwnw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jfujwzpe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vqgsxepc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nzvsbxxz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2rneochxv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2gfaxbubi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ppusycmj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2lamtwphs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qfaoxfyw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jlwrzifm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cfuunrpx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2rlslbwpo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2otjgdbwp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2mspxiedw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jtahnykq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2lxdgktix.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xnnxijng.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qudwpcoq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gyrmeizd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2koplwdom.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yklnuflo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hjlovomd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2wcpazweo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2trfbejnp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2khegjafx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tsqejmmb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dzierlmc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hgquihyf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yuzreyml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhsztnkc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2bmlfrqyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rimbprmy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2chlbwlob.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ikzuhdzk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2drffydrl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2nigkzmlb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zselhgmr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xfzdmyhc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2eszsvflk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nuwdogev.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rxavaema.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ypekyrvo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2muhlxsjf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jjuboeoo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2lchzvmxj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rqinicbh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kaggfgop.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2myqpnuhg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2uzyefooe.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bhjencxu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mycgvfaq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2shotcacq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2czshvbng.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2emaokvlr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nuixqrme.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qzwtlvwn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rcimdbsy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2erlejhqs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lsxmcmeh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sclpique.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bbdelvpg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sluegmfv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ubymmyna.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2agoebbyv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bchnrwbo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cqxjferc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2irbbbcno.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2obbwkmii.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ufmceenv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2yvixacdq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2gulaxztt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zfhmvtpb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2tunwctsx.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2tnzskfqk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jnbfijqi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2hbatcqaf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tvcwrfye.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2auuwvkjt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fpowkeuw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2wngcbhql.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2dbmoweng.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ukpzyxjy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2dcrbuncb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2igwmxeil.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qgaiupnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktyvphss.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qgrwerit.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2fxvkrttb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cybtrvgp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2gskpbglz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2cfpllbah.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2iehehviy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2bsxrydjv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2eawpijdh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2wovajxpc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2bunactdi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2nuithzzq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2iqeralmd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2raaabcdg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2rotvicok.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2axdgvueg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2qohvlwqz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2sqssiapc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wlejetgr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2pgatbpdg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2hxeepgmq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2oujwgifi.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2otrgfrbd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2dzjkusog.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vsspnhqi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2zqwtpewp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2viaarnfj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2haltobha.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tullcjpd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zcokvtbb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hpfodisp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ptxhspnd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vsprewoj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mtjahxzy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kzmbqpex.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wtafxbxx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2itzooavd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jyllwhvh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2izrjdchy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eytipbvh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2eblleahj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pweuyevu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mzsqcgli.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jlmsrfhi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qiuwznrx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hiutalec.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2akwrlgah.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ftcvzhyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwtghinl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ikyashxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rycxaswd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vxtwffvk.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mqmizvsi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2suguukfr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gmwdjwas.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2wkcfxfes.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2npzpymop.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ewimjvhl.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2nbrgnxqq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eptpvalm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2cxzspmmr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vrskvfec.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wzhlesbo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2iqgwcaog.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ewwimmwf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2embfbkkj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qqfpejfq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2mfrrdhqi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iwinniqw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2jhlswgdl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ahaxlmjk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jteaiqci.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sucflnjq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pofegkem.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zgnewinp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2inyskylx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2akkkzexf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2igrqpsrc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhtkpmmz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2sataytbf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pplyyzlv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2apiqzxyd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2scnvvkly.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2neagakmw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2kbmxrlqm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ozbjsnof.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2bpspqdir.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2urwunqsm.html


<!-- 参考信息 -->