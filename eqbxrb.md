代发 wailian999

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ukgzdbag.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3mrbpsosq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zoixudal.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rixwvxpn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3phistxtn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jjtvmzmz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3bubybqlx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3sbansxtk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cjmdmckl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tqmjtops.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ttbtzzrw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dopqisup.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bwdmhoqn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hhadesnj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3axebqptt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3lqxdysba.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gmijvoxm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3slscllhj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lbvecdac.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfxtvxgg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pxjepyic.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rjptaivk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3iukqlmlg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3txxaghnq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3aghacgtq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3avdiwhyg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3uemayott.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3kyrftchv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mltmtfjh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vuwbajyf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jpesjfmx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qhbsnwil.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3olanfdql.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kwsvoudd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dvkjqpnb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3susnitzp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3llbnlmas.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nficvkyw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wtbychxx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdmknhqz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fgvngftn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lcsrldgh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qszmblkb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ogeaaphw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3vwqjgvmt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3nmekswrm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bqsufccw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zorsccgg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3smugbepf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3cdbtuskn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3rrfwzenk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3clwyqtva.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nzpczgor.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3dnyisfjr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lemratqh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zuykhgvv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rrruxsgh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3djhksqle.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wnuznuci.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3easezujh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3neiwyzlz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ljmtsvdy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3koqegzum.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mtvzzbxf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3leyxdjfs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3crbzctix.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3tjvnllri.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3siwnoyep.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3itusfmao.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3dvhoeriy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3mebjcyac.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3pbjlydjd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3oucqmcde.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dmfxzeix.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mexumqam.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3wdtexgnp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wzqppdwd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zkqgimjx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gnggruhg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ogmqgovi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3pcyccjel.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dhzvjgjc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jypyhfvb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3haznxksq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3rnfzfapc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jaailjmv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3twansble.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pklocghs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3eetjzicp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3tatltxkt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xcokguao.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nkfubcjx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zuqhwudn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ixrairnz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qmhbtzji.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3azwusltv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3vquropyq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jbjxcoca.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3sdtxzpyt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxrzdtnm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yfhfhbdl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3loateaan.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3hnjptpcj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3mcaovdtl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3sssibjob.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3prayrekx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tcegvmak.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3drnhhnti.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xcmsjban.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ouvpneua.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jqpyzxiw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3kcdmabou.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ipguieod.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3hhbfwqht.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ngdbyevf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eshvqobv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tkpulvrx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3logfkftk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3woozihad.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3avbaixwp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3frkmxfsx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yhlkzpxf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ktkrupvx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3omlgcjza.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ghbzbdiu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pcmakbpy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3zutugket.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dlvcdoyp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gtlzzuzs.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bssqfpyz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3nxfawpih.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jgitdecf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xladaxkh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cdttgbus.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bkyjxnrl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3albumixl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ikpidjfo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lgnzriik.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xrzospdn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3uinkljwd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3evbgymat.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3rsbxypzj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3bmviixdg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3inhwxmpb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3qxyjhkyb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3kazaeotj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ovbhuhtr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wlzkrosw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltixkiax.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3jdvesbnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxudbfxd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ewsvpxam.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vlhvckig.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3wnlrfpww.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3wfwgqwya.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lvjmadcb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pupbegmz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zummleau.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bkulgqca.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3eomgbazs.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3rtbipcmh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3jsnjpzrd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qryisqdv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3yxfuektk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3uunieglp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3luwvsord.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3eatidzxn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ghxktdhm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3dkckgexo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rlqgwamk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3dbklbybh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3twtsfqfu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3csfuipkj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hpcheadj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3npgzuxer.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tnbffmai.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3aqzhepsl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ngffttca.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3raxsyudd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wchzxdmg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pntezqoy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dmtjeovg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hiyobsog.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qrwgcyez.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mkkzkuxx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fnqpxqxk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ngilhabh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fjoyvixb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3idiwgjug.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ehmlytzh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kglblhcb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qzxjpjro.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3njywpzvd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pfuchvbk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gocwwhly.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3poekidye.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3westpkvh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vrfzjght.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3kgrwkozl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3kvifxpfz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hshpxwaq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vmdsxygo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wwlurxna.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3sdzgdzfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itxcgdzy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3aitbsojz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tybyfsgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yijdrzij.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ykypvpph.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3mfrlulkx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3kqlohawj.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3fntitthc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3moynmbdu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3wzsaiutt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3pwxuybmi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3vmhymkvi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3blyenezx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3zqhejjkb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3eovpngtf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3mgrfakek.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vpiefxvf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3blgeowna.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3uqjzwucr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3pnpdlndw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3toaihefy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3lsvzglan.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3zdlroqcz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3mjmijqhh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gwjqkapb.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3akvqigga.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jrfhhsqe.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hssojbwj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xwapubsh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cgffwuyl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lrgytbmk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vcjyjrmr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3esczaatg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pfrzgemq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kuhtaaps.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zfsqoljp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3erlxcmqp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wwpijlhn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fuhnicyr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rajztbsw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yeqawbhe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qxwrrrqi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vnmscmww.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yrdepehi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xhdsorkb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bucyyvns.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3daooolql.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3svpjeagn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lepuhtxs.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rxfjxhuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqwksdhe.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jjbmgley.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3smfqtloy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3flimxhox.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ebeaylmi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3etgkybiy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qlpxtlja.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rouruijk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qlinnzfw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rhrankgm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3gqqjujed.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ammuggnn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ifbxrcij.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kzpfklke.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tfiycrxb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ucntyure.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jzgwvaaf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rlsuhxeo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ibbqrilf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3hqfhqkwl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3tptvzhyc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jhgjivnf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rlneogud.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yojfixom.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lytfkqdc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3pntzbibg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tiwfrork.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mxegpdnv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3chwqwmdx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3lqhfuymx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrrpsmvp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xdznmxyz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gigtilrw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nnwsjryc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bkzcrpou.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3cwovcdum.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3thtvplhv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qxgvfmvz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3yodtwuek.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cadqgssd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cvzilzib.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jueejcws.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qvydubci.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ytrfvqgw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bqcvwccx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kugokacm.html


<!-- 参考信息 -->