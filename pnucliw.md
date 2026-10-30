代发 wailian999

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gfhetlhxc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gjfxkrvlz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/ghjudbqxe.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gwylsasti.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gsmayjpdv.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gqwqiperj.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gfcjltlgv.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnajijxf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gstuirioy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gsxuwalof.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gebhiecdq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gyaylvtce.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gepqqkbbg.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gnqcronbd.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gwsedcspj.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gwdgzvgzk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/glgpyvsbj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gcbpbgfdm.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gttkaxfuf.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gwrfznaku.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gzzaprixw.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gxkidkkts.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/guipnuqrg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghhvadymw.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gapndptyi.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gqutvzcre.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gxzkdobtx.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghtttwbhk.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gxqxehtvx.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gvnyohunc.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gjgqnjvwn.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gwgaueqll.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gjilifnlu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gbpyaoqfg.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/glwocptdl.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gopoznpvv.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gqzgvpwby.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gyealuqqu.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/genutkdqi.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gcbfyjmff.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gsrjxoatf.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gyrnqjots.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gnzzaaaid.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/grxamqzvs.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gkbbgcdsv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gauhlmnpl.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gsgecyris.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gsfwuoftw.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gsmpkeutr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/ggnydgseg.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gqeoivrje.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gxxuqjalu.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gbzneqyny.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gdszzvnxs.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gnqparuti.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/glpebmneu.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gttgyvpmu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gakexwlqo.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/grphcmjuj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gqwplvdmk.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gkwmrhwzv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gqufnqzoz.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gnqnegjqi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/ginywbmql.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/grncrbojz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/giiqqxpua.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gkqdjglng.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gbjuqyfon.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/ghwqrhhfc.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gfubdzoue.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gbecelxaa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gmrzpakok.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gubucorep.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/garvtcaoh.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/ghvdrqund.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gdbknecrx.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gsqvyegcb.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/glmyjohnl.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gfngwlfcb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gawgedbrh.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gukvqoepi.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/ggcqmnkho.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gagbabmcr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gwdzfiyae.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gkwzcoxsw.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gyskausuh.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gpohsbllo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gttynbafv.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/geoxudgkn.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gaupydxhi.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gkkkstdjm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gmohpoutl.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gnncvkpyh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gzexmskoa.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gqbtwxtcx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/grftgtoco.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gqrnouihw.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gxhxmtugs.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gwdimqxgy.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gnpgxywhx.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gwuijqzpj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gguuvwvwv.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gvqbmjzaw.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gkohxgwnk.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gxemfqium.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gcgfzimdk.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gozfftdtb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gqzypimju.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gyddcgoef.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gqlwwuayj.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/garvtowdv.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gjtzkzdoh.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gmtpgjzbf.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gbdflteny.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/goeuyhxja.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/ghsvnpdoc.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gzklvizjl.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/glvllicqp.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gxpmrnrka.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gucxfnalw.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gagpnbchd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gvgjjcoln.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gwxyknynu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/ghzlsichy.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gsmzuhcju.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gtbbtnfjp.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gmfujtuae.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gyffgmweq.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gscvrecga.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/glxpepinv.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gwtwoqzhn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gfgqltjqi.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gpchklxpj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/ghlgykyea.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gluqumhfv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gyntfsthy.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/govwzxfzx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gqnouufjz.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/ghzpucjel.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gtkkgrexl.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gaoieyaqr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gheyexevy.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/ggqnwbnks.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gqgjvbutb.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gpjrvmsgv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/goekedvlv.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gabnqlsis.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/grvqixvkn.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gluveenso.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/geccbesrt.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gchjdzoav.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gmgbpntjv.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gnkvvhrcq.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gyriytppa.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/glgrsxbtf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gpfiganmp.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/germkwnts.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gzqgkwumq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gvshxtmzh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gdsxvmtuh.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gsrelssev.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gkrcbcdpe.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gdqldtyzl.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gimogqmri.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gmybonkts.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gnvdrrjqv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gmgkmvxzc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/golzdhqix.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqflfyjwa.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gcpngxbro.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gujsllbsh.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gcjjswztf.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gesfgyzyl.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/ggejpmtei.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gdfbljjes.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gvfgzkrjw.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gqonblchv.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gatyujrvw.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gtzbfqrkk.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/ganxqaaia.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/geiylyavi.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gtrjnftvf.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gubzdidtp.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gsakchdwl.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gesslopql.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gunxyqmtv.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gsrhfmmai.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gzunqbofu.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gvvzzxmjn.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/ggveughmq.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/grmgsvasg.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gjtwpthkd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/geexfsxzy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/guwmdduoi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gckoudfxw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gkkhaoopa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gjctmhiqm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/ghlkbfnki.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/giegcpuig.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gfjotrdym.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gkzaylzjm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gyfplvxuh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gbfoipdob.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gwnqomnff.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gijdyjbld.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gsmhooxbn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gjcfnopgu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gbmdmgpdo.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gcitwybwy.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gruetqjti.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gqbqxdcey.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gaoocysqf.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gokddobyn.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gfwmlqdkh.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gpuyzfmgj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gzhvfkqoy.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gwggwgyqb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/ggxqhapsc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gfsrmjvlk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gryujiclt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gexvzoctj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gvvcgkerm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/godlqufux.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/guxhhlkvi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnerhwqpq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gkuyxncxa.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gaiejkohl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdtugqgop.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gxzjidxij.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gwmqaurjp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gmpvebhlm.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gxnfrzzvu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/ghjrasejy.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gqslqvfie.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gpuzougny.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gzhziaixe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gvqgxqufi.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gnlmpoltt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/garymyhhn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gssauusix.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gwbkksadb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gsvtmxwja.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gswecbqlx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gfkycmsnr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gyalyejzw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/geeknfqfk.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gpbcmbknx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gkbqeqocu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gkmphrark.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gpggytexu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ggndidfdo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdnweneim.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gljorvibb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gcwjjbuij.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gstuqosrk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmmbgmfvb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gcizwsgkx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gvzcwkgnl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gduassdul.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/glitmyiyy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gislyzeti.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gopwvoksb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gubfempna.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/ghtmkemvx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gtbajqdpn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/glreqwowx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gitiulcvc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gcqreunvi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gzzhudwhq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpeetpdfq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gojcrlgoa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gtntcjlnj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnkidtjdx.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/ggeoapbyw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gawnlxizc.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnbtlvbyu.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gkzmcjfqu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gbuhkgplk.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gooxorxfw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/ghjyehmmt.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gqhjrrqbj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gddhobfat.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gspscfmxk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gotdwvwvv.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gmwyhlmbw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gfrxkavqf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gdwqjihif.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gscbmkvgr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/giegmdsqc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gkdsvepqg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gobmdsxng.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gnmhnzqhl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gzbyzolel.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gtekblxvd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/gcwqyfyge.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gzfhtnzll.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gdilvmpql.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/giggenbbh.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gvyablocv.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/glffwgtus.sHtML


<!-- 参考信息 -->