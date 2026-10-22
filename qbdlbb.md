代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wojukstp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lwjpdymk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xrymopqy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2yoicvnfq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2cnovuilo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2outzeqew.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ekrdvxpb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhcywdcb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2skywaokz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2kpeyaqcr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2wltsnnjx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zfnurett.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jiynhioi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jlxuzlhv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2anpyukak.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qedqiinh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ogdtooor.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ngdyddkj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ttsgfwbd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mgjfggkx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bsngrwos.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wymimhdc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2zcrkpvxx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ccejogyv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2socwyqgn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ofbfjydm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zdxwbnrf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dndxewrg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wpnyshll.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ydlcgwpo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2srkedlcf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xlbsvqst.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2axisjnmw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zknfkqet.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xqapjxal.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cxmlrxex.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2nbannyur.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ghrhhpqe.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2unsnmgvm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kxbapcds.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2rzeyrepw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ebqvkpci.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2izlezpug.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gowdxfkm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ghblhzbk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cmwlujbt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2shsxdftq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pymmdnta.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fiweduma.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2axynaced.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2tdcbftdy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2cxdxucjl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xexmpmon.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2mhqpetlx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2seapgxfj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2mvdulqlv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2flzfyrwv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mwqwjlst.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xtoeanvx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2insyxdfq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ejmzojwn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2yvxprpvn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2pvhavmsy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ycalfkyv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2jctivxjs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2zthxqdqq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bsuradro.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2auobanmp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2aauxgngx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qrlmqxis.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2yeyfuuqw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2pemciwfa.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2pkwpdcyn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2occqfkyj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2stkrbvms.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2vqooemzy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2apnetytb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mnezpzjw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jswxxvmv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2cmcfccih.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lkgjxsdb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2afuwjnbo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xdcrgeho.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nyrhibdx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2lnysemle.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bvqdpxoj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2yfmdrdfq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ammgvrbu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vxxxdckz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ievmkvkf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2drkwuwny.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lcewtapg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dujwiqmt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2olrliaku.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2elnggcjy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjgbpif.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eurcqjpw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2cqoqwbzh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbgnlnhu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uiqpcdmk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2karkhgue.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2uadrkivm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2mvubyrkk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nnewmutx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ciqnlane.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rgmtxhep.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pcgnohzv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2olermqmq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wdevxbia.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2nuqctipe.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zkbvybre.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cpjksjxm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2mmxiulxc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ulowbmdb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qutqufep.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2attlmzbs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vbwytzsk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2izetduem.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tkwnerda.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2owjhnrpk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ipghymsl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2pdegzxar.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zguogcgp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dgtipuca.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zsktiwqp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xflcsueb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fkynoptf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bityjkec.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ghuvinrc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wovumscs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vgowappq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qudvseqn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2swzolkdr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tgvnrkrr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hzzjaavm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cksazabm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2zruzlieh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2htcoxgpw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jxwoldid.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2glawfgwq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2voiaoons.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dxbuygju.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2inkfsjft.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yikmufzz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2shwacaem.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ujgxmfcm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ymsntsmm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2evyfcqnw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hsfxvabz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2milwbpdm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qgabvzqk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2okzipfzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxmpvdfj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2bmsprxgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atbwwhlu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2sahfrcmr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dlklggmc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2wonwljvc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2jaqjfptv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xcoxrbct.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2soakxgoo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ulbqlukl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fhxmjhil.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bnyjnqkm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qjxwcent.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2nqenimag.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ulbpjunq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2aflbbfpn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qrqlouqm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2sbrrbbjs.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2tldlzuto.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cgdcwoye.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fbnwdiej.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cfvahxom.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2otkkanxu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2zvnlepiu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ekrkduzj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bsmxstyl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qhglziaf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hdkrolgl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ghgsqyao.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2knuhslvo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2htjmhnse.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ahsdygqs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xlsxjtzq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dxvebmkk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wybhxpsx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2exsqivth.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pwtizdkr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2soonhjyh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2rahzbtnb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2egsdrjwj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2rcfizgay.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qhlzuxgy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2kvjsdujg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2anemrcgv.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2nqxwmcxw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wckxwvwh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qghlgzec.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cbddspcq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2imkopvbj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ashxxfoy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2xvjqtnub.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jhkfgzxe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dlgmiibr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2nbxpijeg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2zpzdegrq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2peypnatd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdgijzwp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2bchsktrf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2yuevwpyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnhuwqew.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2vfhbwzis.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ljwyxkta.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2tikuerng.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2kkqkfcnb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2sevbhveb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2xxbkhxds.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2pwvvusqj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2haugphhe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2wlgkvqzf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2idijjhoc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2mycxlwbw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2kmkeoghh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2uyzeicwc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2awseozuz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2pvmjfnuw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2bakxxgaq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2qewzbcrl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2oasyxnpc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rmddeden.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2nfadcedc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mimexiut.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2etstxmwo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2guygwngu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2eaxvpiip.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hxgynpvo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nhhfzexv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ppwvdxnh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ftvivyqo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wqsocikv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gevjmlor.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2szfccdqp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2msqbbwfa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cwkhhqsb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vslzmjgo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dkpwrayn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hegrgohk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yxtpzafc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gjcsokeo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gdzjfzko.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bmqjernh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zfwgodgd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2djceufhs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vmorxzbo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rmpecgkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrtqhwrc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2fvkuzwxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vesjzjoj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2phtsqgic.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bkdbirre.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2avbynieg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jepzqmgp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ibjgltjm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lujddadz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wyaeqejs.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2djxpygfs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qstjwiqy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2jndquiul.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2yzuxewog.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qzngyylp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ajhpvmqx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jedntqxe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dhzroxtt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qhmqeyjp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2etynvchh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2myuhzbmf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2pielrbrl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2seginunv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iiafxfql.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qsdsqohv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2taealdwz.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sgordkuf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2oqrhsqtb.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hyuuiaoy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vuuwhngd.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vsulybbg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2evzmbvjv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qjhjwqiw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xrtarops.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qpjvoizu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2aawxlemu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ncwcogxe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2krbdkrwx.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2qzlqtedp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2dzvgvubn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzeiadcr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mbmqdsbu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xuxxuvda.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2svrhnslt.html


<!-- 参考信息 -->