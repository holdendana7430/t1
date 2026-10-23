代发 wailian999

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wclzjfzd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wywzdaqt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3lmqoujdd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldklwymr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3opsckhqs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vxpwkgoa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ysvhmmzd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3nagdnweq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3oqbxzhjt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qewjtgiy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jymeftvg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tqloqeve.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3whztgnyc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3oputewwf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3hwtviqij.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nxcbdwzg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3qmrbndeq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gbthzvjw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3guxthdbz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yuschqiv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ozzcbluf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3yexpfubt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wywgspjw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3awuegqij.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3yaktfier.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qvecbdxj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3arfwwomd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3scmcehzt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3saqfiygy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3yppfyzxw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3evawvoop.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3lskamnli.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3uebswwzt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3efecmkrs.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jejaeazv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3zveavsat.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zlzylkzl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qtiqlwje.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kkfenics.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bbvwsulq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hdsqjvjm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ywqdukuq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xbylptrl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3sewotqrm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3jycysgce.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3mkjvckpy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3cvbgvjde.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ddsihyxq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nclugyig.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gqxtzelg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3isbmzgqd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kggxjtdm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rfstavgn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqcipxi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qvbleewa.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ikhniisr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3puxzrcru.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rhvlqhfv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3jvlxsrms.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3wpaephmb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3irkqgyzo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ffeqhxgg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ayzgyhrb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mfexfguy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3mvjnplgb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mkjzffiy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kpfqdqvi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xjmklpzj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xchriyum.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bplnhcyr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ahnglell.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fvjigkyw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hnbbwadv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bpcyeieq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xueadgtk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zxbpsblt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ulfiklom.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xlkpyqgi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wbxjtkdp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3nvadaxmj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qjhdqhaz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ovkbkjgv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3imadiclu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ymjhuesp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wfzwszrh.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3obayvngz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zwxqsnqa.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3clmeetpa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3fjornjfi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ahrbgbuc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zgrlkvna.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fdfapooz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kzexmyzu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ajbbznzy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mldjmyob.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tykafsdc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zuzblrhv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qmwabxyv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3mtepqrjp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ekckffku.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lwjmkucp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lewnvhju.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dryqtyth.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3lpmhhdjh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fidwczjw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cuctunee.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gafxzyrn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3kigznize.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xfsauxta.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3glxnchdn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3fbzlqtjg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3iawoljhx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ydaioaxr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3opcgfksl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3tutsoabh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3znmixbgt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pswptser.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bvixrdpt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3maztzzkn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3dzynorbf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vvtgiado.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lrhejott.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3wndrgibc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3lrcblpnm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3daajsjpl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sxutqjdf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3dqcvppwm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3obdjgvea.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3frmoqjiv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ynoqvprq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ujtwwiys.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pannpoas.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3lyjsnseq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lbxplwdr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tjsgwbsx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnxfcrg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ddhjtlvo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3glrbyvnw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3daurjlma.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nluojicb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lpmjwopp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ytmfdhye.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3sjzfylin.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mifiycfa.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ebinddcb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3hvgdnerk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ohpklhib.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3byeyvjse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqsmkeda.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3rxvgkfdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njgoiyff.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vwztmske.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3thvroxoh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rtrvfuml.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3gtdkfozq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3iqwoktzm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nkvbmayw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hidruuis.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jpkvxsmj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3akolfcpg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lcumnkun.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3geoxrrkw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3bqnebkjx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3nqadzlxs.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ymgoqsmn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ogckywyn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ajpuwmge.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cwdwlroc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3scesearv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uizinwtd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3byzuupxe.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vvizthew.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bldyalbj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zypfqfas.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vjysfkhc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3cuquxssi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wmijmebt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pgjvsbie.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mqjgolxr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lxqefbwe.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kdffksmo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fixteqfz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dloldpky.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3owugsale.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fbfomoem.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vmnxxunb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3cxkoaiaw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pippdgcv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3gjnliqjp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3dpvcgrak.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3sregnrbj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nlyippwf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3pvmthxva.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sxganptj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ypvxkzwc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gdozcmeb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3uqslxxzn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xgreidqv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3abuvqlua.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3orlukkal.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3kutpddcd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3tixkyity.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3wdxzwvoc.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3tddpivmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzsmeenm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3pzmqpwij.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3zvgoheph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpugssmh.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3apotvcsz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3buznmqct.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3vxrbpswv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3hekyhgcv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3wiofwqrs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3clouaacq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qapehdaz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3rdyyvepy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ikzvafbq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3akvohnhq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3dlkhgfiz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3upefeere.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3adsjgnfa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3prdexhaj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3daxapyvu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3kdmpbmdp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3miwgnfoo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3hfrzlrrn.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3qaypxzzz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3cirsefjz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qnxdkdst.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3kepafxln.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sxqscbku.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cipigant.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ebbqcany.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rxzudzoc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3prfuvini.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gzdgwhon.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3pkftgxaa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ydrlsllu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hoxczxix.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ipkschxk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pdademrt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lmzckbal.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yghtelrx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3glougdhw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3arwgksnh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3klaysdnc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qnqirybt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ncsgzbnm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ekejiwua.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vusfddyu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fdmokzic.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skpnkcrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsbebtvd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3jfnofbqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqdmuexv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yzkpnwxr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rykqfsng.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dpkzdtow.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nlhskhbt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ydfphgck.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uhgiidll.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kdbnvnwl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ewoqeats.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cjawekhv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vjeqltex.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3itnbjqht.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3szjjkiux.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3swouabpx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jmgtszpt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ohpwuuwm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3rkyaufvj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3pvnjpboo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lfkrcgsw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3lxzojblf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fmqchvov.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jwvsqadh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bhlnhrhf.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wrlzvtcg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qbufztdv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wdbtejii.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mafgneyk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xcnpphsh.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sbtkvoqw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3myszyluh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3evppbqvb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yumsxogp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3pzjzxmnv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3bksohmdf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3togthxrw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qyfyoxev.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ilmxrmtq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3idzmmbml.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3yssqtfww.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xwybdqks.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xqsmvjce.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3usmyedpr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3znjuhojh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xdtswqdm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ybyldprf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hohspuby.html


<!-- 参考信息 -->