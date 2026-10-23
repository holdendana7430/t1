代发 wailian999

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3aaqppgbv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3aupgjczl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3gxpjxkpq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3efjdcmga.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3zoguchib.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3pwfwaajn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3abgnjajx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vjjxzzyz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xbbfmsjc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xgomwxzj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vjewwvzm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mxziwgxy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zqdxodtn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3glmgbmlb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3epztznib.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ydauphuf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zrmludcw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ylyvsiqe.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3uzsqtbxr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fjahnkao.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3avgbxjwd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tmdieliq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tblkgjte.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vlyjbkps.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3zmmzdvpj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dfyxqbia.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3obbhmytp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmbcwkii.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yfrvqvge.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qnxjuzyg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfgsdmfg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hbzamgnr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3njfenajg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pxkaboyj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3izxhpyiw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3gxjvvdld.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lgxvjoxc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3eqnauwpq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jfdrfpew.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mepirrag.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wnhohqit.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3esiztktm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3orhiezfi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3yfendcmf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3iuxhlkmy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zkbsjxxj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3efawlwcr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3afnclqfk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3suvpngds.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cydqcnpo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xexuypjs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wstljzmd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3sqojsnrr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3hblhqeys.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fnmyvpsa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3nhamqfxv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xtjagxca.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sbkhiatz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3okbyjrws.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pxtatifc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dfgfjzqx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cjethlvb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zhtbzzrx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3tbqbzhvm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fblcnhsv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hqnevclk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3hzsgaxvw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3axtinwdm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uzocmavi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lsifzemt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3sgyhzbpc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3wdyrcfxg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fwuhifxx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3gdpcvezk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3poiumsbl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vziyjqxb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fbinoewr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3nzxysxus.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3crxnxpjg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kyigovmf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bespfnfm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sikonmxk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3awxrafsp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wdmiuaki.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pfnsfklu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hncdfutn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cvdoufqv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wfrekxps.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3tncnkfsz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hdfuutns.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3xfxzijdk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mocidwyd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3imozmjtd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3sbhlfilv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wlwjsrzy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3pvhrkjdc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qqwjenol.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3bngninxx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3icmdyfgk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3zkmoiiuh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hjpjdcrr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jbhtuwqi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3yuskbjfg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3rpuaurkv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3svkpohuf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mbepewmx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3yqduooco.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lkmzstgr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3quyzwulb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qxhvwnet.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3iihdsmze.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hygvqnyq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ooahjhcf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3dnookzcp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fxsivmfe.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3swdnknbk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3rxfnahfn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3eqokcvwv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rqqqhusx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzucgivm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xyytwvbp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3naajkdny.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zqplszpz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qwlzfhve.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3vmirvtmn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wzgevjjc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rrhxmsbp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3iwjiokwd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cqvtjgqb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ztbfsjeu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3wceawooe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jglnpruq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hobnlfkz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3mzlhuqrj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3chjdgfte.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qzucbwob.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vpywgghn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3emdnwxce.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gjjlticz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3efuazbbs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wefiputy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bbconhfk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3yocczfwu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ltbyhxnr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mmnrywfk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3iimyublf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3apguzjyc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lsdusscz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vtdtnmsi.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lgkwgwuq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3waffjfdt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xoydtciv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fpihcjni.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wswjfnwh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cytkflka.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lzynrrbp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nnysxcpq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wrfnlsho.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3liofwknc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fnvswixh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cdagitzp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3oqgydnri.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3fmexhiqg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vuvwcowl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jhnimxrg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3txniqplg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kxqrwfur.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3mtqxuqzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeospjgv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ehgxayop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpugacmz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gsrhevgo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3gdpqdese.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3xrhgcatj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3gsxstbsu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tmthktwt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hebsmiyq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bavedxqi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cbsctdtb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3sbnecidp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ymqruqkw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3iiichlwo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3kczxdptx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wscnxvsy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vvqaadiv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jjffcdfw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jkfbnvfr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tlzmnigg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gmmksnuo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ldjvujkw.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zgswjwvd.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3gssfyqci.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3nadsaizp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kmdnivwr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uvhmexob.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3muzlfwkn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vvbukzga.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3brmzjxlz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mapxkmqm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xzijhxxk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xfxyabba.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zhakgijk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3krxqrdfx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xohpaskq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3weammbci.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3okyxyftr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3srrronea.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xqzizjqb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3tzfoypoi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3nimrttqo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3syilkaun.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3qyttuotq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3tkcgdfli.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cijyezyt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3nmrptitu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fdbavodv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3fbldcnvv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bigpkzih.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3kkbuldtk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3yrzqydvs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3nnwnsiiz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3aarnrany.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3dcxmibuc.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3kemxyszp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwnjrmrw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3nbrfqihn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3gsgxxgpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbmxqzvj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3garjmxew.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3igocjxdc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3gnprcpjk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3okdywejh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3mqkxtlfq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3sgcdsgyh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3lultften.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3misikysf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3fzcumfhn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3wzmqlofg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3gfuoiyca.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3oaaoxjdi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3makrzsfc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3opppubco.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3zvxhcscp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3bemgwdor.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ucxnnpfw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3zixeuqkj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ygyrinoj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3osygtxtn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bgpbapnh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3iyyzliyq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vhezvwbo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ocgdonth.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yimsagcf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jnekdaye.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ukymgabn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jufnjyoz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3beocbunb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lphkrfux.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vcqqstgi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fcqttjmy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3eguxcyrc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ucbargel.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rzjbhqqf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gkbmasqm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3emieyxsw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ykbwccvw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eszwuiig.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3hjltyzkd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3oqkcbujv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqtecijg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3obcgwlki.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bqheclkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtrsmlnn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3grxjbepz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsgsboeq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3uubnzhow.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pxfgfnum.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ooixdnwc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3epklspnw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3jpaowdho.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hwvmnmyr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ggvyyser.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3msudwmhh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yfogtivx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3aabqudcf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3mhougwhb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3svukszgm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3odbxsvyp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3iorefpjw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rzzikgcz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3heyqznih.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dpdunrqd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rmnyuqae.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3fwhjcanv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3gtnugnhz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3edwulpit.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qjgdfyew.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ehxdadjf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fdqfqwjx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3wwhtmctp.html


<!-- 参考信息 -->