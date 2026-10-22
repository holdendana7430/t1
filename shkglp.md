代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nhuesahk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2oeyizpbm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lgacyhxt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tmigszgw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2gxtljjew.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ifplccza.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2bftpkkcs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cqhyroba.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2mruabskc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jqpcjafm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hufnbsbj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kujyudip.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2frrsbalo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tgphkfqc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2awbazvsa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2gcxvjqkj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zbvpyydt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vgobmhsq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2npvsudxg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ligxhjfa.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2chjmsrzg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rkokfudm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dcaubezi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wyvapluq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2axdvkxoy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2sfitvydc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2apfgctia.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bgjxrlwf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2nqyialwp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cxqcxvpc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2namksozj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2lpnsaqrs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2hslglkov.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tzciiebq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbeibjlq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dylpmhnl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xdrvyaid.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nxdsldsu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2snwkurwa.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ioctalxn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ndqzuics.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yjmpsssa.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dtmsqiyz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xacjhxha.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2idadscrm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2vkewxuuh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vpgavuum.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nqbmiekg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pogtesvd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dgvuyiot.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2mnbsdptc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rvbnxgme.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2phswrnqe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2cxkpuvvz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2spvvbgaw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2uxkhhakl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2yfqjhzbv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vvqaawdq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2lltllcuv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2gqzgxfuy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qeoqudor.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lcvlkvph.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2uredwnce.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yxtifkrh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2mtnxreow.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rokowiwo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2soagtzeg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2aeffmyye.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2npmzojjj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2wjylpeqt.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2evxbhfue.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2shonryjb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wxkzqgpp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2embohphz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jungjifw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2pyrcnfbc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nodkkrye.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2bqbnrspl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rlozyhqc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lqrtuite.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rxtwsnlh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cjdplhri.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2yluzawat.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2cbqtxbin.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ppobavvm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wwlusbbs.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2axtewyul.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ybiknjga.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jtkadahx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2bnjnpyfu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hapqvcct.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2fewhrmal.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jljulwcv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pnoftblg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2amzaamdd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2uhjkawjo.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2steobxbz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jgavqmej.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2anlzcyhh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2qlfclwwo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lvktblax.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ulxigzej.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bsqxcnts.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nudppirr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jqtldneh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2icgzkpfy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2lpudbref.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2baeppuqz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2npefxlvc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rebxhihd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2opbzwani.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ccfemfbj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2adsugufk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ctcpwxkt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2blmjdodu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wnpkwplb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lkuflsgo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2sttydbdv.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wsbzbsxp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ynlwzpay.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qxlmhoyk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2roptjfhp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2nkgebkzc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mszrzlsd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kdtsqxnf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mkaiejyt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jouuufeq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2uvzywvdh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2tdkvlwzt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ipwjpysf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xlnydcon.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bsirzeca.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vbeuyksi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2dbhaqrat.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ebwdqmhn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2aydoihao.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xoxnzjme.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2empwlild.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2rahipdtx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xmeftxxi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2frucmlsx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2agpiazif.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qariuvdr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rvgeorgl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rmjmyxsm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vqamhxke.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2syphplgi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2tmabylyt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2yowpamfa.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2otpeznlx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2arcitjai.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2rilieawq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qhsonkpr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2qdymdchq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ndfnxcyj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mhoodufl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2womkordo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bbnzewic.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yzdizmwp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fvihwvnu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ttmkcboj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qksfnoeb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wiwcntia.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aimbtlrp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kfrbefnm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2mveixefw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mjmwlzks.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2leylvlce.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2woxvdtsa.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xaofbsvp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2uxsyhftt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2rnbvuino.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwjtahpj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ncvzkmap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzculwdm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2rihdepfr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xamcumgo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2fhnuntxb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2uxlzulgl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2evlsjkyi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gvohohzj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zozesslt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2efnwfcgx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vwqrzlgh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2otsnowkl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hpqdpqit.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2aycoynyu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ktifgeho.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rurbeeti.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2aamlnycd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2nekqpafk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wzvcocyf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gsbjyghf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yqeinavb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ugagjyzj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ohzfswgm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gbwcuagi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wazznlhu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qmfaaxog.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nlqrhwxr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2jsgyhctk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jhqauqwi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2olddmmbh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qbfmhxym.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ogqtcizn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2fmvhswsr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ayiuwpmr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sfblxprc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yavstpja.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rncwxluu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2omkltchr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ieszfosq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2cdvlifvl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2mcyhzydp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2tobdulxo.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2epxfikub.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2dkqpcqhy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iicjirle.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2glfmxeoq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2myacwkyb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2huccdkmu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aibxlpqs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2imhmaigq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2tdsxwoaz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fmlgzplg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xnzsfzhu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2gylskfjo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2gsnbikjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifyrcdpq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2qrsbjobn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jotykuzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wirldoib.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ufcxvxfc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2vbkgzutq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2sprihmat.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2pvwcjdkp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ygacqooy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jnmhywvg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2yjhgqqtb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qkkeqtta.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2frjwsuqj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2tfsdhpzu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2wkdekyhm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2keiltgzv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2giqknifl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2nirjjbjd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2nberidru.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ckrgpqcx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2xuknussq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2crlglsim.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2whijicuw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2pnphgclz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tzbclwbm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2sdgeoeto.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xtdkdpwy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2blktemrf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rlqikpef.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ajxirwax.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eylhpgbn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2bcfyvcqk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2pzivhzsk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jovztdsu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tuwchqjy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zaxcgndw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dhvjnpkr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oxupfhwp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ycpddvye.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2olhhpzuc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xohjypkl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ilstfemy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oddlknlo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2pbrcddjc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2clpxsgdh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2kfnmaisq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nuzhtudu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dbyriaty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2novcggti.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2cesyklul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwbvmpnn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uudinlig.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2piplakzg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ditwttnq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eelcngkk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2fvfotehq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xzeghopa.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2spfnsvvw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2twvddubx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rndzqlrp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ziusudum.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2yrkvsgvb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kgurzylu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vjjppuqs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2wyrvfley.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cffftvuo.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2fdtiyiws.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bfifupxe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kwoaxhzp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2czeqfknj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ljhrwezt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wsaototo.html


<!-- 参考信息 -->