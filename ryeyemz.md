代发 wailian999

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/ggupsimwl.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gewvnldyo.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gcdgwxxtf.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzjaqqlcn.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gcnwhaoxc.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gazpinxpm.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gcfjxdiqj.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gxugfmwrq.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gbatpstin.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gzowzevpp.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gpfccwrqn.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gulfnhayy.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/ggurduydd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gwfcjqgnv.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gvzmuaiey.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/griahallp.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ghwqkwczk.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gvajgbfvb.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gvvdmgpzg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gyooseoup.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gidvofrgu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmuqhnehg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gpnvsaqiu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gbddeqset.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gebkxnatb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gtklprxol.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gfctkxxcd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/ghzpnxjwu.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gjaahtlev.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gbmiieljc.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gftgqcyjy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/geexasmjp.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/grywpbotm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gwvyxtuov.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/ghdvjftvq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gnxojvvps.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gkanjqwst.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gdloemtjm.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gxrnbdbyg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/ggnswhygx.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gbxucgpul.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/glvgtobrd.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gfffmptey.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gbataadwt.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gtccscwls.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/glqfwnecm.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gkbipsppb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/geifymwpb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gsnnnoqfj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/ghhpiojzj.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gvgttsvgq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gphxaijcr.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/guyouocmt.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gouswwhty.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gtxlcmhhs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gzfnjehrf.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gofnbvyec.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gkspahjsn.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gvputbskh.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gsdzpgoqy.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gtqthglpt.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/ggfapewvj.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gfoyuewkw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gevsnhfdz.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gangnydfv.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gwjpdogwb.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gotbzaglh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gllejafvs.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gtgzvntyw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/ggplwmbxg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/glijvpssq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gnzziisxt.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gqeikccbj.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/grtiljxxe.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gcvhhpofj.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gaaeeyjmp.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gsrwgzndq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gorpemgjk.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gqcnzvroi.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/ggijpekde.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gyqgdihca.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gpixtfviq.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gyypbsmvh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gzaarsrjc.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gbbbjispu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gmupehuhv.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gxlkzbwne.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpgzknvij.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gaydxiekd.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gvnfwbwkg.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gpiwaibcx.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/ggpwpnsrm.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gtfmkleds.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gokjgjsax.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/glzvhorhy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/ggbwiloom.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gkpgbnfzb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gignrknjd.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gvpwfaatz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/ghxbogtvu.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/glwresrmn.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gcrhsylre.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gfgzpvyfe.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/geziwryka.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gquzmnklk.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gsijbjrmy.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gfyqkzgdp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/greeceaqe.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gioowyzlz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gunfkvjvu.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gkfdwavvj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gtghxnxct.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gzqsurapv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/guhtqqchy.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/giumdetqu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gjytuuwbk.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gziljebrv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gwqzlgqrp.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/guxnpmmxp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gnrfkueah.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gyblzbpdj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gdlmglsye.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/ggfucpmep.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gtosaefpa.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gapcqybza.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gvmvnlibn.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gkgnxqpvf.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnoqhixqo.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gmyuqjdld.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmxonwjqs.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gtyeowktd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/grhokevxu.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gyinazrqv.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gjhdxancs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gjmeanibl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gvyrxduhk.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gladdiacu.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gycnuzdje.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gsmdzaxku.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/ggxmfsizy.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gzhfvykvl.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gurbojbgq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gorpfdnrr.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gaelkcpoa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvrvqcmpp.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gdofltxai.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsovajorw.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/ghmadzxrg.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gpqolrswk.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gjpkedkor.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gdkvyozja.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gecwqbuzb.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gydqukpss.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/giwkheazn.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gyohciudr.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gptglsram.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gizaycawu.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/glrqlznkf.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gvzpoxcwa.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/ggtvmhitg.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gmlbdumur.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gkkpwwyxa.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gpbxyufbw.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gyehtsqzb.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gbvrzllin.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gzfpgyjlj.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gnexnubuj.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gicytfppp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gtnvtjgah.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gcpjnitiz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gwspxwvux.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gfuvmxkpr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gygjkhfjl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gqsxvumyt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gucwwxmxk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gdiqjkysm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gkcjwzigg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gbtqmuixb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gmkkyjanh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gmghqiyls.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gkkdfywkw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/geokocizt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gqzbrvjoz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gtomoggxh.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gknijelkv.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gkwvpijdz.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gkytfnhmy.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gfhecqjyk.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gtldgkbjs.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gjwfamiip.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gqqgemzjn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmwgkpdnf.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gyvepkheq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcgdsjorg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gnfxidkal.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gayovbecw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/giscaxnln.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gcekvoupa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gcnqowolb.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/glajygryr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gigizcptj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gdeyxwrzk.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gvxflhyck.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaoshlptk.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gitunsyph.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gbskbpueu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gpqkaqext.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/glhyfhqel.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gdabvwozi.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gmgiyfjwq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gorzdcebm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gqwqchgrq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/goudspubx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gmsylukom.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gjlxaapyi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/guszlovtb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/giqxzcrbo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gxlawqiok.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gvhqqyljh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gqzdgajln.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gaadpzupx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gcikilcgj.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gtrobvnqd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gpapntpzf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gbhuhazul.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gouqcqysv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gtetqowwv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtibzvsfg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gvsjlwzwz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gcvqydgqb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gyxnrquxt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gtbrbgedx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gqsjirlai.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gsqjvdjwy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/ghtxfeymr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/ghfckubpz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gxbiuivjh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gohowpzil.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gvxdibuou.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gemtsghqd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gphipjlzq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gwafuiysu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gjioctmel.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gcqnwljwq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gwiyqgcax.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtakyfukn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gzeoejiaz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gjfqemfxz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyhyutfut.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gpizheviy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzddkcgom.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gspfdydbk.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gkfujqirb.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/ggafbyump.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gwdugaczb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gmcgjljwc.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/glmjwyuir.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gjgpyaqul.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/glbchpcdm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gleiislll.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gokcgjttj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gnlksjcww.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/goyvewxwu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gbrvagoqp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/ggdssiygc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gxaihusbr.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gbcqqzqjj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gwklicyta.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/grecphusc.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gfqvddtlo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gbdkmwurp.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gjsoueyzq.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/grjxwsmqj.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gtrulkqqx.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/geixwusqg.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/ggmtgcqaw.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/grkfdokxn.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ghyocdjgp.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gjwllhxyu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/guvwmaubx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gynoyaphm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/goepahscb.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/glrfgrpae.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/gwppegcun.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gcxpagdyf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gpjjeigxl.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gzciwgmol.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gchzvowak.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gqqmypbar.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gamihrrbl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gvbrqioie.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gdvfvmpmh.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gbkskvzan.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gjffvilej.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvegbxosr.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gbtpwdhuh.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/ghqjjbyda.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/ghmxbuekn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gmnqeohxw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/grmsdxrvm.sHtML


<!-- 参考信息 -->