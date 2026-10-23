代发 wailian999

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3dvtmwzwp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3sccohnye.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nzptztve.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3qnxxoaff.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wgoxwgpc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3nghanolo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mmgkfikq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qfzjukqc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yqqnujms.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qhhyafsm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bfrniduz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wjkkamdp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xhwxztmm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3uzcyhpre.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3wsafeows.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kpohmfwp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dzclltcj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rgnalzmw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ubuefxey.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3mclsnadw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3pvudmomv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hasowxzd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qczchjph.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3hczkitxl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kxephujz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3aiuxiibe.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gzsekokc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3srvtrbbh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3xhdzzyfv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3khmcslgm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xalrpcjr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqiafjnu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tcysvlzy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3iqcolnwp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sdexogzc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lzpnnbif.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3uoojdsls.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3enkyuqic.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3aesszeeu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3addipvmo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xjejarus.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3penfmyiq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fmqyafqr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3obqinzos.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ztbklpal.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dundkdsg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3auuetspu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vncuoltw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3vmzcbugr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vjegbjhs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hysuunas.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ngedvpvc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vpnkqlus.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rdluufhu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nbnkjihj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3lhaconjg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qlgcuoqz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3pgstsqaa.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ikmtvnoa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3rbujpxni.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xdpjxhom.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3osmiphld.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tghyddkf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3llgzeivk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kyfoaijb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3oamepqsa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ptlnfuqk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hdjxxbiq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3kdechzgj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ctglcvbz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vfthmzuz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gpjqaury.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dyexxdnp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nzbeumtr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3bxwtfbok.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3vkdwdiuy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ahswfsne.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3cjxnqyar.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lnjkvuqf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3welqydnh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3sjcbxnvj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rougnnpe.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3toglrghn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3owmtdoub.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3booddhse.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tjhrfmuq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mdruhtkp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ktnmwfwu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3vckcvini.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wiqwsonx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qnksmsuf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qfsqrqro.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3pbfsicnh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3adtwmpsk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3vgsxamxt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3arhhurzh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3aivettya.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cxfbyner.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3takllmzy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3wxqtlzki.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3etymzdsp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xdonqgmn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hbjgtlon.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3joibgazx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3apvkphqw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wmbxzlak.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qztduupt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3nutvsufp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wwmqyzyx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pyeycocw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lsfnaubt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3spfxfzqq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jbadkpbr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zkrwvixg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3fbxdlnco.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zsfbgylc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uzzyownl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vntxbrid.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3tbhkvojw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kmmnewrm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3utbopizs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zhytwpex.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3euypxnnb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3projqtld.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3fcpdregx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hbftybdw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ehapsedx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3olcontoh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wqsxhfiq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3qehbwcud.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3zhmouono.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wvrybjbp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3kpfmlggk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3fktkcfdq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ymovwyfh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hnjzessk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3kibijvvq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3czutgmdq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ihrqxwoc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jrsnejet.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ddaldjtc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wjwwnnzg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3echmeezx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3myjsdtbv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3axnytlru.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bxnijfnr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pwzlevtu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3srwxjzit.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wofuksnd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kuqiviyp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hqahfeds.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3cngnluci.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jhacwtvb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fvtolqrn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3bycjlvdl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ylhnhqie.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3hkjdllho.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vzhonlin.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3fqrezimz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kmllfyeu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kdgeakpk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3siawebtd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3lovxwvba.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjnfkkmq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dvnvkgpb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3zzvktriq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zzyfvdab.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3gnixeayt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3zuvhrhik.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3danjdnuj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3cmwahvxh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3cckuzpwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oosgjdbx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ewetxbzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjcnipuv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3suwnkqdk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cwdodxbv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vreulbui.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3evmxlopw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mtyzwdsp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gsyibnru.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pnylegzs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ioekbtce.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3oyujvhdg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3pwrdbibt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3oubwjhfv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3dfqtzlxe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3lrdzqydl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3krbrkwhj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3njvljwzy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3grfbeaiy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qegwvcnl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3phbfpnrh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fxsquwsb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ifjtabos.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3thrgsqbf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kyqxlnsu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xdpvksgv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bufodsny.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ctlpsbij.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3braonxze.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tjtrtham.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pbwcvzyy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nalbojja.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kpgrfkvx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uhgjfevy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yfpxabuf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lpffxnmu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sigodbyc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tdpuyycg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3onabbdwb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3decluanp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3zsphwisv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3zranwlwx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ekooqpqh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3xaekxpdh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3izalsnws.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uaqbhokp.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3jzkqhwzs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qxywckzq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ntokdemx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lkqqvscl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3frwrapok.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3zitskstj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3eqathdhy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3bedfxhkh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3xfetoeuu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xqduekwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utvtubwy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3sikcjjsc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3vzqbugey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juvuncbn.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3nnmyzygo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3spvrhmeb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ukqpcjey.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3lecnrqay.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3qaiacazr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3lilnwbeu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3fibssypd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3wukhvreh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3fxtlwrar.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3pmioilrg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ehainnqh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3kvdseewa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3icwaqion.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3owqgczcu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3jeqywsqr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3uyepvsua.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3igoaxldg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jodljpem.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3cqlfzxpd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3gvnpjuht.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jkxyryfd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3qxbebcxh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hmliggpj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fdyqgbkd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqwjnfty.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nmgxmzip.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kmadfjks.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3bpdzuahb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jyufzldm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gddghbjn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3klkddvio.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ptjqvnrz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sslrqlaj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gqdathvr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zljljpen.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mkdairee.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wtdsvcmy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dobxitlm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3srtkeqpq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3rcwqiflk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ssjuyvay.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lvvtcccy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ymrwpdta.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bnvhehzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjxcaogx.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qyknhdir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lofrerjf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3hqrihdhr.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3sdwikcws.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3nzvfdffl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fgqjdhsv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3oqdhbzoq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vyfrkkvs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3wilfspdm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3wijsyywk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hosbzlmw.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3kadxrrig.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3mlruspso.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qvztfmny.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tyqlpkry.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3rguagwwb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tagcgsym.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3tciurapg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ekboiepf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lovamfgy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3asjqbnxo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3cyzxvhlu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3etppusly.html


<!-- 参考信息 -->