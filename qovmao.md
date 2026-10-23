代发 wailian999

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kcnbvupn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3gbvqsdja.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yfafoanu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kdshkfyw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xazacdkb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nuxyzluv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3uxyvowag.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3migvrhbe.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3byouhcro.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tflsyepf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cqnimbnd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3eplmjuqo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3gyeczzdm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3jdedwozu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rqjvbtnh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3azqdmpys.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3nnptbsuj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3igunmnmt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3kujefsfw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xzungupf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3vofwddmf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3iifflxnp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ttcbwcah.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ifeghnbp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ifrohaqf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3uduekkay.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nnqspgva.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3cfzyktfr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ursuhylb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3svedjbfa.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jlgwqbao.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3whvomoho.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3rsmzzjdc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3hxdhrxee.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vdoajbzb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzdxdcij.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3mlalhnsi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3okelvpvs.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ifbovvwv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3bifyvznc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jzbcmbmv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3psywlcmv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3deuomldw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fszxxkhx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3djplczmv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3movubzvx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3oyixcrta.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3aobdvftk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3auwtkvms.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xhybyrda.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3bvicwtua.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zjuooywx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iiqxlfuh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3agtmchpk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rllfhjbv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ikvmsfnk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3cnomjslh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rrpgkjje.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vuodwpac.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ztziukay.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3rpuchixe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lrgusgyv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ueemnwam.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vcpnskrg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ivmtaziv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3jiubowzd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3zaoduobu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3lhyriplx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3uujcffzz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tcpkrder.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mumpxkrq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iewrmtnk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ahzrfwfa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3arxmvtcf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3mlpcernm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3pvfukcvs.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3mbvmhldd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3cycnxhes.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ftojsuvm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3nervyhuz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3eusgxaoz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yyunzffm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cpecvpdh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3eplprxkj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ijphxqcs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kitirmkk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wyeepgwv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3yxkaykwx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ffxyufvr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3focilyzw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hccypobi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ygvuvpwk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3jyjchnzx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3gnnpxidf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3oygjgrih.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3yrdmjyfp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3eyqkzlpe.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3eelshlos.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3cpcfmcxh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ksepzsvt.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3cqmohrwb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3emiifjlt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3dgeczeyi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jopsedjq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3bvfefztx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ptiaqpud.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xkqxrpfj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dwffavcw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3eizzsgft.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zzjjvqug.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vfgreoij.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xpaxullh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3egdffsdj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3fdboqqfl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3kyaqqbvx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3trtdpwwh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wmklgtfs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vmdhskwo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ejapiqxn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lzdzlfvq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3plsxgrqj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3iqwphkwd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ngpmxbvt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yawevxgn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xmzibjfl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3cqviqhpn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3flfmtmrv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cvydrfnu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3cdplhknv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ukvmnpgy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3pjbzbabr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpnujuyb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xjivpcex.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vklivsri.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3slkkxezf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3prqieymx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jpjhlmbn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cycxrhae.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3poouwxnf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3kbqrrdsg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hllkrade.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ggbmyrgo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ktkqmhzo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3lugoswoa.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bvewovvx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3feslfvld.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3usytixeh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3axpikikx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ezopgetv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ckeuvjpy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gnxrftps.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3sshjbxqm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xjvegzwa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zivkcjsu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3wrmlqswv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3hakdvanf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wutuazve.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qptwhvby.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3svmpiglm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3teydrgxw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ktcxisqp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uwsqzdyr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3eridffhd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3etxweaqt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3runikxyl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jsahwkrn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3zpwuxyia.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3trdvpgpe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mebwzlxh.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pvpqyvtm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fuifvhjg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xeparjhb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yahpjutm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xwcykvvt.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3kzhebruv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3nobhgrxi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3szxxcsen.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ukiyemaz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bhsqnfrt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ppkrzydv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iknjfixc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3rvtroxrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3srreisbj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ukuuiddh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3yyfxafzl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qhlfvytu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3zeittgvm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fkallcad.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nyimpcbc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lbsrysjg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3scbtltvu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cxlfxbax.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3djhmxllf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3xrngtzau.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ucyhropw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vkwyycme.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3znopzcoz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3lcxquoyd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nizjiarh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qmeucalz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ahelsiyr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ylriropm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3odjahhdv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3bzsffbft.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3eejpcizt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wqydggiz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nlxlgvis.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ahgnzimz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vxxxbzmo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3sjuzgdhm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ufdvnmxo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bsgkcdsp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hatyiofk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3swqbhdpe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bnqbdtxo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hoamurwo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3phvtnxtz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dsnqyzls.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3rsnbviml.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fkdgchxl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xkvmhoym.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3vaknluuz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3revfopgg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tclhkkdt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3cgfokdnk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ydgmbvzd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3nnyhstvb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mewquskx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3sgbqyykb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lpzlymmy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ycjyzlnk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wpulsorr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3fkjsuxjc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3myvxxaym.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3mvebsdmk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ocjkfqgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixvqeyae.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3yjujvscj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ryxylhyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hymracez.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3wenkihbv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3zbgluaxr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ushjeilz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3fauybikb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3nbzuqpzp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3hhkrjpsh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ovhouend.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3wsvkbfzd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vgxmfbgj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cmibwyqt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3aqchzmth.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3viezqgxk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vzoaanbi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ctkzjnsc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3kuzqedij.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qkrzznkh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3gppgqdpc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3cvyddlkk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3bahcnbwj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ngeggvyg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xkqufdjq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3qydzidde.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3spreekty.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ruzszkla.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lasscymr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yfipcyht.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3awkowcmp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fucqvbmw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lhoqcyti.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skhhkovs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ncjxivlv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fymsfrcp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qujywxvp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3extcfmsf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vbroeutv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jajjcvez.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lunnmtfv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3nkzpuver.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3edztwhgh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3rbezdgqd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qtsdmdwe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3poxikpqj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3owcwojfc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tmtlonxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sukovejl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpiupezh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yncnwvcb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3pubfydmi.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3aaitresi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3nfnkwhcv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tnbqbdno.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3byqdzkdg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zbfjcxqm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3haozjrps.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3kpkczhvs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3glmetvps.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3euulcfhq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3howvvvps.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gkfzsyhf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3olxfuzom.html


<!-- 参考信息 -->