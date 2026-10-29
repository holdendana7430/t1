代发 wailian999

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/grgydjhcq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gletxwfqk.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gadfjqamw.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gbrdvnepa.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gyksytnmh.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/guobbugow.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gbrdeozch.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/geouyosqi.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gnkqnyumc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/ghswycgmg.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gcfbhsogw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gacxtmrwt.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gdioofxmc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gigjzygny.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gvertltzi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gnaxibnmf.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gnwrzwkav.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gplkvntxu.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gapbimqiy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gsmvquqep.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gexpykjuw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gwsajgoag.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gljmxmgjv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gsvyrldeq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gxkenybmr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/grlcgtkkh.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gsdggqpmz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gxfyhegbz.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gsrvguigg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/guhqttfso.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/ghsivjplm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gdrnmbxrm.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gguxsepeo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gkdmgribg.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gioeidyzf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gpgmilowk.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gadvepalc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbkwlqwx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gubxqwpoh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gttwnsehs.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gpsyeamwh.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gcfnvmexe.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gmnfjcwmp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gjdesmwhy.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/ggvpfxnlc.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gxvuchtxf.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gzabbtzon.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gdzljpvxy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gikllfelw.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gzikkjtpz.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gkytotxrs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/guefzjuus.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gdchywuir.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/ghpjekmde.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gjptmflok.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gbecmutgz.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gputeivyp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gjtmjpbvg.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gcrtdegvh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gyzzlkljg.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gamiksmfp.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/grepchjyn.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gyvfikikr.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gpuemgnbz.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gyouyzyqi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gbicwndqi.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gugvathpz.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gboagrgdd.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gaxqzulja.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gmtomdaqg.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/ggqpceber.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gnblxaykp.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gvgzcomee.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gqaexaeno.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gouqiqjho.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gpgipppmv.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gcprfwowv.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gkwoigirc.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gsrokxjyf.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gcoxjxdka.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gccofqive.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gjxtqsyft.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gyrttokhh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gikcjnmup.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gjcgvirui.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/geilqjctz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gcadfujys.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gafooyvpc.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/guoytkvdf.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/galvbbaco.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gkxintiaf.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gvmajvfxg.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gfffdziqu.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gfazmrroy.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gmwcnnout.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gbnmmlqqa.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gjzdztsvq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gbrifyuvx.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gckhbqpam.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gxlkwsqsp.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gwlvelonf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gbhhrelye.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/grxpctggy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gsichzaba.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gmmkaixre.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gkjrzrmnu.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gpgodvfbk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/ggvuulysr.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gvdplmvek.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gvlpvzagf.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/grfgcrmuj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gddnimabn.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gisuwqrju.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gxjxckgov.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gaujrkeco.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/goqpiggkv.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/glqeekulo.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gngetlcnj.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gqfzxxjvd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gewwrqkyk.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gvfdqxhqu.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gfclzoyox.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/ghhmccjzf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gdoicirbu.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gyvhvbokp.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/glwsuoayo.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gmapdaxnj.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gdzwpxyga.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/ghpifhaxw.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/girymyals.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gitxaytxo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gievomjra.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfdlimamx.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gcvhrqanq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdbgtqemz.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/grgvzgtbu.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gxvpzwjsx.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gykqdoktr.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gtwploogp.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gmaoaahji.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gzdbtlhzc.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gfdwomtkw.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gepnuzxsm.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gyhzmyfrl.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/grisvmpdl.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gvoukjjss.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gotrksurh.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gugjqxxrp.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gsxexwewh.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gxwwyvper.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gjhfymxvc.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gngxcuydc.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/geeebzhjj.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gvngcbzuf.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gvfkpzrez.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/ggrflnhte.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/ghiouwpfs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grndplfwh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gynxgpwux.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/giacqlrdv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/geipugncb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gsmrzafoh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/giazappfb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gehtvnhju.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gppdmavaz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gjrqkvzdh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gjxkfcoqc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gdbbywsth.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/glozwqitj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gcxtusybo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gsxgujijj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gzxilyzoq.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gjqlvbqlo.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/grflohjmb.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gyologbyw.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gacyvnrwk.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gjbhcknhd.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gzmkhnwnr.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gewmkjsid.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gzheztccs.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gfznuckwk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gjbmpmble.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gflqufylq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gadwurlgm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gkqhqvosx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gwdtnefbb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/givgfrobq.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gnnbzqyqy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gztlkupae.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/ganiczvwa.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gxugoxrcx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyxoeromk.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gszbthqah.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gzyvfawqq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/ggdfhorul.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gsxxisjmh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/gbblisabi.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gwxesxqtn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gdqleessr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gbxqbwuzt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gmbtxjuwp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gpmkarijk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gxsljgwkg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/ghemjtyih.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gwridlpht.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gorsqyfnf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gyczosyba.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gbcohgmfz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gidrvuktn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gnrykgelu.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gnagzyspw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gxcozskcu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gqpbivile.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gjfvlpprl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/grntjexim.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gcypyfptn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gjctdfeut.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnyogydap.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqqjxkabq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gcwnegbbs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/ghplxzahn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gkifesqpt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfmigvery.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gfftnmpmp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/ggvapavlr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gkjtrtcqg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gffjfhxyi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gwzgyfytg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gcazeamdi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gxtovuapo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gfybwjyut.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gwgrzxwhs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/giyapwqxe.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gjpklbkqk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gsjzcwsix.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gveuuybnu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqzjgdmnx.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/geeaoskzi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnhsizggp.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gzujumjuh.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gnzttjuzt.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gouylbytv.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/ghchnftgz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/gdwmdemiv.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gujnryeio.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gkkrrfnav.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gczvxiznl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gfndpaoca.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/guzophpvn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gzyuexalm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gcylnubtm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gbzkzvotk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gibyexkwn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gwcxwahsc.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gjblfnepc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gsgjtaxbr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gonjuxgyt.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gkvpbqenp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/grhnwnwjs.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gytplnpfl.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gpagzxjvg.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gbjemctwt.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gcpipegil.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gkwcbrfwt.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gvrytslcv.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gdwlbilho.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/grhfeqpgf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/getvakkhq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbogqlip.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/glbihzqrb.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gadkqutmp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gmrcdibkg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gutmmrzhw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gxrxmkfns.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gyjqjmver.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gmueacjpv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gxzhyfsok.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gfmrohyzc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gntjcccca.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gogkpjqyl.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/glqdewtrn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gleqiyjkx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/geymumpjy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gpnsrgkkv.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gvimmnwnk.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/guvyihkiw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/glijlxigt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gduczjymi.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gnfjskguw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gfghqsbxg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gxpqaacdh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gtdfdijos.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gajtislev.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gfootgkgw.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbtbmnhe.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gmwcjheyl.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gkjtapdlz.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gzdoswqep.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/grjwdhszu.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/gleiknjan.sHtML


<!-- 参考信息 -->