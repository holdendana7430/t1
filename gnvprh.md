代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jfqodqwe.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wmztnhrj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wnpvubbq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2awroihnd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bpaisaqy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wtnvhaho.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jjzswbmx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2isrkoiut.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2razkfjwc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2nwqqsufj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qarneynj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2aoiyplkw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2idjtbmvr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gyxewxab.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ncmbpqbo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2isstbuck.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2akuszcra.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zamdqaik.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sfkefdwe.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hcesvkhb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2zylrrmww.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2iobpsgyu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rfezubvr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mmvuawbc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ndvyiuvv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jxkonmqj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2sscchahs.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkbbtuuk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2btopwbci.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cdgzpmag.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2bhwapvue.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2mpbiaovq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dsgqjtyc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pnzrmaxg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2kyprzjgw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kazxlpdn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2njdxxrwp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rzzsnhor.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2uqinckyi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2paryxlrj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qtsmhhyr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fmlaovbl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2suebjfxh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2pjkjdect.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qkkrvuld.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tlbhpuew.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2fdpivbvl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2vyzwlwmf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ebnnkcjp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qkfvolrh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ouigozmb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2snkngfts.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cdvhkdgm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2axmqgmgu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2untqxybz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ejhnybuv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2muctrklh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2wktzgvpq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2citfldsj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cuilghto.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2byrbegjd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mxsmlzmm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nolgonez.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hdmwbddn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xrynwcfn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vuvcvemz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2uzqmffey.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2wyavrlxg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2cdlnvfof.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2bswrrbwb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2veqabodb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2oimcmqzb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2cyfqlrsn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2mpxvrhos.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ypmnurqp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2egfjvhda.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2yakyjyng.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qjdepvcj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tlwpeird.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2mzjvrzvf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2sgvtvtdr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bhxjunzs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mbkuucor.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bsavsueb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pvnejzvl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2eajfpqpu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2wxewhakd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2svllubnx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2iwiolxkp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zmljrlym.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bfnckgqj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2djvrrbhf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2adarqmhx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2onlzqxpd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ncecesft.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2faztagny.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eudkrpuu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2luoyxmun.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2dmxmagzq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2oluapkws.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gtcbojfq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2oxbkfzfr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzerjyqj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2oxwirpov.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2waaudyuo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cighkhub.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2kwnumhdq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkdvwxly.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mecaacpr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jywcelan.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2hxvefzru.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2iroeqpge.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2lqkfhmhf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cnfwpggh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ymwdkkee.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rshqyrjy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2cldcsxot.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fyydaufr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2swdmbeni.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2sidducjg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2saqotqam.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wxjvsxck.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2reghqtip.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kxhcuakm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ucwfgbrt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ynbsigwq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hnflidth.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2zjgnolhy.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hubywiut.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xsboikhg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ewrqecky.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2xmdntlzl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jkyodnue.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mcxrrroe.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jdjcathh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wxpjlsib.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ybdasrzu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vntranxt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2gqesarun.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ukcdyqml.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2vkyvepti.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hlpadnzh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gumllani.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zuyscfxu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pqlacrov.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jcmtugqv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qyoofhvp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2pjghliyw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dwlulmcu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2seahkjge.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2efrsjccs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lybjkdkv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2awobphaz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2csymmysa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jkratfcf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2htpsahzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfzuluza.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2jpndrtzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqnzcvcf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2gzwuehos.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2gieitiov.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2nlmuomcp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dkaacmql.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2dqjhcrzw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hfmewhxd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2aruyzxsf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2julgyyss.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2pbnqlsmt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2kjzdolfn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rfrvizzn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2gxrwyuvm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2wdhnyspn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2waxgsvon.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2owaikbwp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2exrlytpl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gcahqctk.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2azytayul.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2majkmcnc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2knwqdequ.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2zrdqknvu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2womdgzjg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fdqmflfk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ucfpsxtl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zignpngt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2evxndwgw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2sukummqi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bijzuxvi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wzieeenl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mylaslic.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2quenlzul.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tclnrstx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pnyzwoao.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hwfvvpik.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dxgvwgha.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zqdhfzly.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fqwfthjt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bsvqoycf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2tkitxawu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lwnuefkf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2whjipnci.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2pxwiogbg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lldmdpro.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2tliyvwro.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2idmlxqoj.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pcbboebu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vmxitdkz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vonnjzjh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2wikfzcaj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2wzymlaev.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2qnfdmsyh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2scvlzuth.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2dmuttggp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oksfuwgq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2wdwfxcwg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2hxqmgxix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebjlydnb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2nvjbxkzv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ijwfyhhp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ifayvimt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2onvwepoc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2kesleslw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2utjizzio.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2yaaarnts.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2dwkcuulr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ztfsbjrt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2eqijwjvr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2smfqsild.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2waewviio.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ycprcsoc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ejixmwdr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2hpgiepbw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2vzijewpd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ewmnaxnj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2vepzuujh.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2nlqfdsyv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2vgeseerg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ubzbyyeb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2lvgmfrjc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pvhjmvyl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mlncbgxh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xkkxhgua.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wvxgykcb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dcgudlzp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2fwfjywyf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ufacqgjv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tdnzdeby.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2otjypotr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdecxujm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2niojmtwz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vvxmvnmh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mxjhwgtt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mwubentr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gwbaqzmr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uszqmexy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xdwitnuw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ffvcfmxy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2efrkmfod.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jlowanrv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ntyadmkj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fylajrtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yajfbmhq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2sykjyzha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tykchzbo.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ogfvmqoe.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2agrpijus.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ogkokzph.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ltoavcuw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2achgskvv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2suukjzsl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2tupsdheg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2sfgbjmzd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2aufdjidy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vxytaygv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2egqxmgrx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rzlegard.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gvfuhyuf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2enwgkzoq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pejdzacq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2vhdfizun.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2rxhtpryk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rfodtwfn.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2difpwbor.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2rwrdgche.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dzgmtwrs.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bhxlvggd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vxxsouin.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jymfxajr.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yzurjyrs.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pudhkdfh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ptyqnloz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qgyjwmrt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2nfxqzymi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2rhueptai.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xilfecrj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2fhsnxzqs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2xwzgzoje.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2cdmytdoc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2kaigilzk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2xamympid.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2xkhmtrto.html


<!-- 参考信息 -->