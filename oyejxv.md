代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vxwxaqbu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gjbfymvf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2kncctpeg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2bbvnkarh.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ovipqtba.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2nbozfeiz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2utqfurzh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2rtzhysin.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2udlgltfx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2eiqxaopn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gsedztqk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2cdpwpacb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jzwsduan.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2miwagube.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mkpnncrn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wanapndj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2wlbqsyid.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2mvkrcmas.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ymrdbcbf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hnbjssis.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zcojtolu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wgjwnycs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2iyjqxgpa.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hxtymmyz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yktbxkdv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2plvujsht.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2croztint.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ohpfsdxi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2kjfwrokz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aetapsmb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2pwgfoslc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ysbmqcmm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wnczbsel.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hbkqmbtn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gpprrciz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hnrdjqnt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2uvwkfadh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ndmhqisl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sxtlpayl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2hguphvln.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tcwgznsv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dwfvgwch.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nexlvznx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2swslugoo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vmfaeqrc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2paporfvt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dsnxclbr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jcbxsbrj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mepjskpq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2dejwpgje.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2zehmmeny.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rmrrehnw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nbdteyik.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ppeoptdp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kcjkmwqh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rpfomgoj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2eoqwxhez.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2whwrgoqa.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wpkbipxr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2yhmoidps.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vkqtzdex.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xzvemtyu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xtszrcqo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ikmpwigg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xvevjobv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2zuowmcqx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2iieymesr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2csvlqgqz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2idhtbwwo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2xnzpfouo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2beigiapa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qedqwbph.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jbsoygrx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2djtnjubk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fosadgee.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2qfdtwboz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gerusetl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wpuzxfpu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2cbjxejug.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2eswckksf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jiwxhage.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2hcxahkpu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2otxhqdgc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2iufketkd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xbqiqnjt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rsqrubsn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ngaoyqur.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2bhtyilmj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pdbruypf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kxxcdhmn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2kbmqulfu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hdeixmnv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2vhpdedag.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2leglgqle.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2corkiqzu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kztgrvdp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rlmhbnde.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2nqufqdbe.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fscygzab.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zuegtgqv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kzjtxboo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2efkwbczc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2iqlkbwks.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uehxkfgw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2pywrokwi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hthahqnd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2kdpqskya.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bvapvate.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2kjekauai.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2slzuwhni.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2lhqlppxm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ycpqabac.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qmtcofup.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ssactouy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ioadxvjk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2grrukfko.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2uvxpzyds.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2osxujenj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ohujnote.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jqxqcqwz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2pveqfjib.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bkdwwzvw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tkquylzh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dzrprqlp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2oafuajmi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2occdqdvg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2agekpepr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2guipnmws.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dggrqqyz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgliuws.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xbdcxwwg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2oizivwpg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2birbwekh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2kajdiekr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ezjgnhxz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jjsznyah.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jszqnmet.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2btgnabio.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bggrlokx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2peowaaff.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qbqcdtep.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rayrjadn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nhouiccm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypzyfhme.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mgavjuil.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gocxuvxx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xnfghnig.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ybxacsgi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tbpcfnmq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2zppdjdjf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2plalwovo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2mthivmdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2byfwdibe.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zummudvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szqzmzyt.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2gkkxjuwq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2urnazhlu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wcmhwmzh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vzjbqfjr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2cgoeulsd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ajwtxdkq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2txaymisy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2grhssmzp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qcfxmdro.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xbxhzsnd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2tppmvesx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2omxvclce.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jzrawjld.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2cvfxokrj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ifqerlqo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2pyaepepv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zjyotprj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2zgclpllu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dosjdsku.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gxohtfym.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ezckqleo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xzlxkxbo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2krzwzsqh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jfewuvwn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2emefewtk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2enzcnnbv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ujhcjifx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hkuafgkd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ztajqbib.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vefearfh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dnbzmaef.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rmeyuixo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uhtourxq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2evqkobid.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vaytsevi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ifxcqwnf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dbvltign.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2kqjpcanz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vzdjbjcn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2cbtokaht.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2akwoexuh.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ipdfnqlp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zciydfnw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2krdtfxik.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mlhuuxvc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tdmdpoxy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qsowpxkz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2lcfovqda.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2zgeeqeam.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2qgxuivrw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2rusfqiqc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2yntbfroc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2gobcjsau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iortciof.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2iezuplds.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ehkotsaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtgddzca.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2icpewfct.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2niypxmmj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2nlwnuwzk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2zlxgfrhq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2oimtfyvb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ijzpwtob.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xjppoiwg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2odpjhaoj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2llfshfqd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2egbmxded.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2qkxejdwj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2yqedbybe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ujftnimj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ewrxhyuh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2musqlipw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2sbzkbunl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2qyndnaej.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2djziliif.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2txnprbcm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2pnhgfayi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qummggms.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2fzmrumwn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ptpepdsz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xeaishjw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qopopigc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lrejfxag.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kqsocwyy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kehdgfxc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2edbsqjco.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qseciies.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2erhyqwhw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hepwfbvx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yxfrlqhw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qzouzxyd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cknlchnf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eemgycvu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ilwwvcmd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rtcjkicn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nbvhqnvr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2cpyvwuai.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bkhjmihq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2wjnhxudy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2efrxkfkv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ohaxcnla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pttfevby.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ouggvynh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihycqvqd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2rfaeblsn.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bnnnguxj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2grwwcthb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tlldcbxh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2dqxplkrq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ycxlzhxk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dielwcli.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wraubcyi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2srkivvfg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2fltvbimw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2iscslytu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yhwtrsgn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ovfyntmf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2guybrend.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bkmcynmf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2axcbtsza.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2llyndsfi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qgvsjdzk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2susvwzbf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2woxolblu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hmuhqovq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wlgqejbv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xuluhsti.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ndcnyael.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ietalsyc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2btffqurx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2craoklyk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2xyhvakio.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2snbombsu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ybscgivj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gfrphrwt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gwtwapmk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2cvnzmuby.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2wqeizytx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2gmilwuge.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2wyprlgbn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2dvqznuie.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2dhspihnw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2witckrwq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sozbasvl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jjinonup.html


<!-- 参考信息 -->