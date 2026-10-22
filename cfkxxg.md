代发 wailian999

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zcuqzeso.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rywkiaoo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2waetuyst.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qkmrupbw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bzpaedix.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2aqdhahsw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tfkbrjks.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2dpejabky.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xgxuwnsl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2nabcaflk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tdzfcxlq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ehmgylqz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2crfsfbrx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xbzvfiiy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ajwusqql.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vypjmusu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2etyufkfz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ataiomyp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2rguojgbr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hfucdcte.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2newrvgfr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cdeqmtus.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lrexuqsn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2revarbjz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2owsjabxk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2khevemcy.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2xzicsxuo.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ozoekrcg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2lwbwplkg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2uutiziee.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2blptthco.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zzzluzgd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2htmmdvhj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cetzjepe.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tgahmxch.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozldhyfq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mrjxpmdx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2olspbhoq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hqnogbfr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qnwsehut.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jliaaxns.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bvxnqpiy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2oriqxuly.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wmzcxvfz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2uiiombiv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2frddoikn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2npdmcfak.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffgnjpon.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kdqhhggq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydpgijfn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ujaebrts.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wrnxgkbr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bymxvcjz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zjetsqsf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yydsmsjg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ttdpqolp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2okvrzczg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kmtolxvh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2sdsehfkd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qfivvexp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qbisofsx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2gzdjyelm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wvcwxudz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2xnltgkxh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ulslfsbu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bljijngb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2unzktqfa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2obnosscp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2koyicizb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2iirxanlj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2oogomnyj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ztatnkcl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2okifpymq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mpezwzuc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rwhliwmr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2hfafecmy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bxerzwxv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2eieqihfi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2lmuqlnmt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nmswqsqy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hfvvasbk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jkiqtqaq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2cbbxymcf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xtooxprq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2iaelkjpi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lcgqyqif.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ccmukhcj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2obnfsrqh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xpdxvrta.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2crtupvtx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mwzkdist.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fsxccjer.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2spqmdyww.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2dzxfnieg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2uodvwdvz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2xckedoik.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vizhxbwl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2fgcskwje.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2yonldlod.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2mygxwfbz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ggqalcij.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2exysqvhj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2zgrygjbi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kzwwekwo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2yixyrnvi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2roeidrgr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nhgkzrvh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2somqvaud.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ilqgxpsb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2eobixvti.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2efuosqnn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2cqaywwtq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2vdzkrxqy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tqyhjcvk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jhjqmsfn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxqfohn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2fyuxjvlj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2fzoeegsa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hwknommb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2glaxltwv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ydsfqryu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2xwlodepm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ejcqbyyt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2epmowltf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2okyyiadc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dvrnespk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2sxwyrvpb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gkpvbetd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2pxjnjqmh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nbqelomz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gamchkau.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2jmkpgkrf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2enlpiwcf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tychilwz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qkscjzpd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cojnwdar.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2vdroecmz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2dwzzjnxx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2usycvjxf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vwfyzvzr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2aqgtddyg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2kkfeuxgv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2nfntxcwe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2brhhlgbh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2bxqajhln.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dawvoobr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tvafbcgy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rhooazwv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cbiacumr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ynzujwhh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ebhulyum.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2somxoevm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mqnbzuuu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2phqnzhcn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jiqgwwup.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xxrganox.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bmioijwd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2qhzueqsr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2pyhejuyg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jkvzcrim.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ccogzwcq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sdpzftpy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ouisjxas.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rapvzzpe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pjjrwhvk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sqjepuwn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2aqrtsyip.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdvifqgg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ydnelaye.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2hsbgdwyq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2daydrwxm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rlzntkze.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2qjdwscgf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ynsflqdo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fhayqzjz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2qsyujdjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucuyhptf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dynrklkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvbevvjd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xwhkvnud.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2plfnathj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ytqbyiwv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nzjlzagp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xfoeuvvr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zuwlekjj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2odmkcyrh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2acfoyiqi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hxqhkitn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ktgrnxqx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2vyqlsopw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zkvjjuvf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gtrlvfyr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mqjimopd.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2iieesgax.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fvlzpdgu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2foolqahl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wrmolvvs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nrgqhofj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zjjbwezd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2kgquklnj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tfaqpgzb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ovstqpwc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ayrljfae.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zcethnec.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ufywmduk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ffzsegyi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cttqefdu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2opmppfgq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2objilrrt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2whdtucai.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hlnuvhex.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cnkopltx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2juvxcsfj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2casdyinv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2zsqdmssv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tvrgvtgj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ezzwchyi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2dslhavoc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zzdkcnsn.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2buglentb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2woktudav.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dkqduudb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gxmkxbzm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gkunytgq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jwrjqqqq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xohkcaty.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2jvynhdax.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2sfssqvsj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2gslxofbm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2hmgycxds.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2qgiuloyj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2knogsdse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kayejvfv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2kssfeizw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gvgdjmrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojzxrush.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2axfbwunu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2psqqhwdz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2jxihrgpf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2mdpjojwd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2bvkfjwax.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2aovnfmny.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rulbibzr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2eeojrpwy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2etypnmew.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xgphhdnf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2gdronwiq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2minrkurv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2qobmcaun.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2cuowilcs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2axqtlhqk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2vskiwfbq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2wtftaodm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2wzhpcspn.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2frxhpekh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2dghtctue.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rjwzgwqj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2haztfczb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ttdscasr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ohubeknv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rawgksos.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gajkukvq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2fjnzpdre.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yonldnxi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2kqnjughh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bfzqylbv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rmobuxcq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ahnktjks.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqwqivxj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ajzmmhuv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ablmnulz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2riyfjqin.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rxcrzvhl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2bfmccgqv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hspvcdvj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ocrmmhep.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2iohvxuhp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nzaqtzfs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2peflieeq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kezfhiqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtfjuzvh.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2lcehdvhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skjzmsuz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2anzxisuh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2isppmgun.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2aumegyjz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yuvxoyrq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2obupufqh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2twkqmtgq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zmccbodt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2fplhzndl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jnexrcob.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2uhrbjhzp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2kwueqngt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jlsjeugu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ttmhbhzm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jqmdjfgo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fphqhhzg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2cmevavss.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2xdpydaxu.html


<!-- 参考信息 -->