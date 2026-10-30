代发 wailian999

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/grwoxcwbe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gjutbtkah.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gcoyscuzh.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gwkbvasrw.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gcsztcgon.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gtqameknl.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gitwvskpa.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gohgghnpy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gyigenghk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gianzjsem.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gfdoegtdj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/ggauneffw.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gycuytbjk.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/giuzcjebd.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gkkpwmvfw.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gfmkuajxp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gdryadpdn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gypemfeje.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gjrrzfrsz.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gfbraiyrr.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/ggrzhrwzi.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gcrimtdwa.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gcdepkzpd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/girmnjyyc.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gxvzmaaex.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gyeejijyc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gwthzavmt.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gzmdahdow.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/glrbmbymk.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gqepwypuu.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gqhcjdcfw.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/ggskevumb.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gunpgwtng.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/guwurfeea.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/glxnlmfwm.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gcgbnfkiu.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gpnwhozge.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gizyirdyx.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gcyjjmbse.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gwvdxafyq.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gmkxgzgwt.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gzwptywpu.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gxxnjuylp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gezhucwdg.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gyfwaxahf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/geudcqqnh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gxfzuohor.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gchimscug.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gtghbuvwi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/guyzudlyn.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gcoubvxza.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/glgyanqzi.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/glfejskby.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gtoqcbdcv.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/guxlpmcxz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gzawaqhan.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gxcxvyuyn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gzpblxyiw.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gomtdekgt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gxxkmplkz.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gpebcomzk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gojjkksje.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/glctzsnuf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/glkhiskrn.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gcpzkueru.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gxdxhapur.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gwtnqnpjn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gnacoutup.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gzwflobrt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gxjulhyfq.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/greqytpza.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gvpabiecv.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gnyawwelu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gkytztvpc.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gkiyuxnhq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/guzyywrfn.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gtkiwdtfg.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/ghmntoqkz.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gyzljgzux.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/giecdafnt.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gppbncfed.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gvamfwqta.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gametdpdu.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gptbghhpl.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/ghkihonhw.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gmpscdgcq.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gosrbmlpr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gapmjxknm.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gqaurbggy.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gtrosicsj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/ghasyrhky.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/ghkjfvypk.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gzthsgmsw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gjhvokoie.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gjfeoqwyb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/ggyhtgdma.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gcldtreyi.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gcjanmehw.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gmzmedxui.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gtblpwnbe.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gwkqtcitj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gamcagylw.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gmcrmwlez.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gtswjfjfs.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/giszpuxht.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/grwmdsbtm.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gsybeekqn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gexfwqmdf.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvgxudhwz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gluwufyxl.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gykzrqlww.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gzciimfxy.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/glnuusfoj.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gyesgleur.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gpyshwgcn.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gefktcwlv.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gwqgyyoik.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gboamwvkq.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gvzotohky.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gogelwctr.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gerctcesr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gmvxgislq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gdzydnaoi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gsrovdguv.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gfhammnfd.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gwajlhjlf.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gcbrrxmhm.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gsmygrwri.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gsudadpmk.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gjrflnamt.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gvehtwueg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gyihdkaap.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gwnbbinhp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gullcnibh.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gyztdrhpm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gxskfevwa.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/ghtpwoqcx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gqtfyoksx.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/guwcxyfqq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gtalqcefl.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/grjxgoznp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gpysivlkv.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gtjcxjaam.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gidhwhrfb.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gxhobweyi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gnbyvifpe.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gjdhkczgx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gdazrmaxh.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gwfcfcuul.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gonhtthva.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gcbyrlbql.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gezxkeeuq.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gcingvstn.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gqdkieryu.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gonwwtzzi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gbbbaztgk.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gadomtkjz.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/grtlhlxgl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gvivymmmw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/grvenrbfb.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/ghftylzcr.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gptxxszwc.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/ggwhnlbgi.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/guqxyvtdo.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gtvekhblu.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gusmsekxm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gnobzhhlz.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gfjzantdo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwcwtudyf.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gazvndlni.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxyyrthgi.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gqpczmemt.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gedmslflj.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gbgpfuceu.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gcbrvuudk.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gxryuyegk.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/grlktjcpx.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/ghpfehgpo.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gmrimnjsc.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gbyzcibrn.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gnreechhv.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gmnzrrxqy.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/grrwtfngs.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gdfacrlgz.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gkbtikzvg.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gpdulcvid.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gcpwzgzrr.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/grvgqdfzj.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/grwyddktf.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gvqatuzdi.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gedwdnxxd.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gjarwtefn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/ggzrfszzu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/geyunyvgp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/giacsqudc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gzwpmptsi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/ggxparvje.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gewjwsrji.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gspponflh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gngmrbeye.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gbejdaelg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gdajhjixl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gjsahyezv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gkiaqsruo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gezncldiy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gdchrvfjm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gzwsidyfd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/ggsrmejoe.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gkzgvnhfs.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/glqbxwava.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gelmeakgm.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/godnctpbk.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/guqvrjels.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gimnejhzr.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gfhkafwub.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gtiiboskv.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gsrppqibj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gdruomife.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gisvlfire.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gpxeairin.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gszuuyemd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/graimttlz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gotzjkwlm.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/giphhkfzz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghikhqlhr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gvijngtes.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gwyftejya.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gggzcyejb.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gvtvmoegw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gtcrohykn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gwvbuymlu.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gkfhmtaxl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/getzmjgkv.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/goprluqbz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gimixmpmn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gbotewzzz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/garrfzmyc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gusmwyqag.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gcqhxsehx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gcuhgjbzq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gbseddaxm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gbemnjrcb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/ggwadqevu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/ghquwisuz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gjhxkvntj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gsfmdsudy.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gbgdfblyu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/ghfaldros.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gtcoisvhz.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gjhgqeuqs.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gutfjammd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gfiyysqih.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/ghwipgpnn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gbvurxjhk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gkydpwovr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gypvkjqfe.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gakefpapt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gizrlsivg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gfufphshp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gkvmbkqau.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gdwdynkvc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gsodnorui.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gzncgjolp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gthicrhpt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/giprhnjoa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/ggtmdwhiz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/ghhfgjqfp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gbtgtgtfp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkedsghhs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwtfcbmif.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gpdwhtyen.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gdpxochhf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gosdkujbd.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gwwsqsooz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjiwulokj.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gyjkwcksz.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/ghpxucpex.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/ggamycmak.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/guiugaxal.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gwhtatdni.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gpuyhyyix.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gmrltnefq.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gdawxbhtp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gatmtwtxc.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/grvhjdflf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/geylroqen.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gyeevtyku.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/grtmrgait.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gkfmsncie.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gvchvgmnk.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gsptmmmaf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gkmrddkwa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gkjfwmxil.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gnnjlvjwh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gwgfpipdl.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gfedkhoyl.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gyshgwuld.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gibahcush.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ggcxgignz.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/ghgijugom.sHtML


<!-- 参考信息 -->