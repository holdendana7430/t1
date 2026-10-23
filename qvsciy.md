代发 wailian999

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zdzknosp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3baynxdqb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3rtnqvngq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cygjhfhd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dnupcdjh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ayutabim.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ootkqrlz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtljwldr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cizgmvgc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pfskaggu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rvcbplld.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3udxzzicr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3arbiuzxw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ocdptkgc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3xbiicfao.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3tfsqqpaq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vyuqczkt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kgzmbvkt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lgfeubxs.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kbuoglsr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3umqdlrzk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3yksclkvf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cjywpyrv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3yozjxgxs.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3bgejpyyo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pprpxyga.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3secnxziq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hosyosni.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3fzrnrike.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fxljtbph.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3slpygowv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wppxqnel.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ocnsojiu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3euzhvkgo.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jcpsmddu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3avbguzes.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3kbjervmt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cjdtymzn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3uwrjesyn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uimrevua.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gkjxlcsb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3umftxlio.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3luacmfts.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3yhssszfd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fpbrairi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3uxilfgfp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lphqbeuo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ohbvjgra.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3biqqgabb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hhwziygc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zyglvtcm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xuwdrjyw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ugfyhjuy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3tlqjvipk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xolnqgxu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3linrrfon.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ocuyztow.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ginuwklk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fpmjcykn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3molezgtv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3yxadedlk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3somnaoow.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wclobvct.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mrxaoowx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3samcltxv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3znanascr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3dutwvsnj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vlykrpgk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3istrgloa.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uoamtfqp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3nemrfcpg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qpcnhngq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3kuzyfvgo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zenjazzm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zuuokvxs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hcseulkt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3valiqsea.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rkgqryqe.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ksutlcwp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3abbbbexm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3cqsjfknu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3feosiidl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3othwllxv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qltycpmu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3htaquruq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uqhbzuip.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3coiozqwb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3omcsewmr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hnxuaqzb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3bvbdatmd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3isiyfoec.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wshaqbnq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ynwponga.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3nddxgduf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gwzwoojy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jbnqkpst.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zfbcdozg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ohsxegcl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3zqfrydqt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3isxqipbk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yxumpxbu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qllrwxel.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3deqomswu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wdrezmdm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3epgrogoh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hcylgqli.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3gbmyzvim.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tdnijgfw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vivdgjjk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bninfhir.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ajcxhdvv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3duqyglee.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3faudidcl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ksyhlycz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hqpyfkxz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vnqkrkpe.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3junvaijt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jzbiomoe.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ybkyhbjg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3nndvfbpa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gdwoldgo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bhujrjvg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3tuzelynu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3kkssueyg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lsaonkkm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mynlvnde.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3mkgbmuiz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gkkxzyfx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3golnpgyh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uzkbqgbn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3lskfqyms.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wlvytorv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ozmlgfvp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nvndftmu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gvwyblbp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qzqabawl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ojubgacd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bopdekso.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3cqbjropf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3gsdcdqwh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fvwxpmac.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3yhplfujg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cazvpzms.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bcqlhslt.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3itzrlmhv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fenfvubd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3fwzzqrad.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ysgehvxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmtlgtwe.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3yexwxadu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upxpuqvn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vcyduekk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ifiodmwm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3tcxiuqum.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3nawcirbc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3liqoixsc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wwqvdpom.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3uzbraojn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bzzuyoev.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oflhtizs.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3gibrnzps.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rmlisedm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3puylzlsi.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rmcfavip.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3svexnupl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3lnkbszgb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ntaopgjw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ljdsqmys.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3byyaixbf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ockactgj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3owvhouyu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ebznvbzh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3sjhwlttw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vjnfiflu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3smsgxxpe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3glyuduow.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3gkdemlht.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dlfhjrhe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ajcxkmnh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hyesvicw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fqxikgow.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jfslorzo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uugehpge.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rqupczmv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3spumbqaz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3scalafmc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3azuigeat.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hyafawcl.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3fdjbuwll.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ftxcqzfs.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ovlddhgn.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kzlzmhnk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3zvadrurv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jmzgymhn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ezysuuzb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3giyukamu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3dyaysokx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oibbuftf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3cwfetcef.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3jmlogkjh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3sqbroart.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3crkdmsrj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3eftrczpa.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3nlzkxzvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldtyrmji.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nwsgqput.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3fjbchcks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzfpkiva.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3wmxbfsxp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3fiwuigxu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3soakxymt.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3qgpstagy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zyxnymgi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qpznkqgn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3jlzxddwt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3elpxlrpy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3fldhmwfr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3uvezljpy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ivnddnfn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3bpiozmzk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vtjiqoxx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3maukczho.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ksjkjjkt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3jodqicla.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3tbmocteg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3qcxfvklc.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3hratrgjz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3hamoovut.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yntbqcaz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3vuvgqpee.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3eiipabbr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jqetmjsl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qkpekiyw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kyxlugai.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wpsblcku.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3pbudksix.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vkjigbeh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3snwmmkaf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dmcpboye.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ybqqkryb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3txjtholq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rizpcvrk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zzwylgdq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uscesrni.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ptweyhiw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ksihckot.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fysdfcrm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3aebnjeax.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wrlrrqeb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dgihyfur.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3owqnelhx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rewcdzku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwaeczme.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3pujczfwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajqzhiuq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hpfwgjkb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kkqccyrb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3wxzxthim.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gntmbehe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3eienkkhx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mmafqnju.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3swthikgd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3otnrvxjc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nyyxorui.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3oijviyfy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3wmzbpwxx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hkqmbmpg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3htddsuty.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lnfnyiuj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vqwdziea.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3sannbbch.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3mjjydhde.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3etjiugym.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3usqtfqgw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3nzxptqfe.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sosukqap.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fyesaeat.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qtjgheya.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hvupszht.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cruogxqk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hjksfdda.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dxatehsl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3fgoxikpd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3gvsgtmzd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjgnwiow.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bcftiqpz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cvmxhhkb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3tnzpipbg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3jlcgnqrm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3qcbneaoj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3vngttapb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3vimdcmnj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3zfjlfxao.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3febkxlqa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fwsrqdcp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rdhbfqzc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3syrczizl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3snhzpujy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rzbxjxgy.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3scccfjqi.html


<!-- 参考信息 -->