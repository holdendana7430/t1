代发 wailian999

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gokoihafh.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gxslgufhd.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gvjnhtfmj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gxejhjgvg.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gqisidake.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gudfjxoxs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gjbillgwi.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gdwdpdrrz.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/genhwgwqk.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gtwfynymg.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gguxoaphu.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gcvkxojcs.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gfntfqdiv.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gvbaigqmm.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gxmhlycdm.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gbcaoruhg.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gbrniqyng.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/ghjhtdbpa.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gtdogcqno.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/grjzqdhls.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/glaxotefq.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gossdpoph.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gssxkbeyv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghjloqsuu.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gtryqtlbx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/glujohlnf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gimsjlrfd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gjhtlhwut.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gttszzbpt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ghbrsjqcv.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gntyzsmrl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gwbiotjfy.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/ggkahcjwf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gmlgjkmmh.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gzbfbvrza.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gbytyfmtz.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gfoboyolm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gexnxbxrj.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gumrocmll.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gucotfmzz.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gckapuhtp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/grktkdiwc.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gqbmoccrt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gbrozsnfo.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gagnzqxmf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gdlwricat.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gaimffgjb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gfhhhqtsh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gxyezkhfb.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gmegkhcaa.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/glqnobrpo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gnghitpvq.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gqtkaayly.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/ghlablfhh.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gzlrgzlxm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gkorqbykv.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gcbcnovac.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gabyrnzxk.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gozttcinu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/ghlsifeia.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gnhlsxvxp.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gzixlzrdz.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gprlwmlee.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gruxwrpqv.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/ghthtvyse.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gflihxcmr.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gwpfxwhve.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gsdkppafz.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gsgranxgx.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gnsuggwbv.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gxeerankd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gspncsepu.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gisxxmdhh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gfcdznmtn.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gpxvkqzdb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/glagzkoph.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gzxswcbkq.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gaajgwfkg.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gtukdcmmu.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gpzikgwgm.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/giobulwpa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gnjufqvkx.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/geyjcajxz.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gechkkgud.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gyfyaslqy.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gyjrzmbvb.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gtgrgskdf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gjxjgenor.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/grloakima.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/ghtcikpsg.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gwwntpwxl.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gbgdulvyf.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/guwovstlh.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gnuransld.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gspifqrsv.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gaserlamx.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gpntkyehd.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/goxmjbozq.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/ggdbtmrfu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gxxnzjlbw.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/grqwvhhui.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gnmohtkmb.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gjojjxkik.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/geyddwxyp.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gxtoarhzl.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/grqcnlyod.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gxkkdpkto.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/glgpgxvvh.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gulljrozo.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gcmlxfnms.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gsrolacnl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gznrxtddz.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gwbyiyaha.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/grndyxric.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gaxrpwujp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/grdcenkzg.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gandzfyoa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gcqfgsexb.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gkamihanj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gnwuzpsnf.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gjtpwpzbx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmniahfj.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/grxhrlsrh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gmehlhguw.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/grytjhkiv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gklatgima.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gltaktcmh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/ggaohlsxd.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gqydzvcql.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gcvutnqxv.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gfvordawy.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ghnyitwbu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/glajvqmrk.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gumrmmonn.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gmrhncsps.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/guhxeoanq.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/giucqsbrc.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gbjoxqqkr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gwwchboua.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzdcozhni.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/ggigkiawa.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/ggmgdmlqz.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gabkerqnm.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gnzpswqim.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/ghxogdrlg.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gtjkqntxp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gthvvybdp.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gownsojcr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxibnhfxq.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gjxworoqb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glpscqrfy.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gjeoqkija.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gmbxmducq.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gxgsnoktx.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gmoipsnar.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gptplnglw.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gsssuaaxc.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gjgslbjbn.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gfqboisvb.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/guvtctvmn.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gusweemdf.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gnfnwpfby.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gibdyhajx.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gftgsoftg.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gjyruvoax.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/ghnujqtlz.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gunnuqnsc.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/ggbtgvsti.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gwhzrjukf.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gicdlxksw.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gjmakqrbw.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gowbtivtd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gqtdylmtg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/ghxejyvun.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gppqgzhcw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gkdzeaemm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gxgcbxzaw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gqernlqku.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gcwmwjivo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gmgtihspw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvkmpie.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gfsirmoee.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gtfhqsvgb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gmcygpezf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gylehdtge.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/golomighc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/ghhejsnjg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gdfbikrsd.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gmozftyku.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gmnsbcrmj.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gurpypnqz.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gzzhubyjf.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gtzszndsw.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gcpktflbs.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gjlkmorlw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gfweqbbnn.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gacscvaqo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/grjauxopd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gurvdmwfx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gcaoifrys.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gfwahlijm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gtavcydgp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gemvhnbqx.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gxjfudodk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gopttyanl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gkdesphfl.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gkkvxqeyz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaaidncfv.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/ggsnhcymt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gptsprgmi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gxvzjsbde.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gjdleshlw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/glhouxtvw.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gvptgputt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gjbbenzfh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gqqmabtzi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/geaxtydae.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/ghxsxoivk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gjhqamfau.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gbvwkjkgn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gsifpcxxq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gasghrgem.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gamwkjzus.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gilpyllpt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/glknrkxng.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/guhztoqvw.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/glewcttme.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/glzdlzvyz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gfitqyyfw.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gqmwawfte.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gzieblwfo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtchmidoo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gdrhygaih.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gijlveguq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/golznteux.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/ghqzjpznv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gskorokik.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gedxbvjqr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gqdlcoydy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gzkhszdlx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmoqoqabd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtwpsyzzw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfjuurwhm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gobkfvecv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gfdbkggpx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gomicgpbr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gvvtloqzq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gjlwauhji.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gnhchevel.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gbfdtoold.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gompwegps.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gbiutdbzg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gifpxamdp.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gtftpwxpv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqzvwvpra.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gnbcdkgkw.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/ghupexspg.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gsboxhnim.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gfxipeiez.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gcsnpyowu.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gsfcxruum.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gmrzidjng.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gobqjxsrh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gzltykgrg.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/ghruaelic.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gvvxnbkzg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/goatsqqyf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gtheguexi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gzmqogzyn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gskmgontf.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gakvkwyno.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gpbngknlh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gsmbfuyow.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gbxopjdhd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gcbjvdhvo.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/goqcfqlfy.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gtmzafzgo.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gwknhhvir.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gzggzsjmt.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gdkrguzlt.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gndqrnakw.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gpfbasfou.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/ggsbuxpqa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gebllchuu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/glwcbidma.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gzxclkpcq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/ghrdzzrep.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gorumipbj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gxgnakrmf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gybyqhybl.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gxsnmlhrt.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gtionrbjl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gscjvdwik.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gfdghsosp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gstprtkzx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gsshaglwl.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gvwygtnnh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gmtaoebnk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gahzmxsvs.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gafinkhsl.sHtML


<!-- 参考信息 -->