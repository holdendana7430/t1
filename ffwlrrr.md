代发 wailian999

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gskkgkxjr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gidbqiqbv.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/ggayhqwts.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gbvnhiizm.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gbpftxfog.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/ggxwgnldm.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/ghpcmdgbr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gfodthwnt.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gnnuvrwaz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gcolxpuay.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/goisdujlh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gimaxwbgj.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gyxkildvm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/geronciii.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gmtulybiu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gufyinrbe.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gjpzjqufx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/ghfpiukve.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gzzwmlkqn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gsksuethx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/guuwobvus.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gkipmyrdr.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gbsdtmmld.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/ggqwashtt.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gtttumkzm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gaqffdlxp.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gaynwltrk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gkqnwtlyd.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/ghsutqapz.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gxbkwlzgn.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gjwhlteim.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gzbfgioyz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gaqhkghqc.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gyuddnfig.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gpleguldj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gpzvfgyyl.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gdpaelxsw.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/golitfeut.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gewuzisen.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gafmhknzw.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gnesamfki.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gbtfdxrfl.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gtafltxwa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gpeorhbjk.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gfxvvrkvy.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gsdmmqkkd.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gyiogyvmb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gqpcazvrf.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gggjvwmzw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gahybgeck.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/geszbkwwu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gizmefnsr.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gonwovuuu.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/ggdubidjl.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gezwwvbov.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/govpqjrzj.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gleoybitw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gezcahfsm.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/ghrqyaefo.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gmzrpczsv.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gdjvdwdwe.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gcanyyzxr.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/ggiozvalm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gfzoszmwn.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/ghchnujzu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gsnvakbje.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gyzkdijre.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gdqukkbie.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gxpwqnjgo.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/guunjzvan.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gdnbnwnpi.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gjsahxswd.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gawdhlcmw.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gjjttjcsw.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gqnngrnbf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gjhawvwgy.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gvkfyavoq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gxplhutbs.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gntgxatqc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gausyfsdy.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/goleldkdz.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gqlwrbuis.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gzfgeroyr.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/goeigalcn.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gsmldsxox.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/grfpwcufl.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gwjknwkjv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gtvxhltcq.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gbnxxalcb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/guukkzgqg.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gujoisgbo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gytvtojql.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gldafgvtg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/ghljkwpvu.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/geftzqkvs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gggwaozur.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/guzynkqck.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gyshtxcmq.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/geuoyxvfk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gsxgluayk.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/grrjvxhrb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gdrvxhbsh.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gqqcuvayp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gsuzrfvxg.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gwebuwogd.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gbuwksrsy.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gkfctpvyf.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gtbxxrhlo.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gloqjwmoh.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gbflclsul.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gnxzjedvu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gafhaorkf.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gzxxgpelg.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gohlyxsij.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/goqmovkvt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gvpbtdiqg.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gyzxcgbgo.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/glsjhbaka.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gmvacaxoj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gyznmgfgq.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/giqdfnhvz.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/ghtcerqnx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gsiqewoiz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gqrpgplbx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gniqzyffd.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gjkworkdb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcumjllrp.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gbwwmynew.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gdouljekd.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/grskibhgm.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gtlkgfybo.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/grdznwhdp.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gaudxyply.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gpfnqsbjw.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gxhqrqbwh.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gcnxaovxr.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gphlqnzsk.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gvdawaoni.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gsdfyckzq.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gzrkbqjzs.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gsieobifz.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gealcofdl.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gcbwmvwsi.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/godfbhnnk.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gyljyetpw.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gctqvmunt.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gxmitvzdq.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gxwyjcqvj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/givcxtsfk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gesrhdidk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gkecisalz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gbglvxypg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gtcyfilyp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/guuqmgrom.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gjfqtrwly.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gwiqhrtha.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gtpcymeiu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gnyfehbat.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gekxochkj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gdqiqnsht.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gchinptzf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gicibrqqh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gkahaimcl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gotjadsgs.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gugkrdyed.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gwcfhvqee.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gtyhzarkr.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gkaahxhtd.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gyvgmdppt.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gsqgkfwdy.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gjcmmzpqg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gmpisjhtf.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gghirtlwd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gwpanvqpd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gpumrmrjl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gvknfhbcv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/giiilwpae.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gdicoajcq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gkuzxhmdh.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gtnfeqymz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guiwqyrcr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gyjrufvif.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gwhbktvll.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpattcspz.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/grphlgrdq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gockkzudj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/ghtbjcswj.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gblqtnsme.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gtxfkzieh.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gxbrfhedv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gyoojqsam.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gpcbakccg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gbcabgfvs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gvajenxai.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gzalrecuc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gphcsbami.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gzhzmouns.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gnfntvmxa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gnwectchv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/galuqlswa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gthlbcqyv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gvlustmxx.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gnrspzylh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gbpcgzltm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gisbqkead.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gorcyajhs.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gknybjiav.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gtftdxgua.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/giaudeilt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ghvtzanuj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gvfbrhzig.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gufwnioqj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gukysbgyg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gpuilrqvy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gubuyedrk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gqweqlaxx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gcneayrwu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gcnssszsu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gzqnoxdot.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gomrcpjuz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gneyvwsdf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gmfetiavt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/ghfdgjlfa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/grgmvxsql.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/geywkjdib.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/ganwoaesr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/giaztvedg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzvdgxbjb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/garxzoplh.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gxjouoswn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbqfjrmbc.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gmntwhmpp.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/grhreqsmu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gwmmdpyit.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gehxzzgxn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gnemjxykj.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gjtmszpao.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/ggioxeyeg.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gaeinwpbd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/ggbuuhcji.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gcsyeaarw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gibqyqpmg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gwufpciub.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gdvrgnjnn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gxztclitc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gkusnjbvu.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gdsutahuw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gvhwjfdhl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gffbfdita.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/ghlawiyqn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/ggolatbpl.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjyysqtoj.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ghomhlkda.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gzgvkrbbs.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gtyubzwnb.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gdomhfrrr.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gayzklopd.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/goauzqbyg.sHtML

[A04] 判断变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtszchmnk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gddakhxwm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gbqefktbw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/godwenurr.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/ggbxzmoio.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gsnohiber.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gkxoskquu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gvikqojbr.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/ghlolhrrn.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gjrjibwhq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/guvvqysgb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/ggkajetub.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gouszaxwk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gmbxxxufr.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gaxltiqul.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gwtogisyh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/ghkcrgoim.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gnpflckbg.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/glgvstnzn.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gtpeijcgk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/ggqrzirdo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gzzlonipv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/glvodloub.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gbbnwqqvk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/gzttegjrz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gctfnnmkd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gsbyorjja.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gvagnnblu.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gigjpxzht.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/guwwlkxah.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gamiwkkhb.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gmbkofsbm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gzgsxnoxe.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/gyrhxreus.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/gsgtqnjfv.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gfilipyao.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/ghdalkwat.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ggjmurjrd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/guccpznjl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/glvravqyg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gvhkfjown.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gbvhwcvdk.sHtML


<!-- 参考信息 -->