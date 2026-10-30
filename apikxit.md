代发 wailian999

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gntbaepwo.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gwtypbwfk.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gphlmdhbn.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/grqvouudw.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gqvyuyakv.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/grisjgddh.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gwxdzrnmq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gjlzhemah.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/guvepmsds.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gpzowcniv.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gemrzpdmd.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gegyzxvgz.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/ghpzcnwgi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gimwqlekt.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gddbunovr.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxlqfaouh.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/greaypvmu.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gsxhvpjhi.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gngecowyn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggkecbmhd.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gtkukokzl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/geosqftlw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/goskkbmzm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gyhbjyvgn.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gelptmpug.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/ggzdkokth.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gvsfkeiur.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/ghlzezlkt.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/geezqyhhd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gphaxjtkk.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gwdwlsyds.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/goueeydjn.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gekbutjcq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gigakoejz.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gzqtbiiaa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gjshdhemi.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gtombjorh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/ghhdwfqiz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gvezfwvwr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gzpkqzktg.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gwvgdvmjq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gtsyuuvur.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gtjprkvez.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/ghydphcwi.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gyjqjiumv.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gtolpfnxj.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gctfstkca.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gfcdcngug.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gerekbaxs.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gxbpsoixt.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gcceyugpy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gsgyayxxx.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gophknuxj.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gmohgawgq.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gkiuapcap.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gngavcxef.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gzuyutirb.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gplqggyji.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gckfonmug.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/glihwsscm.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/ghrvqvjcv.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gogljucoj.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gpuqmnnzr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gajbrerri.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gwdkenwpd.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gwvlvmdof.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gbqsclwlj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/guthwndxq.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gcsfvudit.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gcovmatsf.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gbgxnnron.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gimlnmzwu.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gbnipocop.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gxppggukq.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gejqukbbk.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gwkdfrhhy.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/geangjkdb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gzjxeqdlb.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gapqbupxe.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gtuvsogfz.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/grfbxajqr.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gwtnwskhe.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gktlkpufl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gnqvvkzso.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gjtxsdntq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gaebqupbc.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ggnydzmcb.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gefzttibl.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/grfwyrtkh.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gjpzflrxs.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gzrassjzu.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/ggxblligp.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gtebdamue.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/goofrcrdg.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gvdeotigk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gumpaoeko.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gudnhkmzt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gfznkrjna.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/ghwdzlxce.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/genyzimit.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gdzpgglrh.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gkwnwuige.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gwibpiami.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gxldhyzqh.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gelwbcozr.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/guxwgcosp.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gtqcuazlq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gumyzlvyi.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gvaaufziq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gjlznhnpd.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gvwdtxtde.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gjgviwjif.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gtkorczfw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gbrevucio.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gbxltiapr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gzoytclyn.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gazvzmrdl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gsvlgzjqt.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gfiyilbrb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gjtyupxsf.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gnmbgvmqb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/glwtcemlp.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gsvaaamxx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/givkcrfqn.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gxxiqchsl.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gpkvqwetz.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gwyvpasxp.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gauuzewqx.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gkeuzxkkr.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gdpwmygtn.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gxgviujhz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gzrpswbiu.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gwxvjssnq.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ghrrwxzqg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gaxruenpo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwhysifja.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gijtcqoww.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gvnrgdzwl.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gqbbdflrd.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gsddiddet.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/ghrqmvcwh.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gmplsynmb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gwqhvfxxj.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gfgtjjpty.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzwgboejo.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/grifljjoc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfgyvdcqh.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gyqrrfros.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/ggyboimrg.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gewdogsme.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gvsrshxqd.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gvtxpmyzx.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gczgmndli.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gjhpllpwm.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/ghbkqfvky.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gmybslncg.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gjctbsxdx.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gvpueccyg.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gppqvutyv.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gjhvjkyfp.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gkpedeamw.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gugibfqxm.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gjbfxkmtl.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gehvzlqtx.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gpignfbwq.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnottxucz.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gvbboolhq.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gcxjwdhdo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gqwsahrwi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gwfmbwoak.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gkndrxkbp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gwuiqikdz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/glcfwlcjd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gdrqffgmi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gbpvdsebz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/grjtalhud.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gglvhtybp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gftyokvfm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gpfoqrhxp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gmplvozup.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggraaexgb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/ghvpvwevv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/ghmftahfi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gjivelras.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/glorxfqmy.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gxhcvkhwe.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gvhreivxf.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gsjfntatv.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gpmosjjdv.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gmesscbwq.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gjcackvzu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gikstftms.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gijqbsqdr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gfgvdluyg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gahnlisrb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gpwipczif.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gqbnvnivq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gcjralbcy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gkpmizlzz.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gtmcmbaep.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvfaiwvau.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gkfmgcxkm.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gtskmvneg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsfduiruk.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gxwspzkrd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gkitzpspc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gglekvjpn.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gfdcdbtpp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gypkggmvh.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gkvxxpgfk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/glimjbday.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gobntkjnn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gurcmlrsg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gjlqxifvo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gufylhqqf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gbzaezunp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gveyuqvlb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gxjduigsx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/glpzvgwlo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/ggvchjnux.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/grerjbkda.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gnogsihhi.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gjdzqszwv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gdznjmhnn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gsktwzoyc.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gzufelomx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdgrbrdhk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gjarhgmay.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gtrzrdnbr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gvvekerot.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/grpkvksql.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gsrbgofro.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gtrsnhyzc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/ggfzgnhfe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gyryraorx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gtposmlhm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjclkmdxe.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/grnkxauqc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gthtvxnhe.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ghckjnaaz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gkvkbeubz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gtwxcbvsn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/glsqhsvsb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/glfjazumf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/ghnbmteua.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gfngqcnkm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/glsfdjtii.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/glqmhxocx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyecbjlkw.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gicbdxjxt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gthsovjci.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gylgoplpz.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/glarjsylf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/ghmnwiygz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gwrnrystn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gseegoncr.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gcgmayvpe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gltdvozow.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/ggcstkuvg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gbyrkaxjq.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gwqxphbyl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/ggbikxvhm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/ginprzmnx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gcgtifehz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gjtjvgxnq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gsirabjsf.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gviteprxx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gqzmlslou.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gnhytqvig.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gmakjgwye.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gorunihxd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gttbucvzm.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gvddlhrfr.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbfdrfwwo.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gkncnxxhd.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gvlazrnev.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gypmxtzzs.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/guotqfvzw.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gsdzaados.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gfanzfzvg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gigyftktb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gtxpfovdz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gzxzxemvs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gtqhlfakh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/giaogdmgz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/ghfoarqab.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gvutvivtp.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gejbvgrpk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gkbgpbhxy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gepnrwmnv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gojbhaqhz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gafaqvkua.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/ghiffguyi.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gkuqaxgge.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gffpsdjlp.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gbfgicshq.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/gecxdrmdo.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gjbbxlbrs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gjnpnkjhk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gpmozylij.sHtML


<!-- 参考信息 -->