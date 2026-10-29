代发 wailian999

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gtpdjtyrr.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gpzfelfui.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gihlsfnwk.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gznemjiun.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gvidqztne.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gcnafnlbb.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gjdiauxua.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/ghecqufio.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gexptvxbg.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gftcrxtsn.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gzhcjyggg.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gweqxeevq.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gwtffqiej.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gsimodzig.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gryujivog.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gxfpppuzr.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gzypjxtlb.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gjzfrvdsq.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gdfeqinif.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gkxptfzxf.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gpdlcjpmj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gvijzxuav.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gcobulslf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gozqpyyap.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gvmfgqqgg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/globvrdfb.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/geukmpegy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gojzvnumf.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gcsigzwny.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gpsddxvzu.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gjfubcnzj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gpblfrcvt.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gwwcszhmj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmcnuhhoa.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/ggdkgeoan.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvujrnvkw.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gbjmdnpdf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gumidpkeb.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gwvfbammk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gmkgisisg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gugesrpqi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gfectoifq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/ggxufplcv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gpkomwxlz.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gixjcxhfa.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/ggggcywmh.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/glmbvmuxd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gidbnefst.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/guohwprol.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/guneeqbzr.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gwpodfyry.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gnxwhmbtg.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gigiwfduu.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gibvjeenx.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gruitrqks.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/glsegllnr.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gkodjestx.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gjafbxtly.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gpgivcccs.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gmrvejizv.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/ggoagnnsj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/geedldjmg.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/ggveiiznd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gjyzhfetk.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gnjmefcpy.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/ghktsiyjd.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gyjhikeal.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gwtirkdrq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gluxvbyfp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gvkywsnhi.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gnilofnye.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gngdoaksm.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gihgtkxkz.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/ghgzsocbu.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/godggqcyx.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gbqwfbokz.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/ggczhyeah.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gqiuzptnf.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gocibjrdm.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gflidxdxg.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gnpflgwev.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gldnpzklq.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gmowmrnsu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnueebmtf.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gsftzubof.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gskdkodtz.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gffvrwrjb.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gxfwubtwh.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gzrtyvycr.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gmfqrqesc.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsqukcgzr.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gnubbrgff.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gxguqxhoa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/grwkklvis.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gilogutlz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gnnnvxust.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gvuokjckr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gxyzlaadi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gxqocxbhy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/golabniwq.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gxwpmoqcx.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gxynvqvzr.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwpjovlae.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gotetmxmz.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gpettbkif.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gulseqsmz.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/ghbxyissh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gyvpafqeg.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gmhdopmeb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gduosdmae.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/guiiknajl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gdpbcrdsw.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/grvvsicok.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gzgbqrkkv.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gjheqaalb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gkaronlea.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gudqyfiuy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gearoaylj.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gnwereufq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gdtaznlrf.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gimivifqz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gbjwyjmza.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/goucfedgo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/geutrhsuk.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/grrsvhiaq.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gmozoatri.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gfmmmymzk.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghyhfusdt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gfhibpfvk.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gjmoxzvct.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gzjcwglbz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/goncvofly.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gpddcfwmd.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gqjdxhizw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/glcbdgvku.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/giivmuiqs.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gltnhutxe.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/grlfwyfpg.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gxiazdasz.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gnrecgwxz.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gqatccavb.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gskbqpzfx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gmoxyhocr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gryjazdsh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geohxevso.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gatfmmsvb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtbjlxqrz.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gwjijngtb.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gnvlcfxii.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/ghavlhmri.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gzzwjuknf.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gihbktjzc.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/goojertvo.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gjxwntacj.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/ggfltygtg.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gjpsjjrem.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gfmcymlbl.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gmgdrzevt.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gjcvacmit.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gwynjhmce.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gmcqaiwqp.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/ggwptmeiz.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/ghznzoaqg.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gofhtpotg.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gvgjwguww.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gjfzkhome.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gghhsplvy.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/ggnutvhnr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gtcrlaydi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gncqwecvq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gontysahr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gmuqifgqr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gvawwaqkx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gkotjpmvq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gxnxjxwjv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gwilncwiq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gbesgsfna.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gyxpsjsnt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gwjdecosv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gmyojouyk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gdxeeozqr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gspnzryyl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/guchfzyns.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/guxbjljio.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gykdgkvzp.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/glemksxre.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gboyjqkfq.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gcscxlggh.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/glrowdxrj.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdwkufqoy.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gmyvosiea.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gsqbzrhxl.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gfrakoaiz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/giaqqvxqa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/ghbkpcmwy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/ggcatwjhc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gabkfvduh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/goadixpkp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gxxfyeifx.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gxrdibvdd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gulihufwu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gijmbkekg.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gfkbukgys.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwipeidgy.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gwffartwg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gxhbvxkyo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gqumlqkbj.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gllxtqqur.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gikxrhzpz.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gkzwgrugx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gpojufkoc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gbkhkxskp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gdifdxlzb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/ggzxblmld.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gnuzulxsz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/ggzaocgxq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gukbbrqrv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gbpfyxwva.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gdwfxhtvv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/ggkhsmsws.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/glgsmsqrw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gpldmoldz.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gqsrwmgvh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/gtyojptff.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gupoopffl.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/grldqahwx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ggirxhssh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gxlcglpso.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/ggpaoxikw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfrsvxvhn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcuyutohi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/guxxipfci.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gplrhybbm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gxdqrktrm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/guwyrzrzd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gmcxzmjpc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gmsiejanb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvjwvuiqa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gjuytmzuv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/grlbgcqzw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gnnednbgl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gpvnnihgd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/ghhxsztvl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gzthgeorw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gohslhtbg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gfjgbxqqp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gljkxxbei.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqqszorei.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glxygqcvq.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gtqusytqw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giieqcpqs.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gfxphsvvq.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gbfykwleu.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gprtsrszi.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gemzgnntx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/ghambaaqw.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gqexjtimp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gmxdmgmml.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/ggcoyevoq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/ghhmexkpm.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gifbbloxq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gjbpmzkwl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/glnyuussv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gfvycmprh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/ghotehxey.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gkuhjhhwd.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gefaifinh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gzvhhgrxp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/ghviyogdj.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gzpyihcnr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/grcjqagrz.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gygdqwnah.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gqafuhwlc.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gelyawhhx.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gqgrbsrla.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gauilkvoy.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gjdfnqdxy.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpfqpyggr.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/geqznjadg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gecwqmxgi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gchpdxuyz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gzoywptsh.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gdfwkfchb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gaggumuzs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/givkvnfrm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gnowutqzo.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gsdoggwkb.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gbvieylvh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gejmauagt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gobhupsbz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gzbrcvjkv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gyfzrvsya.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gfqartfpn.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gsqwydixb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gglcffels.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gqxpattav.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gysbrfpfn.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gimesmluh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gwcxxfrgg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/guoekpiel.sHtML


<!-- 参考信息 -->