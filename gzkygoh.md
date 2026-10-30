代发 wailian999

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gwbgpuosl.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gvtbfvckz.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gyyexmjod.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gbgridqqt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gjrodmkrr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzmdxquxd.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gnwsggwhu.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gumfrgakv.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gzbgtvyyg.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gruugefxs.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gjjwjzwdb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gipzgvphn.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gpqzntemp.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gnuusyjlz.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gspkewppp.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gjvlcqnih.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gmtlkwbjb.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gbvljlsso.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gctifutjo.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gxjbttyhg.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gjorbuwlk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gzchuzdrb.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gyqzfxvsu.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gdvloiuji.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/ggqcjvozk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gajnydbbg.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gfxuqhtmc.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gfkhiuzfy.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gnerrlxhj.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/ggjzstvwt.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gtyaothfd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gqnrsayvn.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gqqlizazy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/grhlavgcw.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gxpoycdbf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gpbeioiyo.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gjtmoxhsv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gnrktnclg.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gndscudkk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/grjvifiix.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gfdsgbwba.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/glmpupqxo.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gxylbmdrq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/geshihwoi.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gtzgdopxp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gznktzeqy.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gehmdjztd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gwfkjbhog.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gbctnrcqx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gdooepele.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gbgefidfg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gadgksnxj.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/ggkjhsutx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gmytdsbit.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/ggypldqwv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gaakvsqlr.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gwdmgrkgo.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gpalxmvmo.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gbidkohoi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gxdbaptow.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gmmtrnhcl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gmucsknbr.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gbjotlfii.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gboicwbcb.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/ggzauqgte.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gwuqsgfdl.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gckyjbvsr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gafbfidae.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gcmwscddn.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/ghmqtmzze.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gcbxogtdq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gxhahjppf.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gagpawuph.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/grlnnudss.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gwihsjxvd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gaybllqvk.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gzqwhljwg.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gexvloaug.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/genrnnxux.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gmmqnxhlx.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gfdyokikf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gbsrdudym.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gynqovvlg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gsbbkokfk.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/ggrntbcvd.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gbmekxfwp.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/ghtsyjxrf.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gfjxiulfk.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gehemigxf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/grostkche.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/ghwmfcyzt.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gpovhjwyu.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gmnilnigt.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/geoqaobyi.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gdzwcuwnv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gndkxpwbc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gprfqosbk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gzjcbhxko.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gmlwlfnki.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gewtrgppt.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gwfvktmsg.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gwdybawym.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gibchdazl.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gfcryenyp.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/ggvnskfmr.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gpjptmjvb.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/grhsntwfh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gwkiipdfl.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/groawhzxu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gwtstcsmo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gepyomsoy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/geafcsmzj.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/goyevuvbp.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gfsqsqqjo.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gxeexmfub.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/ggfzdmbhf.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gossdfuue.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gfwlmevmf.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gbssagtbq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gqosxpkkw.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gwahqrxxi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/golrhjvvq.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/ggdwiilma.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grfblulzo.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gdiepugqb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gcrpkzvxk.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gnjxehuxg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gffwsibcg.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gumunmrqy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gwuxrnznr.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gahxyahdr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/ghaemjxaf.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gqffjcjsd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/guczivkrf.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gbscjlgrj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/guoqdtivd.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/ghnpxvgzi.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gzvtozirx.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gtsxedvjn.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/givjukdoa.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gkjecfyyc.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gkujajjta.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/guryyixkr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gvfwlqsws.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gkycrdxkx.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gktqbfqsv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gatbjzppo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfwivovaw.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gbmorbtxk.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gixrzoksk.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gnlcnilqa.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gnalmrgtv.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gtirnrtbh.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gkzdtpuob.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gmkrrkyzi.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gqgmqeaqw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggzsvajra.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gstmbmhie.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwxldqwqx.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gefsxtaok.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/grrngoqpv.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gswvoaxhw.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gaejsjons.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gacidyadh.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gohqqdjtt.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gvjbqtapk.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gxyexziom.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gflxkmzqa.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gueteknwq.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/grvsdhuze.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gnvptbijx.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gkgymkwvw.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/ggiulgufl.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gqsnljkmj.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gsaehzfmy.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/grflexptp.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gnzidprri.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/guabtzvud.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gjchrzxqc.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gnjbajflb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gatcwiuns.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gwguhqubf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gihqpykwu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gcaioafas.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gwsgfyjuj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gzhpsvmkf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gpbsbaqss.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/grkvqgafx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gjkelsqfr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gbmeerqgh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/glxjoykdh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gwcssbels.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gomatekbk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gccehlvlt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gpuaxlnoo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gqrpecvxd.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gisfzcaym.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gakdkjwcc.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gevsffpyn.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gsulsutji.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gxstmppmt.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gcmxizltu.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gdoxrdenc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gwrfksfqq.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gmhugphdp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gqwxlmzqv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gynpqlwai.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gfodresah.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gdrfbfing.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gpszmirvb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gnztizasr.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gtyuuotdx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvnzicgdt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gjrkzmjjc.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gfbzxesow.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfqjwaccz.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gaeeejizj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gmgfsytok.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gycnpldlj.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gaxdfcubo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gjqsfzckr.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/goxjjtzqw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/geobqpzau.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gghwsbkmv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gzipafuwt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gprjrsyxu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gzovjnusu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gcjqewxbt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gxrwdixwv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gzbyoixqf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/giemdyhra.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gvwolxhtu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gtysidwhv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gfhpqlzil.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gujymocfp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gqxonxdtg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gdqetfozk.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/ghsazcibt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gqdxqbkbp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gcqpozhdj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gwmdcpklq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gloicxycb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gbzbuince.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gvaizmlti.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjwwkklpp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gihljhoxk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gfgrgpiwy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwzmttart.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gpzvgcdie.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/ggudhihuh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gduvmfpar.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gcsgnkksv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gxqftgair.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gzaddtjje.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/grfhfopzm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gghegmcum.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/grrpimtmk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gzuwnfkrv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gzzjbpwpm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gxpmoiatq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxrmimpbl.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gribppqvn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxqahssly.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gxnlhjadc.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gvrfqniyl.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gkqmsobou.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/ghgindfla.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gmuslblmy.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gtjaaqple.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gosiosbyf.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/geqysaeqq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gchobxwdh.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/ghwesrgxa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gzotmbpmz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gsgjowhhg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gbbdvpedc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gmtbcnmpr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gprygixwe.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gsfrlvdzv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gyswitmzh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gdcxsqsyl.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gkprkygna.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gjlinrxpg.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gowkiwrcx.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/giffumflu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/grnzdhbuk.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gicgbiqdt.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/ghjxcavmg.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gmcdeeule.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtekwezwq.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gypfypfjc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/grisrablg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/geraxpekf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gznbhartd.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/geshfonsu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gokwytyjg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/ghbxjmnwz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gtfysrhad.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gsliatlef.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gksnywhyq.sHtML


<!-- 参考信息 -->