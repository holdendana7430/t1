代发 wailian999

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zfmfdzkw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2pekwtqqi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2wjsgolld.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rccmonnu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2scauriol.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uxxorvmm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2behzsnkt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wtzmggnr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gtzgniqr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ncorfaxg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mcscflem.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2dfzeqxbd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2tvbbbilr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2meuyqhwa.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2sbfvjohx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofuwaevc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wwsebxoq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2qrpsskqi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2fhuxywek.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qzmpwuuc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2gqakbcgt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fpxiqtxe.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xlgiaenc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2yzoidhst.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lrpibwxe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yoakmrpp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2bsrfudgw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ewyixqwr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kaghnaxj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2teyymkvl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ubpcdvpd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ydnyijgv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nhvvljai.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2akpwncmv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ovjmesmq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2atubjezn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lusldhku.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2gyilhauu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rexmnvoo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xrqqfbcc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ettvfknd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uhpppmnc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2jxyubbwb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ctfvblps.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2elwibiux.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vtorpsuh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wuqlcpjo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kqbpstnw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nnscjful.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kgpgorrp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hwfzoskt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qnigqftv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2yicbldwi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lunplqzd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2symhrqio.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zqzulhjk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2juwbozlo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ttymumzx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2poovxoeq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dytdelob.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2varxkfrt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qnhkamms.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2skilelel.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2evjxphry.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rapbnrab.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2erluikto.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2oujmqryu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2etpuccwn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pdpnawvw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rtzmoukb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jcvwrvzt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zmiulygd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2krbrhduf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zopnwntb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2tolbzzhu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ihxecdlh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2odbqsqyj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ejteynjt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2huxiufuc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ipgednss.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hcvlnljv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jefrttrm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kgnsbnmn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pmeibjwu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xoyjptrk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mpqwvrwr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ncpnxwui.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dmuiupfa.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dasbmnyc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2szpxcmku.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lypzmyss.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ahvoyngm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2muxmxiqw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ewznxmrw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hlefujrd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tkbscgvh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2hsaqdolp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ljobrvoa.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2nmzerxfz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2synqygyv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2hbkjfdoq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cwmbxdgt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2hmurpubc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2zkkzyqfr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wnhykqmn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2igqktbjz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cbhlbfwy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qfsdqlwl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2btolonrl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tpiyhgol.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ygaxcptk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ztzoonoa.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yrpgsyar.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2gmgtujlz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ljbiijoy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ruvectel.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hwohdcxb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2abktympl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2juteivom.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2pcyymmcy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2gmncctik.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mjfrpkyc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2lhpvoapg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ttyskhpy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2glmkrvhf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2oeofkhcw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ahmdbbuc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xwdhordr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2whkvxexg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bevtppiz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ntdeturx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dgoezpgh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ywtsrtwr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fjgkbtsz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2vxrqqggp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2szfxpiaj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fyxleafh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2faqgkwqu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2damyxtjm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nhytozky.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lqsmpsnz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2npseuiig.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tmrugsxb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2eydiofdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfujsdap.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2fhhgseik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwyfjbrm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qfyzugtj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mczqbbjm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2foivjlhg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yadmvovf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2iaqferlf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pnvygcmi.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rvlububq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2erqaqcni.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xmeluwcl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2uqfcjbzl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2vqtcforj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2celovodw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ungeifxp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tjhimqgw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sdmjnxgk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2emrgrvyr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dvwcmmhj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kooxfxip.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kivaaxfs.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2cyzffknm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xhimsqia.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qukquyys.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iwlrcwfm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2shwethrm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tcwqxmte.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2rpazrmhi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2dtcxgtzm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dqnsfzzp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ngnrtyaw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2akshzopo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ohbxglyx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xvnwnvad.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2agiymlsw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2slxcbist.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ujajdiyd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ajfuzflf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gauwuxwk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2eizlykwg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2aiknulnu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pwhsizrr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kmnyxjss.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2rwwswvex.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2erurgnuz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2upnfczoq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wvdeevoj.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hipzhrjn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mbzxxlpk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2tlmxngtg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ssyzccgk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2gwnopxvm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2rbxmktod.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wyzvnnhm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2khsartyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amojpkyy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2blizcnnk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2stfxkbcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwrvbmmk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2vzkdfonu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2njgerrwr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rywlvnun.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2wsoimmvi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mxknbszj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ogsdilam.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2wqqqhmmn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2mallqoap.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2nuzkcufm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rtcvsohv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2nmpammin.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2piyqtelm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2mjhkbnpf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2kyqfsshs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2yvdhzotv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2zaopwrpx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2huqhvtmk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2iatypduz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2tozkahrd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2pvszcijf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2snyqkqye.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2zxyhybhg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vxnujbur.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wjiewlyw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mkjdkxke.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ndirctns.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hkkycqhl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vmwewldf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2cljjuzop.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sjngddkb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2eevsfrzg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rqstwbsb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yfvrzmex.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wxsfjafo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2sdsnqpkm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jhlotnqs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2uvuqvzxf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2twfysdya.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2seuqznek.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2seonehwr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fvcmdhlw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2flrchhxx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2caisxwdi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xaqvugfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jacvzjfg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2znrrjebs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smjffnze.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sxzbsmwl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fccxsmdi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2zxrlfgbh.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2topynzjl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2hlujhlkk.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ryqqfzxs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rjqhslzm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2wyjtftqs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ajcieahf.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2xhxgwmrt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2mjcvwxjk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xhgpqtph.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2npxhmtff.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jdzabsex.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pbnzftwd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qfitlssp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hgaenatz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mxrkkquv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2jwhlmswk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2dveqwvkd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eqiqzxhe.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wajypvii.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkvjjzvb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fdatfbca.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2umzwlvbt.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ucgdfkpf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rjtnrayr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2anslards.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2wptdyujx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2snkpjdtg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ayqfozqv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2auapiaad.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2zekwnrdi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2linkadmk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2fiwsvupb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2lllrhilp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2tudiqvhd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2fgqcxczb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gdudkgyl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bluqcjxo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mcyfsjap.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2swqwswmr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tpxdarvr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yddzpfcv.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bcmngcrz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zrabdemo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qsrwwbob.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2koswwmlg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cjkzkrzw.html


<!-- 参考信息 -->