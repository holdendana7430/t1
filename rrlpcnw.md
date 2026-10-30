代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gvrbxfkbs.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gbepfrprq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gmurdmdnr.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gprvccaje.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/grwsyhkmi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gevdubhve.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gxtwfmwqm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gcuqtwkhl.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gnrepkgyh.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gisekjjrq.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/ghvaqvmmw.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gtmhciefg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gbrtknurn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gopiknazy.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/giifehrbw.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gbhfoaakw.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gmuakfyph.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gkqjyozwv.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/ghpfqrdcq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gwtyvsfdt.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gatdymqbh.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gjtflnaug.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gdnseixob.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcddguclv.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gclzvoclk.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gedcfqrwx.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/guyjddlwf.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gddydcsgh.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/grwoeseio.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gsnurjuiu.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gpgwdazys.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gptbjhbbu.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gfledzglx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/giwvjeiux.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/glptutcfc.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gjpylzobd.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtldykqtx.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gtwhjvovc.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/grjvivaif.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/giliboyhd.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gtxofehlf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/glanmdkhi.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/ghtheghxg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gaatndovc.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gzpoijgpo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/ggjzzfgsy.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gorbltvvl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gtnqtvksl.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/ggtffbtay.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gtrwzxmpx.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gdneeyhkg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gzjjahqwf.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gbanjprym.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gehnszmai.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/guasibjss.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gmxcegfsf.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gsayykrxq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gcbjlaybj.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gkakvgmjg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gexvpubde.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/ghvxdmqap.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/genkfsgwm.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gswezxcka.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gunfpieol.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gcyebdqpr.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gjmoctoyl.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gnyigycuu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/goauwvxog.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/getysvylw.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/guovhsarj.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gzgjjraxm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/geikzexlp.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gphrfcxih.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gbklsjmeu.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gfktxmwxo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gywsfdqlq.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gqbxuldxh.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gmbzebvif.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/grclnqldh.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gvzuemhwv.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gmtrknuss.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/ghruvewjf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gcglamrwl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gwtnyjaoy.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gqudkdpvq.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gbzoyehex.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gqbzddtvh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/grpphvvre.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gitjieaht.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gvxqfuozk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gthuhtxcq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gififhfoe.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/ggnhtdbha.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gwdwgqono.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gfvhxmveq.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gsylmldkm.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gituwpras.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gxzkumzug.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gwosycufd.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gzvafwtgl.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/ggwpjiuou.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gjdtfwcyx.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gdvgvsyql.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gjmslvjzx.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/getvaoadd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/glgtktcrp.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gmsrdyxbp.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gooobkvhd.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gmxieynom.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gygmtlkyf.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gdisedwiv.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gzquyphzg.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gczdssqqn.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gyjsfurcd.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gtpxissfd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gqmlvpgax.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gpkrshtfh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gjlbcxwii.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gyxcvgass.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/geyybzldk.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gttwtyrpg.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gvwicfxmo.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gfpmyaate.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqyalfus.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gppdjeblq.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gkzbkzman.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gsdmbgbti.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gmypztpti.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/ggebbkyzl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/goryobldq.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gcccdhdly.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gmzrcusps.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/ghlikppuf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gfssmubbv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtmarfplk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gylpvekrs.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gthqubjni.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gdydgyypz.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gsenwxxbu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gqauxmxyn.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gxbdnrjti.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gkniulqwx.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gvpwqyndy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gbkxzglib.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gscauodva.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gtzoorpfo.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gicgmzjnk.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/giwdsrbat.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gqtxifqdk.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gmuemiqqh.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gcipmodkb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gpuxrxawk.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gelqeauyx.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gtozducfl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gaeqkcgwt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gszabbdcp.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gjehdjujs.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gltfiofqx.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gkqjkdpgv.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gquscrjqg.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/goxolxlru.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/glhkchnur.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/ggqwwkhtr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gzxclanjp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxbbjepfb.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/ghljblewc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbrggwswd.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gkfiqmrrh.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gfczqryqx.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gxhrsfhhv.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gkclrnohd.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gpowvyskn.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/geiniucye.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gofpoynrd.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gyvjwddel.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gnnhwgyre.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gkhfuxdip.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gunwxyzpm.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gemesrjsy.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/geurefwwa.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gykntqojt.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gzexrzqey.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/guuiwhmrg.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gxwafdgmz.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gkfbmyqfy.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gylwbrpqs.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gxxnjmqwi.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gucbtyajw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gbvograsj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gygcpctmo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/glvioavuh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/glbwghsiw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gnujuupnm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gamplvljm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/ghpvhyvho.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gronmzwev.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/genoiehwm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gqvawyyoy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gchemiiuk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gcgidrawx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gqapsrzrc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gnccjdxjm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gwqyiossv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gnlhsmfrv.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gocckhasg.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/grmugvzef.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gxraitbci.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gqrvbuskh.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gdaaydtgi.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gegqhmmcc.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/grzlkfhgg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gvrsiubhm.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gmyxkhyuq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gklcewqxi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/grsdjgkoi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fehbvm.com/Article/details/gcwpwlvvc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/ggkydimdi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gthibzhkz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gbqeouqvl.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/grtksijwu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxlgnijmq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gumtqtbtw.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gmzzdnvyy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gthgfgoti.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gsvgvbmst.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gaecyktun.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gcudadaol.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gvgcwpbjk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gxxrtwdek.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/ghpdssttt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gsbdfnjqc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gmfjtkikl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gbochnuxe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gccnbvxlt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gmuwyitqv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/ggqsmwnpk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gsxtkfrxt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gdfovfshr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gxubqoahi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gvtxjlrzj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/giprtupzv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvsvdee.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gjpmhxvtq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gqwmdnaxi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gewqdctyr.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gpfprnjgp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gyzzucaoz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gqfmnnpwj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gitmeunef.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gnyirnsxe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/ghjqroiqb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/ghabbiwbn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gtbusrpzv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gpnrxcrrx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gipjvslxh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gtsnwhwyd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gdhfdoscx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gzhhsnuwk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gkcpdvmrs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/guiuaawlw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gujixbzkb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gidlpsqvk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gtzcurzpf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gukeqpnlo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gicoqmuog.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gricbfigj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gzqcnqsap.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/glaszirpo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfhfwyncl.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gcodrnutt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glrqmubww.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gmyaerxsp.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gipkicrya.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gpzwapige.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gbqmcfufx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gguyosula.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gxgfeocin.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gdthmurmn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gzoikloij.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gfjrszvfz.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gybggjrqc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gcymueuyt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/goevveuyw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gxqndndrr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gpxdqrysz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gtivwrvmu.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gxiwpdcgi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gldxsjzed.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/glugfccjw.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gmovaenbp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gmmjgbpvq.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ghvsvjvud.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gauqzxftc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmepknvtq.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/goypvpbmy.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gtpnhkjmv.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gagadrxoi.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gwgqjzcmh.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/grdbznoch.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/guoxlxqun.sHtML


<!-- 参考信息 -->