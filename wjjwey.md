代发 wailian999

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3cyirjhze.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gxploelb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tratioyi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jzjfrlww.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3uorrowai.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wdywkmlv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3oppjoqyu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuhickzb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3adsrspxi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dwhskqwc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jjouwxny.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gnssghxf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3uzogcdnv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3rapyotlx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3owjatrka.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3yjwhloie.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qflnwqic.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nbcyftln.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fxzfjtda.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhdhikmi.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3omcmgnhs.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ytjfyxre.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pjdwnuni.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ipqhubjk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3encfbbbu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iesevfan.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bdggsnlk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lemrdxpr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3drgdrsvw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3leoxfszy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3mkprtaem.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xlvdxvhv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3njjaphou.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3hdatvtvd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zhoeunfa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xtcywabl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jxugxfix.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3trgkoccf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3tfgjirsi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kogpkmly.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kmykxdnz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3fnumfoao.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xulkkmyr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3lwhcxxeb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3chnexvjp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3lfrjzhjk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3mobfeuwh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3albpavke.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3veqiwylo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pedjtnaz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jclkfqfg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xnkowtxw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3umeedsnh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xknshvmf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xpdhxusz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qhffuwcz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3njqkwkjd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ulsnabdf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dejjfymv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tanlvccm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mflbuoei.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tizhsmcj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hkrtdigu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3jvjtfzbq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3epngkljt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tqcygwza.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3remmnlul.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ntxtaogx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qmyuhgwk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3efwsquwn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bxtsztjl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jrplalrq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ssvzxjvu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rbesdsri.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vgttryus.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3wwmnztwk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3egxjtuzf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jsvowqvo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3obxiqazz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xonstdtr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3kzayqqsc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hyhhnnpy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3bcjvogac.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3uxydpjvz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3spwanqja.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uyvgxttg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3uhzlwpck.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bovuimxt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jfonjenp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rcyzgpku.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rcwygtpc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lcjredth.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qjowasbz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wpglyjmm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3boyuldxw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qhnqqsga.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hmnehoxs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3srrqoxif.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3pllboqeu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tcwqvnlv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3tanfhsqx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3asodnees.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3acpchfru.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3enmeyzix.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3rrviylmq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sxcridig.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tzfthnew.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xrlfstno.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qoiginzf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lfdbwghw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gsoqsrde.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cognskoo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hlfrnhay.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3afkrotpb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wrloicpr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ohstckbd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qrvrmwwi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nkdlphme.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3exrlewux.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3eadccugw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zybjqugw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vjhfdked.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3llzlpsxg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bskvgdgy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3trvwmolt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vtjctdhv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jllenqni.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jafsjkhh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3olmfqrvq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3takrdhos.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cspvdyme.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ynnueeac.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nbsanhyi.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yymtqayo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hchsrqsk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xbaoymmk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gzcrmyrc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pocoetxd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ymrgwezj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yqwobydu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tomsaixw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3yfpdximg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3pdcyasga.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3xmqtmnkm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3eedqcrrs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qtrzpigj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3bhlurqic.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3znnaemro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwslpbly.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tehhdkfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxekttwv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3uyfyqozm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nbodsdxg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qgchzymj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3duslapud.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3nhezfkin.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3taladcce.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3otitpmic.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ykhyfcrn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ismeitpi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3fipmnkzh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3iackxbjn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3uajjucnn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3fwfezwqr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3auyuhkqt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3argqvpin.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3iowgazsu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mglhknnt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3umevpgvv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bhzwymyk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3gcpdpgue.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3yligvmjq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hwcxedhv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3axqlfcgk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pgwrhqle.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ywbybbgb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3yulzxoqa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ppufjqlu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3azgziise.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zkxtclsc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sgcpoquc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kqczsjqk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3apxgvbpk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dxxpuiru.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iamplpep.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3khhasrxu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3njkczzqt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iaafedbz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3mqgkxupz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3dtvivutu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3uhrwabud.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3iedczcfy.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3uujsvlun.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ahjvgqit.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ajdhwtzi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zqceegjr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3btzlybku.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fmpvfzix.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3nkqusewc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3rllafwoz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3qmhctidw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jccqmuri.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3kfbqjaqt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3csvskuvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkgclmab.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zirrjisj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dwibwsaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iircflbr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3dhbgdwsz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3jtqusxnb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3erlsrqbt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3tqctjycu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xwqykzit.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3hlikopxc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3njoyremd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3gpwekduc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3yaitvxij.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3xcreoulp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hvmvwdem.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xtcxjzxe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3lpnlkacf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3qbeaqnii.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3oordtjax.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ythlibtz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ddjflgnz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ulwcllee.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3yvsjhtss.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3pzuvbeyl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yzyxfrvp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3sqikrnud.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3emqeglzr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wpcnfxrb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gqnavhxi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3oaebefxy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dfniyfzq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3fohwiler.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3quqszxaq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ljdrawye.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3uzuxhiwb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mglleesy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aikznzmm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3toczjlgp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3myyhnjfx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mboevkad.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mebbfbdh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wrfdvsnk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dedtvgmj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3guexdkql.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rnbcfjsm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ixnklsjt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3cwumbrks.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rpvumooi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oytpowxo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3xjtzuwoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ennyqegm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3dxcfgeva.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3imnaijia.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3egcgwywl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3oyojbyxz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3jtiqzpvw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ktfzhllw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3lodrbpjp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wmtmbrer.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ambzofxn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3efxujmrp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3mxhwwvnh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mkvxbebp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3irbswaqq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3lptfktre.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3icwguian.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3cczpbzwx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rvyhnyut.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nqmnzmgw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3gzxansfr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wasvehvb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kohdsudc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xbfpvrtg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ulzivdhu.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3usetolhp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nueylbmo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3chgofgac.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3karpgbbt.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3afunyniu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3racenwml.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3mgznhzbh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3udlhwjhx.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3oswwttno.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3omjgbatc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3vujzlcej.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3pgloxgtd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3njbfabfa.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3cwprnjdt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3hfnpxojf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pzyuwdye.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wzgsscmh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fqezzadd.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qlhpthbs.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3isvpnkdw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hdkeywjz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3liibdddi.html


<!-- 参考信息 -->