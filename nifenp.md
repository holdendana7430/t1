代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3gvfzbzbi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wuhcktgz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kdenrptj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3epomkjwb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sdvcvnht.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3jheuvqra.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3razukbfd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ohlcgzus.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vftnrjzu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3iiltexcc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tiryujvx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3auiqxdie.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lkpcufte.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3qhzlukct.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3glkycupy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3floclzsq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rqumowjd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zlomgnig.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ctrgrzfo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wvyoxrke.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qnlgeppz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3znhnnmdw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3akcaksrp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lttktcye.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kaqbauhh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3fzurgjng.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fhtxsqfj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsjieubn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3mnmcaoew.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rsovmsto.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jlmabrzf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxqpqfgg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fakxmtqt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hofqrukk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pznslitp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3npmikmdk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ifctkauw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3plkcmyxl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fzxidmzn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mkljxnfa.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3adsvpbjy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wvuaqziw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mupbflwx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nzwtoool.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xxlpfwnn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3mskjyefm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3eqyunupy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vjizzqaw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3aczvkkoz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gosgfgby.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3nhopagen.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3yimddzye.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3doznwcfl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ylkabelx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ccbnygui.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3lwcmclha.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yfjkngpy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mnfcqsuj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ikltznwe.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3rilycfuu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bmwgjrwx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ptrtxogw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3pdlqvtww.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3eevgefzp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3aokgvyqs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yljdoubk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nkydpsiq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3inyxckcm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rjmzbhzu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tceocwjq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3eskpoyab.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3relnvdpe.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dzsxnmjo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jyiatdtf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jsaqcvcr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pcklahux.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3hlaifvuq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3aqrchivc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pufurcfv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3hrrlllnd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3swktmnig.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ujrfmylh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3xxsnajji.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jnkmezre.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gwwqjwtq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3cnxbbtcc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3iefsvbui.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3izguwlid.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lhrymdfb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nojwfipf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3snqeteoj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cvfudccw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bquxdsaw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vlifmljr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3mnmuqaao.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mgqchehh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3uyfgwhyo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gyeumgiq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3cgbyxfbb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vbveicin.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3iwrsdice.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tnykezpn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3twovrtqx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3krwydsfr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3nofybwgq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qmpydeyc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3hosbytmv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3aahtpvsd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3tepmgzqa.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3huvqhgnl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vxztoxhx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmsftgf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qconglzd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ambsfikn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3shcvyboj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fshenyfh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qcbcyioy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3clkudbwk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wwkfibqx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cmawigdq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pbbcmydr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3oejkrphp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bymuxmoc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sisckjpw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3tfxiimqy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qdblnoev.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zbctnwqi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hfwncfsd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yfbnxmss.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nhapinnv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3hkhdednc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3uurseswd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zskilcpc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ixmusjkk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3yryllvwy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vdzzybom.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ysekjzgy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3erddmfxc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ptqnplyy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yqhndlby.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3puqkfuuc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3asnrgnem.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3frmiatal.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3extbogql.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vgqxvmze.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wmyvctzf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ldsfbrpn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qtvtkbll.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mzegykag.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3aybxijvu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3geipfzzr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3jrxqyisv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dqvzecng.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3kcxutmcg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ebqzpycu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ikwlckum.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3aeofqsli.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qwqgmrgz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3vhttihpk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uweflxeq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pekmkfok.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3emyamlgt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ltnfngbb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hfwwbeuk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3usskhebp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3lnpxbquf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qmpkkmmf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hayrmnjo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3fbpixinf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3yxmpjcoa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3mccjpjnk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3uuqylakx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zibnsrst.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3hxrajmml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpccfoxm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ykmckmdf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wtehqsag.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gyljogti.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3vxvsspjy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3idljrnmy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ycjxjchw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jgmxrmof.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mivibhrz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pfzjyark.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3cstaigiq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3eiyvzfmm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3plnjrocb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ucovzham.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3msdkvfrh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gdbpfkxl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wmscxkmy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3trhwezrf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3oemfbaar.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vzreejjp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3rhbozxvt.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zbvkjtdd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ezdzywgi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vucrbscy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3rawmsain.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3nmmcrbzm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xclhdvyi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3miygazbv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bljqucjp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3weueiofi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ttvqkwdc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3izfceeyq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yqtuwedd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3omgxrqaz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qbcjeopi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kctuajxd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3cqedqouu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tfibvvgf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jzzuwgia.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3jztfiziq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hhjwhzmz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3nbxarybr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3pjgrfbum.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jnhanuvn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3blrkcgwh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kejdzwia.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ledmiibn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mewtkswv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3padppewz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3uoovwgsh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3fntqdjen.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3erqwgppo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3nafkxoar.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3zcqctzjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnazczdc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3mgehlyze.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3hynpggvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzmrmtyr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ubbmafmh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3cxfruqsm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3sspwwbsa.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rfcnjzjx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3tdwmtwjn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3vcyghjnv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3jbttjzlb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3atydjgqe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3lbeujtvs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3pdxujswn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3owsdzeyu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3tieemvpm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ytddfiho.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3kgjkdymk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3fsmfjujf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3qqmnkfsb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3hhflivqg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3rixqpvls.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3qjxykllx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3bqnpyfhu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hezlshvx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3wlbqubmu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iopergxr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3frznfkdq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ljlskaiv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jqjmmmea.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzlhubzc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ykwdcdqz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3echvskum.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qcsoxdil.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3slpzweyy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qzzehjki.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cjnzgevg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pgwvslyo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gvwjbccd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zmzujtdt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3etjbnhhi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3flfwbtcr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ixwkhxtw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3drehphlp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nrzjozrn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vohexlhb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ptxiaprh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mxhthrci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akaeyjmy.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3nmukcgmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjmmprrm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3thplgwft.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xnlfqpag.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3jzuaiett.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ttbhxszg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3fvmcyugw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3acszhrlh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ncfbxbdv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3kxskbeqm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qvgmegfy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3gqeisnyk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3zasczhmd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3iuszzbxm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gbhkniml.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3fkatilvm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3etbmywwb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3veazreaw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3rrexzcgl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3sikhdlhq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3utktkdif.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3gvslrexy.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fwuohiwf.html


<!-- 参考信息 -->