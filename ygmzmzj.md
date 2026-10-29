代发 wailian999

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gfktqagqe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gtwvmnzlr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gksykdmbv.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gqfilrweu.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/glopmknlg.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/ggxbtwypg.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gtbheoonr.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gmvcgssqp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gidwdfvps.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gzbkvliba.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gslkkpvje.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gzmpcxolq.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gzaxfzoio.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gpumpwafx.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gkxoadyvc.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gywlepcxy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gysrchsip.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/grbdprtil.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gekeuuobc.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gdulpqgdu.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gxxubthxo.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gazdbxkyl.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gnlkpqphx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gthbrkubi.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gclqsvbao.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gwulzyrva.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gynvszxpu.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/grhllnmwu.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gfcutyadw.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gzykyspyh.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gftovekjp.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gawrytihy.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gdacrbipj.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gihkijkhy.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/ghpyirezi.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/goibkqanu.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gagakbcfd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/guuuffmtj.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gjiosdtmd.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gtsrbcmsd.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gylrvbkix.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gbzjlxfls.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gpgqiailm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gaersoenu.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gskicitlp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gitswmlca.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/glpykcqwx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gpizocthv.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gdkrasqvf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gdctxrzze.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gqhurrqbi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gotpryybv.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gucfiuabc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gkoitzrtb.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/ghzzriadn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/ghhwujnrf.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gdqvtqrms.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gfzgjfyzk.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gpepgolxr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/guylweabo.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gqiglkjvc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gzlenkpxg.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/goknqnmqu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gsxsnmzzk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gqchskqjc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gqwafyehp.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gcuvwuwjn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/geqxpolyf.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gmxxmnlvs.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gwlcyfozl.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/golmzjuov.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gqqvfutkz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gjoethtnl.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gclmdtdqs.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gpehbngcr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/guiuksrzk.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gaoqpuyar.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gsatftchl.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gdraxborz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gjuapcxwo.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gkvvbhhxr.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/ggqmzzrcf.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gdkxyskpn.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gtniqpltn.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gwuhzghpk.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gywjoibvx.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gncfiluwu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gwayvaxek.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/goosgymih.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gusubhalb.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gqpvvaijb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gxmqxrktm.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gmcspjwki.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gvotcaybw.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gymkqhlqz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gksyyncju.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/grgxqvvyp.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gwwqianfv.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gysevacvp.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gricqaamx.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gvclhltss.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gnymtczjf.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gjkeahyze.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gnfzcivqp.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gpahwawee.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gmezdypsr.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/ghgudkgpg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gjobaldks.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gblqzdzlh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gjnwbfwvo.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gkxuttfdh.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gzcpuhlzm.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/grfwtvtfk.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gerlfqzao.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gebezkvxe.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gvozfdlmx.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gvpvbhhpt.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gjskclgno.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gcdctfngp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gybpplrbp.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/ggndwbuus.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gakilvsnj.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gfnzlxdcn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gbmtbiauq.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gdbdjnzai.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gzeigdfmm.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/guibbvvnm.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gkvnzibpd.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gwtzthywy.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gphxbiyru.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gpcobrtnz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gozsrjptq.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gqlojfseg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/ghzqmmgdq.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/geslaaiqq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gegxmtlcq.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gmkyxlbei.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gsoyxplyz.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gowfiusiy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gycnqwvwd.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gbvacbaze.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gfgbxbdvx.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gmpmzdoke.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gxjvlamks.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gftatqjvn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gvfqdocaa.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gziwigxjr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gkxcadtvt.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gdkfskbsc.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gomcjdylj.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gjkqsmthk.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gtllhqvzf.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gryszqfys.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/grmscsckl.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/glytawnjg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/grvnwcdzn.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gyebzpzon.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gxwpbdujb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gkudesiuj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gexiygghl.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gwvvhzipf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gnydlqraa.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gyflbbspl.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gqoqnntqh.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gycrnqwlj.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/ghnugkere.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gpfsqvelb.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gaybuxwut.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glatwbgpc.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gldzluubf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkjuwhuai.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gzizusnrv.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gbeeisjqp.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gskkuzejh.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/ggzwkvysn.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gtuvtxgkl.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gycblfeku.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gviaqzspx.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gkxqyqnjl.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gxucqnmee.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gyxqcxobk.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gkdiqofkg.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gjomxwyuf.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/givuffaft.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/glqsurauf.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gesalawaw.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gehevrfaf.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/ggnsgmvwo.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gytydvwpu.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gmlogkjze.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gcihetqoe.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gmtatpseb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gpztvkrpk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gfkisvdnx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gmkbihfaq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gafgjsfiq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/ghxcioymo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gdimgjbrb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ghblnecpj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gtjnbexhy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gibiktrzg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gqfjnkygo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gxqqtdbdl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ggwlelxyw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gwtrvcboh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gcalumeow.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gelgkcltt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbndsbzws.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gyvlfjblw.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gdtecznxa.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/glqxhidqt.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/glegurlrl.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/ggygimpdv.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvuyakinz.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gacccvpps.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gvnjfmdfk.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gfhcrcrhe.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gxgtvjhho.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gsnubhmon.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gserzfetq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gsshtoilp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gblmljhcr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/goftvkmmv.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gynmonqey.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvfownule.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gbdvoaqkf.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gvywskcjq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwnqogzce.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/glruubyah.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gjjkiagcq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gabzrdshb.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/giomlpyas.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gctkycabo.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gwkfjubsy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gmwazwfxm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gezwikdub.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gzncqlnrj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gzhwfxjfh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/ghuwtszwq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gyqicgbyy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gmkumnplf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gsvbbjtxt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gclmdoabv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gyzoxqznu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/giyxzfiqf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/goilcwwnh.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gpljttgob.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gismhigtn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gurmhjnyc.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gqbsilrvz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gpkmuxbod.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gijqhcpfy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gruocibky.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gawjcgtth.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gdwqjkqid.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gnndnwuag.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gwpfpgrpd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gwuoutcjm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/grknrurhp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gaablzkuo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gictszpdb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/goqyupywt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gvwlsotxx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gkjmzrezl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gcsjeisfc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gyjxjpgnu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gbklkaicp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gpbajdlkm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gygztyimt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gkhchuzat.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gaofzismi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gorcxqylp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtkgbgzgc.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gqvxcmapo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gddchspkt.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gevrepygj.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gjyjezydx.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gwijceuym.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gymoqeusu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gaclvcftb.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gvgqsrsen.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gfricizkf.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gxpluumkq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gofonhtox.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gjyivhemn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gajeokaew.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gwmnyuzhi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gngusfsvc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gzvkdhssu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gkadpvujs.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gdbqerjye.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gquuyrkjg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gytcrsyfp.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gpcxaqqai.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gxfcrspmm.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gigmlvpik.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjdcriujg.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggsbsmsyp.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gdobbrksn.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gwxtufjgd.sHtML


<!-- 参考信息 -->