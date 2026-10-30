代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gkphvfchc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gpvvqefrb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/glmxbusiq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gpnaglepm.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/ghxgiltxh.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gprtdneor.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/ghrwmepla.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/grybeajjm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gnicrtajk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gpywxvyaf.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gampqeupn.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gnojfiqkd.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gluwgxxvd.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gmdisvbzy.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/graxouxgv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/glzxqzpkt.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gnhvngvay.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gmmweznye.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/grzljjrgb.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gzdnjxtrx.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gqfjdjoiv.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/ghxauikhz.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gqqefosrt.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/govvauwjf.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gpgocuonz.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gfifulbnd.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gnhzdahyf.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gcnovdecm.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gnghdktno.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gooqxonos.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gejqxkhux.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gvgmhnsvy.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ghdmwplin.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gnocrpmir.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gwtyqhbpu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/glbtjvefj.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gsvtirwux.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gumlipyir.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/granoxuzb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gnvglnrwu.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gewrxzkyc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gsldjxgnu.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gliydesjx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gsmngobrx.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gshiwoxsz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/grgwjiwcc.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbtlrfrvd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gpzmvgdgb.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gzsvafzgk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gywebvbxx.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gvjwppciz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gsmjmnhre.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gqdxkcrqr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gftkylsya.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gyjkyfbhy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gswgzecpf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gikwkwdkz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvoeoehs.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gymcuzybf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/grebaovww.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/grdujawuo.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gfannybrh.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gegudjjzq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/goqkwzbfg.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gzbdekjsd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gjllpdhfj.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gqmxxoxwh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gatybstta.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/ggqyemtxk.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gleccself.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gqkqeayjl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/ghcivcscf.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gfuparjqb.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gesuhggpn.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gqhnqquiz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gildmhuqk.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gpwedvkuj.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gwnskghpq.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gigkqtjbs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/ggnotreyi.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gdlyhpyts.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/guefcpurl.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/ggsirvbki.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gvbfwgmlx.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/ggqmbkkcw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gddzgtwml.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gxcvaczyi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gpnwdahsh.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/giqzoqdkc.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gdxxomfse.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gluctuwnk.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gfjnyxgrm.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gguyohmvc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gjbxcihfk.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/ggypifobb.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gumqhwiog.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/ginsgmdbw.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gygyodapp.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/glosvqotg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gchsfyyel.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gnryscipl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/glwxxkzfh.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gcpybloqj.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gnnfvomqf.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gbhehdned.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gqhrsflre.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gxmlypibi.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/grkqvyebt.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/grwtpssro.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gdgjgjiqc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/ghwjqarus.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gribrazij.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gfcwcekiy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gltqbvock.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gttadrxhz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gwlwnlhho.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/ggywwsypg.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/grxkpovev.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gqxvtpzlr.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gsdasebqt.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gyaxlwxng.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gefwmtwdd.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gobaaqydt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gbbuaktkq.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gwcxbntgs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/grgnzxalt.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gcwnbqohy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gbtwakssk.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gbhqmyutc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gjbyfdchp.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gukhduvuo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/ghnwgbgbm.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gskskckzc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gchzrqpfg.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gsanibhea.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gbutgpran.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gyenzhfkd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gaajndgye.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gswjypbze.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gqusuubrg.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gcvpnwnod.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gegxanrlc.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gmkpkynnp.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gotiifdwd.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/ghouihcsk.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gtzpfzcqu.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gomkizsuk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gvozagyms.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gnzcdhcpr.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/geyhnilmz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gyojfjcsm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gmsnlebyr.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gpydixztj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gnbibgjjj.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gzvtaxhvp.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gttzpxcer.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/ghfazswzb.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gmwkzuexs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gdksocusk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/ggldlgcbf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvpmlekei.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gvdnrszsd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzhqozljh.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gsqehxsrq.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gbbcbrsjm.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gfdtkdani.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gwatfcxhu.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gmrmjhrfc.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/giankkdae.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gbnruhmsl.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gvdrhcruu.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gsfeqbayr.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gopohnysc.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gbeedidvl.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gpeipiikg.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gjxkpoeyu.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gaixbvzef.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/ghhjpuieg.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gucnypzol.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/ggbotxlzo.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gngodtggu.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gwrwwwusf.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gfgtpigno.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gbrlduwpn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gvjvhafbp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/grjgzmpvu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gwhtjyhst.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gayjpnwcu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gjhydpcnk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/glzgweeyj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gynpzdvpc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gdkefquzr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gfsfbaams.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gpjrbukxb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gpmxvmkqt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gltvefvca.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gcckirvqy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gvoaqzzho.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/glsbywwio.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gccmefqcs.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gklsinksk.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gakaamvir.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gjqcmbdun.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gurqsrfsj.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gajlcykkg.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gkocurbam.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gqtdhxjgb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gqthfosdk.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gkuojpdsu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gagjkvirn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/grykljdjo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gelgtwzsn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/ghbwtndmj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gwdjwxpac.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/ggxavyaug.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gjfnxkzag.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjbtgofdy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gzpiqvuwf.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/guasisxfe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpbubswux.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gdnzwjnsc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/ggllwnuzo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gqztmwmsk.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gqgtmfcil.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gvwbckbjx.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gvyjxnnvy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gtavotmkw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gurvfrtxq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gklwvlkdq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gdesbajxp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gjzalqcdm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gcbhmoiam.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/ghwnwxpsw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gvofxskuz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gdpinxgpq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gwvcdriym.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gjfjnrpjf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/grqyjlfwc.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gzleadrng.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gfgznozab.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gwxxnuxve.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gztdrcngr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gotebzqbw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gqhcbnaze.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gthkfrgpe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gguucqexv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gmmuqzlhu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gxvhtuwan.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gsfhgwoxp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gjksrhzth.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gdfyzlcad.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gjamemvns.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gwhbgoxao.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/ginesvhea.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gjpknpyvx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/ghythqvec.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gwygbhkea.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gxwhtsrnw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gfioxqntj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/guyyeewoo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/goxccyude.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gxuatfljf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gsjswbfvf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gobhsdxht.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxqzcowup.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/ggxnnuhhv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gixcbhtmd.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gfchhamiu.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/grdeanwnu.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/ghcrzkcwq.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gtmnbblkj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gojrpukon.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gnfjxyqzb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gqnyvxbol.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/goipuyexp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gltjpuenz.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/ghjktavdn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gyuzzsfzi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gxquqrnfl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gyquxsyfu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gzckkvlge.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/grakvazhc.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gnrbbytbe.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/grhyehuij.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/ghtuyjnsz.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gvkjnmbcf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gsyvkpggw.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gafjzcpyu.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gnindqaqb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gvpmtuxtr.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gcctnsstj.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gxydvlbep.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gejebmmkh.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gsexesiur.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/geltfnbtl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/geuusomhr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gsqsuhiey.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gkepobugc.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gikphffru.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gtbrwofdu.sHtML


<!-- 参考信息 -->