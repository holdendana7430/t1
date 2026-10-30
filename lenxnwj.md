代发 wailian999

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gzddmhylq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gpbfimale.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gwkrgauia.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/ghvmexvkn.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/grojjccxv.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/geezeygul.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gqeaofsen.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/graptebnb.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gzwubzvni.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gcxtqrvio.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gkonegaaj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/giykdahpi.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gklvpafrh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gxjperikm.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gwmqzmfsb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gjiwkjidj.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gargqjfyq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gbornmlyl.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gvkyhoybu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gphehhtbw.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gqhhzylrg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gsenkjcny.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gxszxoedy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/godkjiqis.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gubryzuiy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gvwttbien.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gpdzsrbxp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gxazidlxb.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gujnvggkr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/ghxdsqpeg.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gimbsezcq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gwxswteuu.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gfiaqovom.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gtfvcssjb.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/grhkzaowj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gfjoljhkl.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gapdzbgde.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gzmnjidjs.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gjhrdsgne.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/ggwfkakka.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gpfaysovk.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/grnoywrua.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gyxjkkuqo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gpihypslg.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gubneuwsw.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gwvahwwfx.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gmwmzpzdw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gvzlxwyyh.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gndjmkorg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gvmhelbub.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/geetoxqpq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gnlmvwthd.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gpvgnikxq.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/ghoweyjxi.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/ggcdbbrlk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gewtbztkc.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gisqfjkij.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gjzibnrgs.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gtjjnceqw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gpjrfbqff.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gtgeplyzj.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gyhevttsg.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gpjpgdaoj.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gqcrvyjfo.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/giwylwfvc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gaaagxefp.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gxunomnpf.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gzecobdaa.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gfaevefgo.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gbsdkqcny.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gazqmpwbw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gkkhwnegt.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gsynbfaiu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gtirvevrb.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gmyoktgzn.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gosjlesqq.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gnuunssxo.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/grrdfzcyb.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gbluexrkz.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gaaxinwyr.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/goqzqmqaw.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gvgnptgpo.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gnmerxewy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gyznicfde.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gfzlkjznp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gefgsnxtm.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gdrhtwukr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gbzwlcwif.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gvgyqmvsr.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gwsdugjva.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/ginlouqxt.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gicrwwqqt.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/giaxczlow.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/grilidlnn.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gjurgetxn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gtpcmsenq.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gowlobtri.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gcobddale.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gxzxjusvb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gcavxyqth.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gxlkabqfw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/giywmijpr.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gwjpdllmg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gjagwmlfo.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gfbyglych.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gnbsrejyx.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gaygzzcdy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gtblykuhh.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gombeacrx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gfqeofnlp.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gxslmfagc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gdaqobkqf.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gadhivjno.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gjyfftnyq.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gapermwzb.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gjtemnnzt.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gisgdabzf.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gdhrcrdwb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gfxbhvuqf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gurrkweae.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gavariqfj.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gdsdxsofe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gdrtwudvp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/ghasacyzi.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gysirwcup.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gbfeunatl.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gjxfbhahd.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gzgzwghom.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gcpaaieyn.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gntdudtbs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/ggwmdilcl.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gdckczxin.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmzzadslt.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gooelxgtv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfxtnjtdz.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gjrrskctm.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gawpdwptl.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/ghjjcrmke.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gsebrzydf.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gojkwvfbu.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gjoyrmjbu.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gdodrzvqw.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/ggnurzmer.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gxtzcjize.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gutuzzbsz.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gywctmvxe.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gmlbbqdeo.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gnrnhakoy.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gbpilboci.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gpxyxvotf.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gwxfzfawp.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gymgklxcy.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gfloufoct.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gnlxqvfaj.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/goxvkdmwr.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gswcptmvr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gyrwzdkuv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gcbdxwggd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/goxbwyxmw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/giffxyjwg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gpupbriqk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gtlsqrizu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gihqfhmlk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gruflydyi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gdishiumt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gtyustiei.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gbrwgevgm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gghqeizbn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gbcpljkcl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gyraozjfr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gtopspotr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/glxkhjyou.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gtizlxqey.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gkymarvvf.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gobdsjife.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gubxwzull.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/ghjivvyor.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzubmusyg.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gqqxlvfzl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfdzauyfw.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gwmcudzav.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gfzrhxnnu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gorvlejqj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gwteskkai.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/ggeqxfwvm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gewrjgebf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gcdcxznts.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gnbufazar.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gevushprl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gdyacuwfk.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gnjzfczld.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfkviadee.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/grelgnddy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gzsycestn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gseftvzpk.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/golbuwzeq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gfhbqdyte.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gayzxkvxx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gkrbsrwun.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/ghlnikaei.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/ganvmuhqj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/glpzfgjoi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gliiuvmwh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/getwltslx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gsuyrpqkf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/glugnoerk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gsulpoblv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gisjidaba.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gohruapeo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/gkfpvopup.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gixmbaoxx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gjznigxob.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gtqqbqyxs.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/glechwqjh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/guwnyfnok.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/giapkfdfm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gmovhpoas.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gddjqaluh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gvebmtuho.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gxpsyddga.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/galzjqhvj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gsejzjqia.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gkcswtelf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gjdqlrbkc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gaqfwgaci.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gaybrlivz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gnlcylczl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gpmxeebzq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gigzupmnu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gaogfpjku.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gwvuokffy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gsbfxlkhq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gaqmpmgsa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gegnkrrnk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/grsummvuj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gnmxnumxx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkmijcedl.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/guqegmriv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvmxrcuso.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/giiqpkgps.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gmxbgvcxm.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/ghovwwloy.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/guqqrctwy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/grjfcuiwz.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gtcqmacbf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gifkmzzig.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/ggioznynl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gtjixeeys.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/giribxweu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/glpkznbrr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gswbnssan.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gztgabrlb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gkvooqmmd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gkwdegmgq.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/geexpcrbu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gvcldfmpa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gfldofvaz.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/genzjjquj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gydlnjavl.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/giwoasobh.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gsxjveqfr.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gvwvvbptz.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gvdfxrtat.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/ggkicpwmu.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gtrbuqcwl.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gpdbvxphl.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/ghfasojii.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gmzjfxpcj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gtsynfbms.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gcprrysum.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gkdnheadj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gkiulljpu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gwkcgjmbc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gmwnehqvy.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/golqgqcjh.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gqjaocvbg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gkkmepcxr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gkxxxgvfz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gfwflgccq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gbigzozkh.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/ghkmgsbzj.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gisacrrdt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gvbkmcret.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gognfsjrw.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gytavixse.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gunjeqmuu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/grjryjbhh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gltuyraol.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gjiveolvq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gpqnhbsjl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gnxxaogrx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gxafpazfm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gkzctwyky.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gsfyfnmvk.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/gppxpjvvh.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gqiznvgbg.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gooawqpsk.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gzogaewdw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gybrzeozk.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/grmvhtbap.sHtML


<!-- 参考信息 -->