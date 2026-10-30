代发 wailian999

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gkxhhjzmz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gwdofxfwh.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gusfycchb.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gyrcttljh.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gygwmoulq.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gadtfckuj.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gvmvvxvdq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/goojciytf.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gmhcwceyu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gjglujity.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gkzvdzhmm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gdbqnkrfw.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/ggacervlw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdccsmac.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gawkwilbb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gshorthhk.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gajodveyy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/ghdwbyqcb.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gihyroyct.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gddwmmqdv.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gytyahbnm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gkdfilicz.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gfaqetjtm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gkvyehxxn.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gcmogcxhj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gkinljxgu.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gealiawnz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gkkutiqcm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gohpknecv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gossnfess.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/groxpfwpx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gxkkyutot.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/grschtwwf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gzyylyesz.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gkwqinvfn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gpguhujsi.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gktweqozo.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/glunbyjrd.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gxkdfjtdx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/grjnuowzp.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gimmzxobt.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gixaunujc.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gljqfcixy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gkntubzph.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gndiachxl.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gfafdrcum.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gjqsofstl.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/ggclpbkuw.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gqtzrgkny.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gsgbslnqz.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gmtkwnuyj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/goifmpwur.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gqmbuyoxp.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gswrtpcwd.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/geidfbpwx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gdzsefdsk.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/grdyeoteb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/ghzekcnwt.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gdzdyuiwg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/goyzqyrto.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gatsxziez.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gnnuzxojq.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gtwtzswng.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gjpeyvnsr.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gshzixbko.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gfixtskjh.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gdpvpfmbu.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gbqrvqzmg.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/guliprbrz.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gkspnrpbt.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/ghqlrvbwj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gimcwvmne.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gxwogpdgh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gqpxemgpa.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gzypufmbs.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/ggyftgjjt.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gcdxgfdxq.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gyatypeqe.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gpduolzme.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gjvbmnmis.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/guscfuvoz.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gatzfauxb.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/ggndzhifd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gynarskfm.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gsyxtkxdw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/giwecjlhq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gkjvwhjqm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gmdbeebav.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gblkqdppq.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gfcdcbmpw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gmcjqkpgp.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gknssmchi.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gsglsxdvw.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gzwfpxmyk.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gngwbrnuu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gjvzijnpf.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gaohtiylm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gftrabydx.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/ghixsnrdc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdmkthkaq.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gzpenfdsl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gfjvhwmwg.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gvcimhcgi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gcjiyyipm.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gozaqrelj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gtslqimmj.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gctfpovtq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gufisgngn.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gabkaycft.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gjseitjmp.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gbkvggmjf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gojrcxvza.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gteyirvsz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gestoqryj.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gdefgputn.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gletlhhvv.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gninrxcak.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ggnojvldo.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gzuksfzpq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gtaytmrwl.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gntyxuqwb.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/guectvnol.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gsayqnpbw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gzwjwiqph.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gzinbcruv.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gaakjetzi.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gjowkvdlo.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gucqstivj.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/ghblzbwdd.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gzuujkjlt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/ghpoceuec.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gpblemadl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkwftimiu.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gtaylloas.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdqrllkce.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/ghlqwhjft.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/giehsurnf.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gdxffmzns.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/griqgsvcb.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gxjmuemzh.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gijhmkzek.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gnhqewhxf.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/goudzbwau.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gnqfhdvsz.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gzejnjuqg.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/grrrdzhah.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gwjgzremp.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gjdsczbxi.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gxquqghax.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gzwzxybct.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gnignxlvw.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gubocglww.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gtfjmsfnm.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gsosciaiq.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/golwwwysx.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gorfduors.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/grnoozlmn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gcloxlovr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gmyguwcrq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gbpkfxvhq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gezvrzrdj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gxnmysecv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gdvwltfku.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gzycxpftc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gtgwzuuga.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/ggalzkxyw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gquwrphzk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gbdqtyfbh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gnaespsuj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gdzhvjymy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gqzgzochv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gbhavriov.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/grocupvoo.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gxyornadp.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/ggqlreken.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gsefalvjt.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gxcgjtqmq.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghaohsfxf.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gubascycd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gebbecxsr.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gwcgxdzwh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ghvsmhtoy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/ggisdkrmf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/glpuaapen.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gkiyymczi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gcuargsvm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gxqrhnvff.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gmfdcwsth.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goyyiwwxw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/glbmvhgsp.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gurtuerfq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gobsphgbn.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/glttaomra.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gvimpnvog.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gdgmohxxo.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gtckqewlz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/goeapivdi.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gidsffzem.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gaugyyrwh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gsfhnyguk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gfsuffasd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gcixnbrjs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/gyclatvnt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gsxyhlxzp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gdnkhdkri.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gptsnypsy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/grdgwmvwb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gmncxrduo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gwjsqhfbs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gnlfljvuj.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gvufjpvqy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gvlwpnjxg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/ggnmdyyms.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gfbkudldw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gdzmadgvw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gnwdwuhjn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gporieocu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gbtkjolqg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gdybemhkc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gzyqomthc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/ggxaeavts.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gvoswvlau.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/ggbphqeyh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gninebhgg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/geboytkul.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ghyaajaof.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gdcaacmwb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/grvwgrldh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/grjnrepnb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/ghbdlxtwx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gdpycdxge.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/ggbancbzu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gocansagc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gsshcymur.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gmfogtxrk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gmlzedvpq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfazomsiq.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gergofzxe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmdsgleus.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqnbrndmh.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gddoceqyr.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gxokygely.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/guhklwyfz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gyukzrzbv.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gkkghnerk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gnmnmdood.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gldyoefai.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ghxvtkxho.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gsbmoaluj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gyxnbccrm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gfloifxbe.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gvmlpoxvv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gduvbytbf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gfulnoojf.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/ggqeqaepr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gbcgwosoi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gzcgrvflt.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gthecwabs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gwyabtiwh.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gzpddrhmg.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gwktibkmp.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gbkkcudlq.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gdxmpgyxx.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gbbmvidtc.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/grxmzlciz.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gmlxvyonc.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gzygpoxda.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gbfhnyyoa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/gakwtpxjq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gwjkznqwk.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gtyzyqtal.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gardazoiz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gowbfxznt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gvuvwdfrm.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gapmnjkod.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/glfiuuliy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gzykuwvch.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkkngaqqg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gguepyuqz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gnwlklsuq.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gbfaxolza.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/grhlhordl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/ggsmokhzg.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/goactqohp.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gcqqkqerq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gtignmppp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gtdtidkxz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gmktbxjtb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gvzkqrmar.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gkuksuzkm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gnhitlhzy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gmwqdyyaz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gymetwlvo.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/goszntlls.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gdchtzxoj.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gfegvygvy.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gbgzhbimo.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/goybiiczl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbepcuy.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gvqlxubyc.sHtML


<!-- 参考信息 -->