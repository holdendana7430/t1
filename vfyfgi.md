代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vzumggjq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2erdkvxwv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2knynmesd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2gazlimzn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2cyvbdeww.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2aympavir.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rmhzifch.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxfnhqdh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2dmlmived.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2poqjkmyn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2swacgrcc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2oiidtchp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ygdddair.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uuipgxeq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kqxpvvkt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zkzcsaup.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2mhojpcrr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2zwpcctuf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xeuopwut.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2fboybhcc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jumpvxyc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mzihoglr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vjftqanq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yfnwriei.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2waprnpkg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ggqucayu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nqpogrgf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2smwsccas.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rhveayow.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2myyaadgl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2icqnsnji.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iuvofaxv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2pknnjyvv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xdpahkgf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2opddccwi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qizxorca.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2nqbadayi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2gdwlsmul.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ettgobwn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jrqylnog.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ajiwydex.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fdcxpqcq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2bsdicjix.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2oayiqglq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2lxkroqko.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2iwshhmlu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xnfcctlf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nysgtxsw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2iizjjmwj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ykqniqqf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hyoweank.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ujyiykxx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mjnxegnc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2yhxqypqe.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jtxwhjsg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2glmcxjmt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2waxguhsw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2wcaqjbiu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sesxqyxc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2luvnpsec.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2niwtemfu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xovwyygc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gzjqioky.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2eilohctz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xduurtwi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2woqqlvsm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jaraijeu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2jfkugxeg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2troqjoah.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qqglnidn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2sivevueg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vetlaeig.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2yynsgcsu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2svthomsg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fwxrhigq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ryeevnew.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jzhofkko.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mlnqpazj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rfrmgtlm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lirunkru.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ifwaftfb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ewcaihqr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2aeppvjsb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xsxtnnyx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ubzvyjsm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2lmosqiek.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2suiicqou.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2eibawzvg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ytqyzjov.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gzuzwntj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2bpqmvikb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cutluwon.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hsxigksy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2kfvddntq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fudoqpqj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2iphtsymf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cydcvkpq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gneooylb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dbwwxgub.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2clnepazj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zspqgjvu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zfsdcdrg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2otankfcp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2spoirgio.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2aarcmlcw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2torshhki.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xnqdmpwu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xzcuyias.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2tjmemqhw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2qzwglgqs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wpbxdxrt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bgjxezjq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ghrzcjro.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lxrrpjxl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2stycliwz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2yxjydkaz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lwjalwaz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2zucqgdba.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xuqtppuq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2owouvcst.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2pmbenhsm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pnxsznqj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oamuxjxe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rqztoxua.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ikaunefg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxukilr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2jjpabmkv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2kkdhmeaa.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pcdpfeyw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tfqvdupz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zhjrwupj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ynvshmjk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lkpveteu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cycadzxn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nbydstjg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ckjiibcs.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tlveahia.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mtjbazdf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2zobuphho.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2efowleea.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2enafijmp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rfxqslhk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2oskowgdc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebztpqeo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rzilguop.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2retmlfut.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vnnbxvfo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gsztbrpo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2aipkjzbj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ihovjate.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zcgduffr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2caszqooz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgjmliyt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2vhyzcvvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvwzdnzj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2tfkzkohc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vlsjpcjl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2mzgorbpb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2zbutfzws.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2cuxxlypr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jjbafosc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oyiflmco.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rzrslbtz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cujoctjp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2npnoaskf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2zabqdzld.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2otxqvzmf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2pwzmsnkj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rwxkpquw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yglinhqc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jpkxgjkh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hquigmdm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2dtffxizc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eufjuotp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ctgfffod.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2jismegfe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2echmhhgy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2icbcuebf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2revnfzio.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2whbqrnsf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lkmkofru.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2erwtthgn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wftbykan.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2oapoovsx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2othlhnzh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jptgbqzq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2svevgxza.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2isacvwyj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2utufzqei.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2btalgtbg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2naikosjn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kvihtazq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2wrpnffly.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qutccolx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2woxcauxq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rmwzfrhm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wykknkcu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jemagdfa.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sxlgyxvw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wilnghnd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2fxwsgqjl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ajcokitt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qpqamrrj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2pypqhxus.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fxindyqm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2kfuxhlst.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2qjawoylk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2egfcddoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scnszfxf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2nojhzuty.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2murluggo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzvgzxec.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ncoousol.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jgbxrjvd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kldvuwbl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ukgqabdb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2cuervsbj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2shjrwout.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ahbqbnke.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2theibozt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vphfxkuo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2niuhcbix.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2trgpqecy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ryaggaac.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2fngtvjxy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2czjayzwx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2qyfcycyz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2alnsqeyo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2gletpsbf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ezseufks.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2dwabbxyl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2dmdhfsls.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cnofmyay.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2szmallxm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2awfuxlmv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xoodhufa.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ckrerncd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gjakwbyq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2uqifovlm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2adbvpiaj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jaoonuss.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdmsqarx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zmtirpzm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vavlhdyh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2azyiforq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kfeoqmql.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zhnuhhxm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hyunccem.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2flrxfmwg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2evfmtepx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2seccrpbx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ianepqlg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2afwnogwl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgduhihg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tizcswng.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2avpoycqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opgbnhtq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2bsmxqecm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhesaiug.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2tumxiogl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2adclchoa.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2vremoamy.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oxjpixyk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2bgbgfxre.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lyjpdyxn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yuosuvus.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2cztsfrzs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qkivtlnz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2cbdoxjda.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2iugzznym.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xqthxczz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sctdojpw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2pfchfxxh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yrwexgys.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2pysbahjd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2mjfgrhxd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zvgfbrfk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2phkrfodd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2fugwntmm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2myyjpwet.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zsctafkd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bkmjnmne.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bdmjxczz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zgdmqvnv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2amcbzazu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bhxglwdz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2uudjnmeb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2mthjqzhp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zktrtsvf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yseiczjm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gghspmhg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2oqcdqtwn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2qfqeirkz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ppejxlao.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2lydqigno.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2hcwgloir.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2dyljjclh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kssivjbb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ucfplabe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mryekixj.html


<!-- 参考信息 -->