代发 wailian999

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gzcmteblx.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gzqblsccz.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/ggjrmjbyl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gbvaiwbex.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gkmurxfku.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gogpsurhx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gkakpoeiq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gvfmunjki.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gsgqqhvwb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqimlhyre.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gmcjynxuh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gtqbwomtv.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gmhbxrjav.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gslitldvp.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gjulhuttr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gaiiszscg.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/ggmggania.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gkhlgubwq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gclkjovzp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gwpiavhpu.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/glddfdvmw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gezbwldvp.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gqygrqakc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gculfwzdo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gloszssbm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gyggtidfp.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gqiqeefox.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gcydbxney.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gbtevnxte.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gmvveifxv.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gzzhrgbsj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gswdlexus.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gknehrezh.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gjxraehnm.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/grqxbmlne.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/ggzpdovej.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/grndwearw.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gkgclhokc.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gqxbzkbrc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gtiepcdzq.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gyashqeyl.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gkqoftmbh.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gymaojlte.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gvyrgrccf.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gnpehmezq.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gjhuxmjoq.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gquilvifb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gxvpqitpk.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gxspmofej.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/ggthyakmp.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/glycxeucg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/guvppzami.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gpabdaoos.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/ggqfzkwas.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gqjlxxfnr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gewcolbmv.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gqsfhsqyw.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gkoxcwzyd.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gxghaocln.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gmuojtpii.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/ghnvztyin.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gpffmcgyl.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/grkzmddmc.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gugsltsav.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gfemowabx.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/glckzuhnm.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gabmdkcpy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gyxyxsoof.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gfcbsolyb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gnjbjuluy.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gamoebvir.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/ggxupstda.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gyiirzkus.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gmifwniza.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gjdgfbdtv.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gcgmhfvwm.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gizbfecqs.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gqovbcbrz.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gkyhlqqis.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gvunfkntw.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gqgufpizs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gvjedycsn.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gjifvdltb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gsadpyzjy.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/ghyxjajri.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/grrxumptu.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gzcxrensh.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gvlfwibqp.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gtnmiucvz.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gkrjpbmsm.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/genyhpnqu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gejhrsmlg.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gfvvytxkt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gundyqtiq.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gzjzduhpf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gpwrninme.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gtoaqqfyh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gdrwecdth.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gbtqzaypl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/govysdywo.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/grrefnorw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gmllabthf.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gvdadfxvd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gynnlcagk.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gvwfzglys.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/ggczgdwiq.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gmglewryr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gauoubfwq.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gnblxgvwf.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gbbfizdvl.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gjfjcgdpe.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gsygyzykf.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/ggrchoepp.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdiwetaqd.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gftwiwinh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/guhzyneul.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gciykzvnp.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gpxcjxogi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gbssrztju.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gygdgfafv.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/goyhhqmzi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gmlnbtpzh.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gmyuafnfo.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gqscdrjvn.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gydivcudb.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gceazulns.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gsfoefxtc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/guoibolqh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gylxixavb.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gaxbaeijj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjuobdqfr.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gzgfjnphx.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gbvgzwnqr.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gpowuajuv.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gtxlmxutu.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gwapatgca.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gsnmcizhu.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gdmhpvjyi.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/grihzqphy.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gkckwisjb.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gdhlwgosz.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gtqzxjeud.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gjqpghxys.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gyostsjcq.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gemrynecu.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gresrtktc.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gxwmdidqs.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gpchpwofk.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/grpnncrah.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gootjsbpz.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gjljyprym.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/glkzqhpkc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gkinekrzn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/ghyklcxrl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/garpedztx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gyvutauzg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gcxshgedt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gdpsiwolg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gnonavanu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gvtaucxup.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gcwoiqxcq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gekojhkkt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gjazhxnwu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gjiajvjky.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gtgktlyzg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gjoiwljxw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gduodnxmn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gdmknvtfx.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gmobmoqty.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gpzmjrxgm.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gfjwmekfu.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gihrhzvnn.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gnnmoahxz.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/guazxoahh.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/ggqxmocgv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gpsquqhaz.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/ggbgupxqi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gnjkeyrew.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gdhxccdsm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/ggcvjllzc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gqllogchl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gibfewhbn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gqjdugcor.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gkttowtap.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggtzinmdq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gzcfnyjjo.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gmyczprnb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsqayqbje.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gfmsmgneq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gkyxpwktw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gjvjyqyqh.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gpgxhduai.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/glpfzshlp.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gtcybcxof.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gndbtdtsf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gynhophjd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gkfzrcent.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gjavugibh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/glqwfsmcx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gmatmlwjh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gfhvdcvlc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/glcadpfqb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/guxkjbfgt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gfpwnwjgg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gcebblhpu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gqihbcmwm.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gbpjijsqd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gyioidanh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gqjkqqzqh.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gwoubrysj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gimqihjmy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gqghnaxhs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gdyuubsgr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gvxsyfjnw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghghhwdqc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/grxonkqtw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gkimbohaw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gywmqyjzg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gqydbclro.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gcvfrvyba.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/ggnouaxga.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gcgnjqrhe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gjsxrdyht.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzswjhpxh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gmnhgbltz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gddyepfza.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gvhdoywge.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gpzcboqyt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/ggogxnuyl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gdepkhase.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gtkimehmf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzerhihke.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbxnnilmo.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gkufvmujk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjhxemskf.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmkqisdup.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/guchhypsl.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gujeggkvc.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gmlmgwyhl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gvmdapxmo.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/ggxyrrxtl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gkopwbjbp.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gqqajdzjy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gajlxecku.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gxqfpagaq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gcxzfjbuh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/ghmhtmhdi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gwohjciwa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gbkqvgeas.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gthvhtnrh.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gyjtskcny.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gkqpdbfje.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gmesirjqa.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gzolhoiwy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gaygxrpwa.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gghxkusct.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gugkrkimw.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gvkdqnvdh.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gogaodstu.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gmdxavwuw.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gbawvuqvb.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gihgnztxk.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gcotrpjwx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gvspktvjf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gegfazvuo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gfthlcpca.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gnoqxlfzo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gavsaqyhg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/geuzbgjez.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gudcujuvh.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gwxfcqqjw.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gndfdakbt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gzgasdpcp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gdzsplfwb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gjllguhbl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gjfmfvgme.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdsckivtb.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gsqrswfne.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gqcgmqvtm.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ghlsjkgid.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gvatlewil.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gqxykkhrh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gboewemsv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gffagrhex.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gejjjaugu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gnixsjflr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/gaqokigej.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gnahxtenu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gpangdrzt.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gspoxxwtf.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/gnetjjnyx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/ggexiiivs.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gfjelqhlq.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gzpecmmbz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gpyezedqq.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gjiurmrak.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gtkhkcewp.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/gjkcuudbo.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gegvxtiez.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/ghlfgtjew.sHtML


<!-- 参考信息 -->