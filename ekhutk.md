代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3akjvqlzf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pkjuwhaj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qakmbumh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ftwqmkao.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xjhuxdop.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3djsgocmn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3sbzpelru.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3iddkhqid.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3lkdjxtny.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3sbnygsrg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nsnggeiz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3fziwgdkc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3lnkvscxd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3uncnzmyx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3tmemgtcy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3azrzzqgy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3cpcpoagx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3yqeiergn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gprhjiyf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3btpiptun.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3uebxgrwh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3jhoaeagt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xlnxpixj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ndjkpwol.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uwzyamgz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uzoqcqva.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3sytuphgo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iagsxenq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dxvabuxx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3inhpqhwn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3npwpdcll.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lqvmltla.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dllokrry.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hkwynizh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3fhyfzyqa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3anoqmpcf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3lkjjlols.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mwcmamzt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pfvhinsc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3codfnxog.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rvyeipkg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3pvnblmhu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3zwdqtbly.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jlqhfsdh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3gvxeuble.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jmnosdpb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vrkgrknm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ouicwbmu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3eymdrsxo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tvrbotvi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dxurrvgh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3mtlmzrlo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3tancbkln.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tzbbkhya.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ewwlxjkx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gnhxbqmc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3otiluijn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rsbypnjy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3rgomlhlh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xzhrzqdz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xmummtkx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3frszrbxt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3orrptnzk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pjmljjhw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3uvlolqvb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3yagizpbj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3juassvik.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bzsrdctg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gajqwktl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xmykejdc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xyvpuvub.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gmupfuvn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3daduqamg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bywnkqzu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3vwutusvf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cebdctbh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gogqysrn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3amjgbcel.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dcrtlmli.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3psljvvhc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3olmgmrkw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fxbxmndj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rpvjhfyr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dsrvszhu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3oosovqtv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jsuvzpvu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ujdhclse.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3snpfjdbe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3smvcrzpr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qvmtnnin.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3lrjxiuho.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zmyxvpcd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wrslnffj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ckktxjmp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wihxqcgj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rdxqixhd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3nwnkrljk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xylhszvf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tigaicjc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3clbujtcy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3nsnhxwgi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vgwvkann.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ebrllmex.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ofjkzjyh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hqkpdkbm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dwprmvpp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3iqvqfcsz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ydpgrqvt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3fatfcusd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lrldeoug.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3dshefmlj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3pixzalkh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3gslchpsr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xjdmbzgj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vwmbeals.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3jtmkhxbs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vvzuzair.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ybzvwpjt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jqoieydz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yyphmxvx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3iqzjzxno.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3fmifyiva.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3gvzangio.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zphzqgoh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3kiixmklf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lyngnmti.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lsakzihg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bhnfumjo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ntbbkcwb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdonxby.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dzbreaiy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3stpjdzkq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ngtwjdjj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wqjxzith.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xhibvuzo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3qubfvqax.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vzsdikkm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3smzsynyk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hzeyatkh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hvjdvghf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dqzmnjdc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ecvefeqx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3uyjhsjiy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hpusxith.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cnargjcm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qrzbyyrf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3jvlvsaru.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hovdtzxu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vfywybpw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3vgnecill.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3tutvvfbn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ljeqluxy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3jojbsfjn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3svgjtvan.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ejwvtmmk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jtuzmftq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwlrfhwr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3pzyujlsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtkxftqn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ujtohwuw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zzfyzoij.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3cgowjtma.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tbgwhxzo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kdgwegpg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uoipzzxg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qgujyezq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xbcxghyk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mnsddtai.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3thcwsxxe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3jywyfxtj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3gsrtpdpn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3xriegmgw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3edghnmnv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3tcrotpdu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3thavhmuh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3nzgfgwzw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ttqvilmu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ssrrjvgn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3yrcaqtje.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rikfcbnu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uctrtprw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ouuoqthe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wzmijynw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3otlsrpho.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3delqqtss.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ciihqfnb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3raamhaqk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3egvierut.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fbublhlp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qgoxhswq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ahwqsibl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ndfuzahv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lugcojqv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qlixfdzx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3vsipbaxn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sylespgs.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3bizsuehj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3bhtfemjd.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kokcyvxw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3gougorxo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3fyefefll.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uhebteta.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hzzvddlf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hzkvbbnz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3axyakgxo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gbidxupj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3yzfefnde.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ogfrtdyp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3vggzzmvl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3velfzajq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3noamuplo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3iejsngrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnflkalu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3sajntmin.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3swrmhlbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urfciaai.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3rixiswnp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gwqcwaib.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3xxodchpe.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3xsoaiiiu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3lllgrpad.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3fatanrmz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qxgjzhbh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3uqhebkag.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3xiayptqy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3pdttzhhq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3evhcmygw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3bizhwikx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3rgrianor.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3tsgkxcal.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3efcbspjx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3rocivacg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3jokldrxr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3nbnwhtrb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3yafniyvp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3wjmiuipq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dipeacqe.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3rzogrusl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eojvmytg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gtcsntjk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cjmtaata.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3psyqtmtc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zowzjirm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3sbijbxzt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vlidovgn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mtyrrzvl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tiggpurs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3unknydrc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gyrtzgfr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pytgpyei.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3attmkrhd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vhpeuzxx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mmhflesr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jttlrwwk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vakqvjto.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ttbcdina.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3apknllbv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3nhrjuxji.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zncxonlr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cpkpwzij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfztrrot.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3usogtzca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bilqxzqt.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3pbstwejt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3uszgcgwy.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3cfbrvadq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mvrvqehi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3vsvymxfm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ofnqpiua.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3idbyutid.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3auxuhsdf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cubtpobc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3koebmruw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3zcdlwglp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qatpfwvt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kjehmuag.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pbvlnkme.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xhdyufqz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ykywezim.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3itjkyamf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yesjejjo.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3rewjdhxp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ejrhlstg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3niadtavq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gvlngpqm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yvafohwh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bxfujsgn.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3moepqvhk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3uititwle.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3guyqawas.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jselmbzb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3tcagltfd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ogutcwvg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jmcyorwf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hracporp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3uybvsvei.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ungptydr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3dhjyewvm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ostbltlw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3kbxkuegg.html


<!-- 参考信息 -->