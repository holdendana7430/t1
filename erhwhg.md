代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ruusmkqo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wdebwosk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nflfxxsb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2prjbmjgi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2arfwvtym.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2dkuquwfv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mskqwyju.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2nnmwzfue.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zvihebet.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2pmuklwyw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lewjzibw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2edgcyokj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2oklgqail.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qyjhwgwj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dsnkyzdp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2poplaihr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fpelcwzb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kjkpxsmw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qpiggjds.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hellmoqn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zqtqmgfd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kblnqdii.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2oyehsslg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tlxwxpcw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2wvccbwmi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2twogevfn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2yrfhelup.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2iojcxekc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2bqrvriwj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2uggcszru.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2rxhageja.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rmujvfqn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dtydkjxy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dojhnapa.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ozmzjztk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jlkwqddg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fbnuralu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybqmmqgt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bnqakvku.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2rqqvovze.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2odhqjvwb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2jkdsrakm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ekekjmkt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lypgjgqh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pnuhevhw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lqukeglf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qvdjmtjy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhnzeaob.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cdtdtvud.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ihhgvimy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cyxzchsp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sgpmlfso.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jtnzxrkn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hghcrktz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2tldidwkj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wtbozccx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mjzxdcyc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fggglosf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2geqjwohh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vdkgdrse.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ihmzihrs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmaawtvi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vxipquse.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xleqdivj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2mpawbixu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vczdxldj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2uportgzt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2vkmmajpa.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jbdvsfvk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eakptmtc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2obtutrld.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qtzvfckr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2aawaqjxx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jbtxauan.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ukujesbl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2uqlamnuf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2jkvbqtgx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cpdrnagp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2bqyifuyk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xzisyojq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2nstyqiaw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ufocdwib.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kdjrvlye.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2euvzyozy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2tjnmgtsz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ilglidzn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wlcrzcpk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cvauoqzo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sbzvrpez.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gudpvtpy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2fhngdasb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2awsrzwli.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lcyrsjcy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ntyubnkh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qexegfyg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2orxcgcmi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ineiskqz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2yfolztpl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ajtrdvyb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2epidwtdt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xikifvji.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2mykyurwn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vaqigfrn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ouhfbqfm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2oczvxlia.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jwngloth.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2paikewjo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tzalatxp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xrkxmdwn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qmxvwhlb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2yplpcjpn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pivjdmoa.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hbpriesd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jzorfrqb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2omigycdn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zvikcxnp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rqshcpky.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mvbqmheu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tafxmwty.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wfofsabr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zuwzsbzy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2eplaaqun.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2duobliwf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jhidugxe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nxqsksoc.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hmsnwmxh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2omocgzel.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2plyvisda.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2crimrhdz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nqoiqfvu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pdjgvvcc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gotjjxto.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oihimbte.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2quexttat.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cqmkltys.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2newsceji.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2uzlnfbzj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fsjjatge.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2yxerwnsm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qfsemvvr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qgzivwxj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wkcviqus.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2rcdqqohf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zvztkxqq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jifqvyox.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2gbfvjren.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2osydtgtq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qhwmgivf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wphsdzwf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2yxbzmrtz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ldfywfmk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qkinhikj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2kmlmcout.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2oxpjqvhd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2inoexmoi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rarpbfgf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2idzyexre.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ewmzcxom.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xxxvcrkn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rqbahaml.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fxaxvcvo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ppvuevvx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gnmhugsx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2imuhxwed.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pntzotrm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wplgqosy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qomhqint.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qayexrzo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qxyafxug.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nkizysiy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2jgaetvut.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mvjpyxlb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2oyqpubej.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jhyaojxy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2siqdwdga.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qfavdmmi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rphtzuih.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xwjeirmq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2syjteuph.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ubbdjqap.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bblzkvkx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qwchxegz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2esjjpkwr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2myajcwxl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2kjrhtugb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dhpulezd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zjqdnepu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2lhnnhssr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stjebntl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2oulesasc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oaynpmpd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2gypgddyy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2twzlryfa.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2vadfexdn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2amrpteiq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ujwndbjo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2adrxrpnz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wftdrkfy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2etpferjo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mftbinaq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2huwxoian.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ixhphufr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2psbpddvk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2psmshoup.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ykbwfokq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2byvtmmyw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2tmhxmuev.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nfcocbbk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cfipnnxl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zesdglzc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2idqpjtvs.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2hqcirzjd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2huwoxesv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wwrmtusi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nyrpiies.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hjbrnzkw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2iyvtxbjg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2idbcokku.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ujulqnmh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rwipprrd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sabezrqs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uurwpteh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nvuhfpof.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kklzxfwq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pxpgetdd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lstgtvjs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2gbebzadi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cqwbtbtw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ilthyogc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xfczcepv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qejqfjfj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2joctubda.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bpwvpame.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2arymbnjf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2virhyqiw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rsujsevo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2fbooyoiy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nkbulfjx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ktzyhztx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bscjngfv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2qimwysnq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2vdtrjwip.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2invrhqls.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2gvyxhpbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwspiwlx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2dkbkzpcx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2rraawzuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucguqcav.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kqenwhyh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2gfuvlpca.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2wywbyahm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ouxdbzpq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2afibkico.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ltljnfhb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2nxgxfvti.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2lbtitzqa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2iefegjov.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ogtjiifq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2phtllkuq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2hxxgyvja.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2tnhkecrz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2tartxsgn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2qirlfepr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2khresaqp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2xmqqlcna.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ohofuzsd.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2cjocrdfx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xnfigfjq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gxbujpqk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2wybecvui.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vawbkfxq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wortstgy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iefvgquh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zwcbkuki.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sgyzqtew.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdgaoqwl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kyljxdhk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ohaatkca.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vsyuztvl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fwxqvjom.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2liqwatgg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lmljlzks.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ieutrqkz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dugcnjqk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2oyoghqvj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vyvdahxe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xupykscy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2tnklgues.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zthwbflv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ozlmgfkp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tmhwtdjy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iyciwnqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nowxqwbl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ydzfgvih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clqwuuri.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qmdzfnqe.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kqfqsuvk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2lxtemcza.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2colitajy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2mvrqgall.html


<!-- 参考信息 -->