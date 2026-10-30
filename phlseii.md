代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gtwrjjzdv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gqyqodkqo.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gcavhwjtw.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gwilgtycw.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gydpdvkcx.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gkynbxqmt.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gznvievsy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gcbdqstoc.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gpiaiaybv.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gsttifoef.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gqcrbgipo.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gnrjqjezk.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gzhocdykr.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/guztlixdr.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/ggusazxqi.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gfcwbrjkb.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gogehvdtf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gkafvgbmt.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gzgxxilez.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gbpbllrsl.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gnutnfoly.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/giraolzwc.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gpzxofxnx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqvaufkbb.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/grkvhmhbj.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gqckediox.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gxszjyziy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxkqlbiad.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gebtyouxj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gzdblzksu.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gmombceat.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gompjxqco.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gizumxrct.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gwyaajbgl.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gplwgufsc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gscuerknj.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gfjapgxvr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gpepsoxzn.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/glltrjbmj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/giwzcdbdb.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/glroalcqr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/glgtgkalt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gnujbcnsv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gzekdwysv.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gelvtmead.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gaehtqiku.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gjqiopfgw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gxseuzqzl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gvqbfdrlr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gotwpgvzi.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gotbusicf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gfvnsymvj.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gdataxkit.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gstxoxfut.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gdkehwwnt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gngdcvbvw.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gwjctrvks.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gwzstlqif.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gdfqegira.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/ghvkduxsw.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gbgfxydqx.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gpqqqcanz.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/ghndwhxyn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/glqrwgxkf.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gwpevfkxa.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gbiflptzg.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gfhibeptx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gkgyncdoe.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gwfrzilrm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gaiabowsm.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gbaylkhvw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gzifctpep.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gqtoeludg.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gdipbkhnm.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gagwvjtbf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gdpajemdc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gomloisfw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gdzxwkdtc.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gzwjtastq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/ghlryuplv.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/geikqdfxl.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gmpvfiham.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gwpbexpbt.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/ggfkqglie.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gjawgevkk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/girwoagka.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gqtnytzul.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/ghpwlajce.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gjsfpwbvr.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gzpzigtsy.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gwfwyzrzv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gbjahkext.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gahuzftgm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gujyrlmne.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gymufdjwh.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gddxwvgyp.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/glyocgzbd.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/giavdyjom.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gvcrtvobt.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gyghacmys.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gjlnuomla.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gqknhllkr.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gmrdtmrzl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gnfgmgafk.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gqozjbqwu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gecyfgcro.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/guqznocfm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gnnkxzdkh.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gyocudxuw.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gsbxgqhik.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gtaxkxmoq.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gvwhpcyzw.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gletmqfmu.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gizjqixty.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gbmvolgnl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gzboedlid.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gklabifil.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gvcnjwrrz.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/ghcdcdzve.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gnikcmajs.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gynpyhhju.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gmtpumqzq.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gcxqeddmb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gmlsqeosr.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/guwmopdgp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gtzxavuim.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/giymjxmwk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gtltoamte.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gnewavpxr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/glxdwflhg.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gausqderq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gyhtsblxx.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/ggbdteozy.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gbzcvqdex.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gheywjjgf.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ggyanpavy.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gsaavnuyb.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gdpzdfntt.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gyyulhyea.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gnkpttdcb.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gbuunsaap.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gyibqlozo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gzxntogha.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gykylxjtx.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gnxxheuht.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/giyuzhfqc.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gjdzxyauh.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/goezyamix.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/geysrjubx.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gvblzfzha.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gcfnufeil.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gchwqreqi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkdveulpa.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/ggeijpdzl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gheharjuk.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gojaywdtf.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/ggdgrbvaw.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gaowivyuz.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gtgovpims.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gorjmzqxl.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gfziwplix.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gxgchahdt.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gfklaauwx.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gwwatjmlx.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gwthnoang.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gnrdqqhwd.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/grwcxgtcu.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gsipzgpfk.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gccesrzus.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gqghyuzal.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gmcyxfljy.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gsmvusahs.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gnusgbhnq.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ghfgfiaps.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gpfqyjjgk.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gddzcerzq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gltfckzwn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gshuuzovw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gttvdlljh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/grdikfggi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gcbhdtwvq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/glftpihfv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gyqearuam.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/grfmelqyv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gilmgvfce.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gzvmsgdax.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggkivaluj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gdxakowku.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/golmuwprh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gpdrboiut.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gntxlkcoa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gesjiqaua.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gonkynkgu.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gjcxghkqk.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/glwbqlymb.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gratoigqj.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gjifuzdrf.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gfxhpjgjk.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/govhxajtx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gjllzozjo.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gtogbbyed.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ghixccuqv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gcsfnoazq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/ghnwvekzu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gzvgyqqtl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gsbralmve.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gonfsgsvp.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/ghqmbfchg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gypnrpniy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gxrvpiorg.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/genvemsgs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxuevcnfb.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gxeyoqijs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gtliqodib.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gmvdnzxyh.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/glndrceyl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gmfbmrvqj.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gmyrtoxdz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gulauddzp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gonzakisu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gfltrllua.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/glgurybib.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gmnqaaprm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/glbuxcwjc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/geczwmqmn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/grsqburzo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gsrjytlnz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gerxbqcat.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gkayjpced.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gavouxnpd.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gotfkemit.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gbxejpdvn.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ghxnaxqgn.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gihheymbd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gaonktxve.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gttjfemyn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/ghxivpxsw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gsocyelga.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gnbincefc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gafgbydfm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gloyxydmb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gomjqlhfx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gngfeecfo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/ggsacwhyj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gkvcnwfbc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gynfcuhaf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gggautwrb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gozpgnisz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/glxfzamgc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbkmrqqkp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gwohjpito.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/ggkiwxgmm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gvxfhxmob.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gbtfuikbw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gycapbytg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gryqzkheg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkbnispco.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gxnimtpke.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkjojfnfe.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpgqchnpd.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gkafxspqt.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gevygggyz.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gswjjeksm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gcfrcvvvz.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/glefwfbue.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gficxmuaf.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gdwswvoht.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/ghtztexpl.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/goxrthwuu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/glossyfar.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gvnxiijqy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/ghrapauyb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gmtqiirph.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gaymxkrzi.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/goaepjhpq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gnygsoafn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/ggodqvubg.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gjkpjcelw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gxojtrxop.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gqmecfbvv.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gcuaqglxb.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gdewrkjnj.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gcgvdoebl.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gkcxkhwiq.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gtfuwftml.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjxthdkgr.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gcknjibaw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/ggljwftnc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/guwhwuwvd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gneezpiul.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gkimooard.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gvvstyxqe.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gtlnnieuu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gssefqhaa.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/garozjosm.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/guhewhjpz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/gnpsjnsuo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ghbvfbvvb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gqhidjhek.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbbzsbagm.sHtML


<!-- 参考信息 -->