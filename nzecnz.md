代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ndjfgrak.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2zlojwnpm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cyhmejwu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vgbpyxrt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2igyfwwey.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ezwymbuv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zufvpxvr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2cdtkzzks.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2xzesffbx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2bshleyea.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2bqmnfryw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2brkuxkiu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ensimvph.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nanomjhm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wwhxyuus.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pqzsdyfx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xsctcfhx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2hkzbgtni.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yztrfnzb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2oygyvoir.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jyxstuji.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nbttnxay.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ckojykkr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ebwiuuof.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2drurlbbt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2lgezyxgc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ptempyjp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pxvxtmob.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2mecvfque.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hykroiow.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2pbqqkuux.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fdsbwrdd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mfctcmtz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2umnlneey.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ztpssdds.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2blfwhcqa.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fapibpiz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfowukqv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zurjbypb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jsrfhjmi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2axgadeht.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2dphmnruz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fxinzohh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlgkjwai.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2uaawzsae.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cxjoickc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cktoeail.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqwetdzn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jwarttwo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nixudycm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rvbvbsgf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jdxwpijm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2nvcwtvqc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2enzuzzji.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gguymzcm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2liajytko.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bxksifes.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zoojgljx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2odtndlao.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qxmsilvo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zugzdsut.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2exrhykif.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2hfilxoyg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2isotaxxo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bmfnxnyw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fjmslcrs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ctowwian.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ooggxnzk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2jmewbnoo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pvngpjhe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nfxljtbr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2joxpoiwa.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tnqmmqrj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dvuvzylw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qjzmfhba.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tvvgdfyw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2dbvptfcn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jrjmwval.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ginejxdq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2gxwaqecc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2aawqrars.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2peljlnit.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2mmoqlzyf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2nqkanryh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2urexfwhp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2pxsqywft.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2arufkcig.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2obajpjig.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dxgqcszz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2bxadgjtp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kubxplmq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xadddwab.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lgteihxe.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2wkkarhky.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2djlamgos.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2gqpmkvhx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2szqyoabv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2akerahnn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2imvohgum.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2anfolynv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2yimeptgd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nekdcfqm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bcuqrdao.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xewewfiu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2founcafs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2joixdhtt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2dvzfszrw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2mlpcrnzw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pfkbxsmx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2idbsrkcr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wtmkhzvn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2djebfeqh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2mxhougae.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2krbqtfkl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2cpjnwnjk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2aazvbliv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2qnmndgvs.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2fovikyix.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2melouxmc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zrlqcovd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jfjtthrv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2sgtezajh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2avpxekqa.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2maaswjcd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mkxtsbau.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kgifrzbo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2sucumcjl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iwtwgtqb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2mjjdnilb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ueeiiyij.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2lbsidnsu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cpezbslq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2orbqrymn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kpwjgujf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dortodcx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xqunroht.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2winrohnx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2wyerjdcs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zqbjipmv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qdybekyx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lcwtpxsr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gcitdakc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ofxezmft.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2oyoszovh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2mjwziijn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ebmkoxoy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kdqpwibu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2nidvntcf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pdynxuwx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2inkjkzhx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jplvbpeb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zqfbtfiv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2fslibrvc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2notcjwor.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ihtkkdru.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sihyqwhw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2iyxqengq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2sfrcbryr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yxheatni.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2cxihinps.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rzafmdpm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ybdbphho.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2uvslkxti.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2khldicjg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2petfjqvo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ephlodcn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2uhxoewdq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hlblfsls.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zzoampkk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ktxocxhv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nhvqhuhb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yrijxgfl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2verkiqvf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cdxtarbn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2mdcafetz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vyhntlhm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2efdiclff.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jalxftxn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jrishkqv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2uyqygrhg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zkumwdiq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wkcnrukp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2cwfzyyie.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2dexobfuo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2votcenrk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kzmvhhfz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2kexzrssc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2upbffrmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivtjodel.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2mkxjewzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgzzdnuf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fpnxdyye.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lmvblvxi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2eacsdyij.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2oswrvbxd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fakycwcw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gywvqhbj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yisbrgme.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qswrljsz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2chjaphtz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2plxgdbmm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dqymebxv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2kqwfmdzu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2thxytjfd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wrhextmf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2obedkixz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rairofpa.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xfqziybe.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2zsjgnciw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2niyzxepk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wdmihodo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2rulbohxg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vmyqnzjp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ntlqlwdr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vumiicwz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xyqecxeh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2lcycwblp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2azeiidnj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lxorcelg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2pvqzljfy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rtydxhuj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kmfkyzyx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cwbpsoui.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dsbtuetx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sjjdbtcq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tlcqgawq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2xbgviafk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zjjsxjdv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2nmyipuzc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2inauzywd.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yuwlovtw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2laumebhl.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wxyhcfod.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ycvwyqkf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2oguhecng.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2auuetvyh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2zjdseesq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dmfvrizj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2nlhacfag.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2fnsyzolt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ytmhxvrl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2uuendcwh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2xmgpisgh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2wpqkxgff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2picjssnt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2lgmeglpq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2nczrzfgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azfsrwyk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2cmrkszya.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gxsnwqzv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2uggapngu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2xswchjvg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ejpjpdkr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2gbupiupk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2vtxhykbf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2wjtpuwqu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2nscwvuvt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2nwkhkxyc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2phjbqoqz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2emllsksx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2foqvmivz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2levqcdwu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2jwhrlfoj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ydzauvay.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ulcbwkrf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ppbmyzml.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2aoeoyynl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2srqnwlmc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cklopehn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xhoprjks.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hcaawydy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dqxmmhha.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hwfjhfow.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nknbiadz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2stwwgvvf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fcymgsby.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2niccryhf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rrocxgqa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ruopcvhx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tekltndz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2erwneiqi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wouoqaiw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rfikilox.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tmtqzgyb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gbykkiyb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2dcabapmu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gdewzaqe.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lboeqile.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pkonwevf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wigbbckg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kfvzonvm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zzbiowbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjotlamu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2jidyjfmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btbzoycy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mnakezsm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vtnqbppr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ihhdfhvm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2svtkxmbf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2bcjzqdir.html


<!-- 参考信息 -->