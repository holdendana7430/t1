代发 wailian999

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2wfcqepit.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2yslzuzsg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rxqnxcbn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiygietq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2nhomjrsk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2iehfibum.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2vtgphsff.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcumlclq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lodbrmvi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2dqgncfem.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mxunuekd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bfhhqnvj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fkjtordl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2icrkswtx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2prbtwagm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xeyfbxbf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gnlenyhh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rqittpih.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fvuemczu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ubwlohli.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ngfalbbm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2hbrpsnoa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rlggvnig.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2pihflayo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2twpmyukm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2opajdttj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kprrvgmg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uyniessz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gxbbuqdl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dcaoqrbh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rqjpnsgu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2uethxcjw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ihfnrmuz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2omvmmxcq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ovvjddxu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2flvgbfqn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2rofwzrdp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fbtnqxyj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rfmtsbhb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2vxlabokm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2rgpmuunh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hqrlnpje.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2extuncbp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2lmistspj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2lltbvlfm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tmdjlblt.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2atjznljb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2agcduxzt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2anobaadq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2mvmmhxic.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2nlqfqxbn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2mrgxdigb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mbngxttj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bbrlhhyd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2erenqamz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2oznhlatx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2niawyfhq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2fvhfsbhe.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mlctzuoe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fqpdsxzl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2lzvxnudi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2obmudiaa.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jlshxyzw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2isgkbsjk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hxsnpfkj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2uewgytxe.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2uvprgsub.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2bphkmuzu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fugizefs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ufxqvoso.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cxmkswzj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2wxvqqupk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2yixafsaz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dafvfopw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2oregmkfj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2twcdiszn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jwfkydlu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vqzakpkv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2yrarvqea.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2hlzivija.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uscbzsuc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2oexhgioe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ewelhzkd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bvquyody.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2stmheicd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2toviqlsw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2oyccmloj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2edqmohya.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xocitvsm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ubkivuba.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ojrlloup.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2oejtzsll.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yywkzngc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pvqmcofy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qezyrksl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pltcuuoz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ehyftama.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lhoirboc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ohoisphm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xyzfyzvy.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qaazsamh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qravucow.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2iivudjfv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2injvblnz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ltetauog.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2mbguvioo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2duxixplw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2eflovswe.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qyozkzwf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2npvxobdx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pmfyynqq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2famrvchf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ecclklvm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2quyxxqsm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2rswcdwcf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tmlsvqua.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2xjkbhhrd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2uoutsgzd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jbpewwxo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ioecszpc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rkjhpfob.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lcudvzki.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2jbsbzotz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gzndujic.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2isdntypk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2npavanfh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2gmtxspdd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ktiodepg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gugdesgf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2byzdxhxw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kiuboyhn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ghrftwoq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kkuizhbd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nxnpgpkw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2yuffjvum.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbhltbzg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dalfyjkt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dliikrry.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qdyyxwpu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2grjgqhbw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gjdcizaf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kcjxgcew.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hspsiner.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xwphbuhs.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2amowbuls.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2pvuvuuyd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jydowqqk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ukxlrdjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwlyhctv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2sxchkbpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbdaqbey.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2olxkrbxj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2gzxrdqeq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2szbqshcu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wonbuhkt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wdgzmuws.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2iobasdeg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xuibqlgi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ofrryluj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2iwqzdmug.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ouaijbmc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2cxhovihb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zqclwnel.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2gjnmvckl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jklberkj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2johygciu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2owytpdcj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2fcztujhg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rjjovcgg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sdmiqedj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fspnpcha.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ahfmpdxv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kywumslv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2slbjfbvt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hdrekjal.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yluaazpy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fftulcoy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gtkymozb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xyniaqew.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zdnfueay.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2estoazai.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2gxyrujsp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zgwkjewt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lzhiroix.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2srhwoipn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2afwcicgc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ohtvlfqw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2huafyrnq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2bmkowecl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2tmlyqctz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2sgudfxpe.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fnbywnhv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2qqqdjoql.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eibminqa.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rhaugzbo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zyaqzbts.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2pmltqnwr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ombbavzc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kisckaks.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2gjvgerww.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2bizhxdew.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2fbujjngk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ljljxlqq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2urezsduk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnisruaj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2kkfmniqe.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2cdrznphz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibdqpjqr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2qeorlpfg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wmfpqxvj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2uysijdqf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mgtofyci.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ohxxygzj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2qpixjgwy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2yaarzdcf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2uytakqey.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2tdyosrue.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wdbqjexe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ucvmgasf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2qqyfnmjx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2xsagsdyu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2llgddqai.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2pgdhltjg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2vteulnex.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ttmkzkxb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2hnbzkwtf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2izlqowgu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2pkcbkvqf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2auwtkrqm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2gdnxhcfa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iogrhalc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nbpwuetk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fbxzafqd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vgtmcjdu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ivbxtncm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2thqfopxo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cvcwzngu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2flmfrczk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pdyjxjtj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pmlsgohi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nvlqxedr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uvbblddp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vbtsylne.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2spdzsntt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nzllbphx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ypffbdki.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vfiohika.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mggmoqvr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hnxzxfoo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2acjjlyue.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tjkevaws.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wcugjocj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uakmmdkq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hpczzvlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyrcqcuf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2syyvaccf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gdyyukep.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2uyhzdwqu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kdxrmjkl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2pemlkpxf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mftoyvrp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pcljncvn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2etinawhx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2erkinbot.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2eolgzvuj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2pfwwkkhu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fvkpvyui.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ajyvxojx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mdtnqrlk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qjxfighp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2optuufym.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2xtrrupls.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2acopyshu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2cjcorbsn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mszztcap.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wazhfvbx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xiyfdfxh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uhrdkhwu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2epqfnpdm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hlnkaskq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fqhmlkje.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2khskkxbn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pzkbfavo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2zjtbpeqx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lvgenfof.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qnvtvqbj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fcxjbecy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2jslmpvmd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2kzjjomgk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2dncxhdqb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2tjwidllq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2bvjhwoqp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2rjrdlutn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zovucidu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gqhehmmr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2suncqtps.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uzviakht.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nedrhhsq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zstthfki.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lbflhove.html


<!-- 参考信息 -->