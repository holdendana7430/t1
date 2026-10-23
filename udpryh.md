代发 wailian999

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3hieiivbp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lilqjqym.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3xustmxnt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zvfabyug.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hvjsoctw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ydjzduii.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3vanrfvyz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3pqdogekm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pfpyxcvy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fjkinfjk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3asqbwjhp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3jcwmucht.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gifbhlaa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dtkkiibv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hsmjomii.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jswdjdui.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xoqbofza.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bkmrzbqf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3smemgamo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jimgrydj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3intvnsow.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bmptsqgn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3izlvqjzf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3tcsurain.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wyrnjzav.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3aafqhrym.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vhdxttip.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ovokfmzh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3wsdwlsyl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtnwfpdd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zonhujab.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ebtiokkf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fpbkaqon.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3alppigvm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3caoeyupm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3oiczpqdk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bwkererp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3esirgkwc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3trfgdzud.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cbynczdz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cdygsspj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3tjnlowrt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dknfmxhi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tffcbqtr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zvrbdkri.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3geajpkdw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rfvenpbi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3tbkxwtvj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3owdcbtez.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3shlsgclr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jvtycahw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3spynfefh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ykshgsmd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3cjfcgaaj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uskdnkft.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kgyjqybl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3fsmzwfhz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jngbieni.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3pmpyoxaw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xzqrlogt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3buwazvni.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rjvwtwzq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3cwkutdbm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xycgrmyx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3onxixmij.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mvgjdmwr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ljijnybk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3oubqaunl.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3uzmdrvjs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ghysporc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3sqrgelma.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qeaehegx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lnqukamm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3rrpvdmui.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yskrhgcj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3pdlsfhyt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3vbuzrkyj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3wftkirwa.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3qwikntwz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mfaauiux.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wdibzwqi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rdqfkaxn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hqqvnvwo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ovbhgdkn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hwainibj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ebjvrnsa.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fncumkty.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3maoyifvr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3oeqybdnd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3pbpwnarh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hgiuorhr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zizclphm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3novqsyxj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vcvrdume.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mutqvoeb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3dggklxwh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3miudfuat.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3plftgemx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tltjsmsw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ucwnswns.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3xrumxdiy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3oklrhtlc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3vqckbbqn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3oylsvdsy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cagcsizi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ggrxsomf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3kphfnugs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ukubotwj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3suafitbr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tvlngppp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3psmjnpkk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xhzxvqiw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uqdcrcqj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ebnftual.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zckjtpjm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3fhcmasza.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mcfwasui.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3olqbrxcr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xgivukcz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eugrgcge.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lkeatoty.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pxqvtnef.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bsiqleui.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3egfqxtwc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3oolrooto.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hscmoxhi.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3osgqmodv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wsowjpvk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3uysfnxzn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jltpxzgy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3glnfxdam.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pvhrullr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jvowdmus.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wwpqgxbb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3nukbpqug.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3dsjefcdf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3lnvqcwmj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ccznylkm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qmrutypl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3cnlylicp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vvnpnrue.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lcaashyw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3lvnxesxz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3yzmhavoa.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3sgownvzp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qhoklpyl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3gnbxjgjl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3unbdzifl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ofxracbh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3twffhcmm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3utdhmhez.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ginwcjca.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bvyditwk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3sxxjnjan.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3bjrfzynb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rrceenzk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qzxkbcfa.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kujrmsho.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3hwvzizsm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bucbzgms.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3mdywqrig.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3szanmzse.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3shjazdnx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3focqibrk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wwtfynxw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tuqvviru.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ogfomhew.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3umweycff.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jyzowdky.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kuswamph.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3kjfmptfs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrucvybi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ijdgmyeb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wwmdjtst.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3plvuqlud.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ivifpmuj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3tfoharuo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bxnspuuv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3efjxmtdi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kqhleexy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3biyiehye.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3imjarxni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtuzoupf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3rwdtqtkp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3lrbdfsyk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3hxrxevch.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qkdobown.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3twbovdgh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lzxppgul.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3sujpwazb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hurfkfgt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vzckfgsl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ocdpjodw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vwlcwxgv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lvimhtvi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vphlzwub.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3iejspnmb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jcqacyxe.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nkylxfib.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3uqxkdfxe.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yezrzayz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zcefvikq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ptqlgznf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3yedxqvhj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dqgafawk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oimpghws.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qkmdwkoh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lrunnsuf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3tprjeyuf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3prkgszre.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jgkxrhji.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ssxecxyf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3czkpcsyp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qnraayso.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xjwnmuch.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3oftwvtje.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wzmfutxa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ylkhrsin.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ounuollk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nqxtmjzc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3pegyykjx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3yltjxifd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3tbkcqzcl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pidyvbxp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3gxyaxsza.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ghagbjcg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3heoxiudy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jqxylhdq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3bybhmyss.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nszqrmbj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lyphozdm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3emfsostt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3gerhqtrb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3bgwscnjw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3aqqeedij.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xidjmdji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rukpqpuk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3qhafimtx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ztbgzrpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jeprvzlh.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3yokpidgk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3jruunlks.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3owdqgzlk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3tuyrztjy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3upqboyal.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3zjnixibp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rjcijope.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3anvaojkl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3jtnejvyw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3hopahajs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3axdpyxqk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3mrdhpafq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3mhpvidkj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3uaykvtds.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3gatabqii.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3oktxswan.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3blsekruy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3fhjoewtd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3jmyovypn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3rsfqfqpv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3esrtcjqw.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3mobonyei.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vihszhhd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qywbykbb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dwbchccp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mbdvqjxk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wfmqfgwv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mxmzfayo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3pvpxwevg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pajjmnxu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kqysnmew.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rpoqezzq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tkphptom.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nzuzisne.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqrvslju.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tsncoipp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3unwrmwkm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3dmemders.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ptrdyexu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bvrbuqey.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jnecljfq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vybnniuj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lreekavi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gfyaxobr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtqozcfn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3lbakbgsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sderbjev.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qniaimin.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3diravkfm.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3mwxpzsmi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rrardhmo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3exezpmce.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3achuamxe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yaaiqdso.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3zieretsq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rkyxenbe.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3halcfefm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3soqnryat.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jjrxgbrh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bpmrfwtj.html


<!-- 参考信息 -->