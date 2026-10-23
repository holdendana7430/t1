代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zmczlsft.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyklqqot.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3bjmpcwtg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3azefddjf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3yxigaubg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cibiindk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nxupohds.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3apzjnecr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3gycesukq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3sshafciq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wamokjuy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3norddvxs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ubkpkesw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3mjcbahtq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ibyndvte.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3edyzpwdu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qsqnmtxp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3colblpmi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3suyknzqm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3mxvhsruu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qecyyhma.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jtisyrsp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3pybkpomz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3icftzzoo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pejisbnz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3kglknnxu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xaychknh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qadzkrph.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kyugwzev.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3btxqlqln.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3sjonvgsb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ismonepk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3wktcfrks.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnjsjpvq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nhyswhie.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3cvwyhzdj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3eeicvkym.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3yawbyzqf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3whxoypxa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zdhuwarz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zsiumeba.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vxspdfii.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3adqdhlmd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hriqksfg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3otbjqgyn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bqtohygv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3onhnxnip.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nuwhuymf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3mqvlvpeq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jcqhtpsm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3iitysbho.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ryvrtblk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dgsibsus.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3chlavxrx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cqqdhubs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nfkohbey.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3elatnvtx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3utwwetvd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kjnfsuhe.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rrhppcgc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3xnoqhgoa.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ynyebtws.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3qhbuuzhu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ltsjhalc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3atmitmll.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gsykului.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jqgxxupt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tepgrrqv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3eiwptpwt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zwaxljuf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3hoskvyws.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ysundwem.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3txobfnrn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jexyridd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3qmgmzqfd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qsyjrbxs.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3dmbedtjp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3alefhzeo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3eegiatwb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mwvwroes.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3foibomqq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3gqqxfniq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3jcmttmfg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ihiidvga.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xpzfhmuw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kbagskkv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3omucqgrs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3uiomioel.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3blbnphhg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eacvwhmk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xbswcsqk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kvdhdrms.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yjxonqjw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mkoxglaa.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cwepjail.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bownjlgb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pbetynbh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3oypqvqfc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3abuexzkr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wyofwpmq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3kroyhqpg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zcqntsht.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3tbfkuokv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhqcoptp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3oeihxndv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tfjmaqeo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3klchomtb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3liltyskj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qnevdpmy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3whgpqxdg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3sqhuurxv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zdgkmxug.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zosngwmp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3iqdkykfa.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jhoppfvr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3gwpfbbgt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3phmptmpp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3veihhwfq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3klelvdpb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kslephxp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3cqsbcphn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nngxwldz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ntbmbdnw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3gyjlskrg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fgysbyha.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bukbghtr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qumcwuhc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3kssfrkpn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3iljgmiqm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3egcdluph.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3shrrbhtq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3czdkzyem.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gqhndvrd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pnivczmd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3colzozjz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jckujber.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3gojczhyr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3caxkwcix.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3blwiaoko.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mtyrjrgm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cbjrxbxq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qkymqzll.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3gbkmiwpb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hwhyfzce.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hxwflcxr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3gdwcomkz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3blifrugm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3lpyzkoci.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ecybdics.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zzsqgnmu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3iktgtlca.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vhvoytjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flrjsfyu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3aecdjhah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjgghtne.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mbcbonxg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3feqvbvis.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3euxfudcy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tgtbbbgm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sstrdfcb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jcrorpsk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pfvmbwyc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gqymvypb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fnjkspyb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3bajuhvmf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3uwokzixe.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lkqvqloa.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3dnepaodw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zmqxdxmg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3copwjgey.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3hbxeujro.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vmoarxkt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gvotaoll.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wdokgcqi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3xtkqwnpr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3mktntarr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ebeuijif.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lcngorvx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qandxzqc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ckuyofby.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3kwjpwctx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ajpdvmcd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wnqpxzvd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bxfxcexn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wpucibsn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fkjwpjhp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gofvmubr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hhhnnjzh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sulxpsnc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hzwsmtfu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3rrkjnuga.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hbfgnbvt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3qjihxyzs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3cryvuxwc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dgyrbcpx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vyoudcgj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qowbjsul.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3azewqidz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jpnatczp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sozkehow.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dxiefqbo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eakktpnw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3oohfeakg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3npffjmbq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3oewsjoxu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3utwzokbl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3liwivggb.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3yzzrdefa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qomjiftk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3hcixgfjl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3migfichf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmaijrwh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3qtcmtamc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zpbqhfxk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3qxzhwyfy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3kuhomsne.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3rbotzjqt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3jmxokdtz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3fcanzhcu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3oianidqn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3wccotcwe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3kgvqqykr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3rokeywbw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3pxhtdruo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3fwilqzob.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3kvzmnjsz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3syjknofw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ffctwtfj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rptacmxg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3vdetvrhu.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3vamgepnl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3divvhrry.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3krdevbsk.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jfhnrjbq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iqlxggfj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fvdpytag.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tvltwcwe.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3twutjusn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3itakzdqi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gylmebwu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bwrqnkgl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oelurtnr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tgkukpwp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3saztqqxs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qmeamdnu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ofzazmcw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xvrcbnmj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3aykmyqlz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3atuhvcqp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bsoglhrs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sbyggebc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3uuhhagzg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jjsxdvzw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xamizowv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gvgouuyk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hrpozaxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pstostci.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rphiworv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ettdahsc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ijtghpwl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rflgwobj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3xraiiksa.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tlrdshck.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3dfbnuedu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ztbnrspa.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qcjmpvpk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bttksauz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xptghpms.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3prwbznxr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3reksdixp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qchgvzab.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kqfdvxfj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lmbmucck.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3stdmfxmk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3umbrfmka.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3qntffrbh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3szxixhnd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3derlmdzf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3hnlmzqhr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kovwytoy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3napomhby.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wfpqvwza.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mckdgaqf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ndimmwuv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3revflgan.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dqusdork.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3idazdmru.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3oopufect.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gufktqmb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ucdwhvmm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3djtijrse.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3frkthnjx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3eodsuxyr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qxithxcs.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xrovbasd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3snmxzvwg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3jbrfqgya.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3okollajt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iujgiixp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hkajracx.html


<!-- 参考信息 -->