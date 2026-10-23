代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ssdbbcyb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yukczdws.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bihodkmm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3zpibzcsp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qjgewryd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3hwvkvwex.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3degpsbgn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qcnagzob.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3tkzrjijw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3taflucah.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3mfayrzwv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkpfhjjn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ltpmhvbb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3lzmdrizb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfpekvnj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3voiswedc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ynlpejjh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lbhhepkb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gjybxcfr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vqsmwtsq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mhzopeid.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mikqpkjd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejsedfmd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hvaqpaox.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zbtrgnyd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3prnltmye.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kkxrorvb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sfccsbko.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kfmxhqkg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kzesbipm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ieczahpb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3bawlaefd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3bujandxp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3opqiokus.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ochuqfyp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3nafhlxyc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3yrcrznet.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3srznzztf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3omwwgfdb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cklvbwsd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3eteimrmy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rtgypeup.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3sywgahux.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hhfrvegn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3thfijbrv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vvhdcklv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yledoxhm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qrfjkryd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fkzvpgmo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3baieysva.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3eedcmohn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3sirrqhpj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rxyxxlbe.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3drqybbqz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3sahahwjy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3gdrzcchb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3cpaazpbe.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3llccapbd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tbuklltb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ntdmxqlz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rmvabkkn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3gmfvdqbe.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3obdsjypn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fhpokwmy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3odkgsnsb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gmzjcflo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rtfahpez.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3nwnisguk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ljvrxpsu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3fuaxehot.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3uvixmini.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3jgzsmrso.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3bwfirqoi.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bwtknrlh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rgsmhpsv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gicwakgt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3yucfhbxw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xypjgvyk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jywcvype.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3qibylxdz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tdvucqsf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3phrccyuz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3typbsvnv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3citdhhjy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ssfzvpia.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3tsdufovw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3oztjughk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3apdsxisy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3niznqbsw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ahkwhuqk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3tzclsmdp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3udshftor.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sgyvrmdx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wtwprqwk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3aevmnxnw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yawumuai.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hqpndmll.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wccnfpnz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vdxxalts.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3orooftij.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3jqyqvgwb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nsnimetv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3afdlykrv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwlysmpm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ssmxvugl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sycqynqw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jgumrhko.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3buzwjhbu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3opkeahql.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3iirhvldr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vcecgpmj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3pvijmdst.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gstsavpf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3rgswmoxy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jmgyuidz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3pfabmvdu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3aelzdrec.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3etpsgjtd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3cxvocwct.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ihamfbzr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rdjzlgan.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3asnjwsaq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ulnrladu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rsfntbbb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gsftybha.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hufcfqse.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jyrfdism.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3oaxedxtw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tfbpiotq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bbjfkerv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3upzlwfkc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3sxhwfewc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zgmfpduf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3loshrpjk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ecfvoziz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vivpabcn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wpvajxmw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rrtdwdzr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rrrwthhi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rgzkbkjs.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vbcqfizw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kctupluy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3xhnewdkr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sipcnsgm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3aoyhfjyp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3njxtefrf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3cgmgtgum.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3smxqjtlf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3oanqesnb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3snpzzgna.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3gzdqeihb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3cwirejem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etmgafea.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3pphtjhyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hisstjko.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3twvuxmqt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3afnabaoj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jzcumpro.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lgibumzz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kwtwaeoy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3eehzccna.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vhnospst.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qcdudlgv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3edvrieiv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3exksjzfu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3twpdnkqk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3qbacuthr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3gdmeffga.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ztsowtlb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zkrwjaee.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3fdcpbjxj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mwimicsu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3onghgiza.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ihsauhsz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lekobrdo.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kvgxhwzi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3clvtarzz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wkcidgqv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rvqtonyf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nlgdyfdz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3plqypmst.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3minblnag.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fjqrnmgx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mekfkfdz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rwgwmxle.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uamlfxza.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sncsseup.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yoizpppa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mjmudixa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ibzncywd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ttmfoawi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nujlctxy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3wlgxakrb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3imhiwapk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ccjxbmni.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3gtzjlblp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ndufqlli.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3deneigdm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3nqtwotal.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xslffrdz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3kdrekvwh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wwkyhmjs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3dkcvemcf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3zeghgett.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hvmljhmj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3xbdqztab.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qvtnxujo.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jwsugkax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3girrebrn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3relkoggg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3rexgcekh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhxzfcyz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3lcqokxtw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3srxbhxhx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3rwprvquw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ifbkzvxv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3cneftjgb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3kusufspi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rvmamebu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ymtiaayl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3fsksmrqp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3mqkfkazu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3jzzjtkps.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3cmhatmhp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ibdmufnx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3aklzpdwu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3orrrzdrx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3enaeelwn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3kurmgyer.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3tyzljrod.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3asqupxjg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3bumncjct.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dnvkymwy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3xhjpepuh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jrubnfhr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xqsfcqou.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ebgbunww.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uywpzuvd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ryyrfylv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jecolqyt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3estdbceq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3bcuerlna.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tjtwbabf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mguqktrw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eotoqqjw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iqyscehx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ovcizsmo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bywzvcqs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qyqbkoia.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yglkziow.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3urvraqov.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ggpsqwrb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dptbshii.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eiqzonds.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wkgcqdjn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gqdlfkfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnuapkbo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ykdlcufq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqwkpvyd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bpnzribw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3swnvyvvg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3vapjyqyp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rosbtwbi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3dhuxqhtd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qicxufvf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3yxoxjfkj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3hgipdnnf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oystpymy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3bfjzvpal.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3akvywihy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jxrsczjb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3iyvmjqjt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3vkngjrpt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dlbgymhj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3cgpblayu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3vwbgpjxr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pugofqll.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3yvhovmho.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3mcqpomuk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ewbkjiwt.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nhfrcpma.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bqlbdcsz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mwmrdrmh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3nrnucrbd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mqfzxlpj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zmvelkic.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3thdjhqdi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3xjowvfio.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3brpkpiws.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3btbfcgxl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3umhcsutx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jvmlctko.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3orvejfmw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3knuplszo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3yetuyqxh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xfvamctp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3bcqmjumk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zuhirgnp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hewsapyq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eckoazkv.html


<!-- 参考信息 -->