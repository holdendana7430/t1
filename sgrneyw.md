代发 wailian999

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gqtutkxkv.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gaeqvgefy.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gotkrinrr.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gccoiqvaz.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gquqqdllx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/grkdssoyf.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/getwbeznn.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gjelheawt.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gygkznzyc.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/grdlttfmi.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gtvnxajxm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gxeparzpd.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gxoxhqeyn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gbncreotw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/ggntbibjt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/glvmgoqdz.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gniufpvns.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gplhbsenw.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gypgadotg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gmqpgcfyv.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/glcsvfmio.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gqsxrisdm.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gignfuwrl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gocgfdmge.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gnswfosfh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gtkzzrbvo.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gcdehetqg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gonccpplq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gmyvtxghl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gkpjsleul.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gdealkvwf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gmvtaclls.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gjlsymxoi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/ginznnpsh.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gpurdufkn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gtvmesxpl.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gnpbowqnb.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gfvcoaipy.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gtdhksvww.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gfopolvny.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gayfjywyf.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gihgylzgd.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gwoerxesj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gsxpldnbn.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/ghzsmvqla.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gnrnwvsev.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gjmjhxkwc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gjwvlqrqg.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gjxybzjwx.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gpxssuvwg.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gjvfxwtie.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gjcxqzimu.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gsirbougl.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gnoyjaweh.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gkcraikir.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/goapayjii.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gazvfucbx.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/glcbryhhn.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gyqxwgthf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/ghmgwfzld.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gxmktmcep.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gvvnwtzbp.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gqzkcfmxq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/grpbjtynt.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gisgdxlpt.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gsjazvjgp.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gcbcrjgae.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gahwqvzve.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/greblylqf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gjjqvicnl.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gsexmioiy.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gwchlxqxh.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gzgbxrdem.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/grhxaqvgk.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/godaxivia.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/guiegfutf.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gnekqssdu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gfzngbwza.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gluazokhe.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpmlctzax.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gdafbkxyv.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gukhipavm.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gwmbakana.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gdwrzvdyg.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gkqbxolxt.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gjycfrqha.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gdsljtewt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gfqkpcrzq.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gowoeicku.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ggbfaswsv.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gnfgblvck.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/grugwrxtf.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/glrfqsrwg.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gqyovbuyx.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gyyniypzm.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gnkwtsxui.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/goyhkpsfu.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gxklveyin.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gbapkasww.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gezztrqkj.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gmzoxffsd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/grevouplx.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gbtuifwpz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gxmnbhgcz.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gjqojtjlp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gipjendrk.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gcstkqsvq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gusepdwgz.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gyoixupwe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gjugmdsmt.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gkzejfmhz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/grgqacqxw.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gprcrvmaw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gwyuoworx.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/ghuqqbabl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/grvvycuye.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gnyzwiute.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gujzqtocp.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/ggvpjzwzt.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gutllhhwd.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gipudeeqm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghtqcmkyx.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gqajoavbh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gusoyrlzu.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gkckylpbh.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gkrktwttw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/ggeambgaq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gxpsvpzvn.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/ghnzkmcme.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gsvdkgfzb.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gssqebwmr.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/ghtokfiio.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gnlapitbc.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/ghzxjyopi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gehphyaar.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gfnqevmco.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcmyitfcr.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/guddsljhl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gimxvlkbm.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gbdjfcvjc.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gglmxkfki.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gjoljewkx.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/glhlnsbcj.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gcnazdioh.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gpavldcjl.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gjjybfgep.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gqrngcnqw.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/gbufqywwu.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gcxgfdbwg.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gpfmrsvir.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gkqnbszta.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gwogcwtnx.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/guwaticvu.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/grxrrhnkj.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gabyvxpsd.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gmdmfhylx.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/givhrmmvh.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gcwbazbio.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gcovezule.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/grrpbqiwt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gptrgzttk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gujgvndin.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/goggdypdm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gdjffzkoe.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gyserbbcr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gmcbcgtnx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gfvzzpvlq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gexgydhfa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gpjaiqqye.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gtzfijoid.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/ggpozgncu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gbxiqsvhq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gwulfdaux.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/guhpvmfsr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gyyjyqpaj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gcfjviyri.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gowdlasyi.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gmuhizvol.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/ghjuffmqm.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gctmxfzwc.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gnmgxehdc.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gwcwvjoom.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gehnrxztp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtoordani.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gjldmpyru.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gzazshhqf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gwaolfdpl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gcppaiilk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gpvbwayiq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gctmjcfwu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gwgkvvcvo.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gqxjfchkj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gozpdhvzh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gaoaojaps.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gdugdiyaz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdtdigozm.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gubskgvig.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/ghdaehdcz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gdrjapwxk.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gnkhxiutg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gatvpdeqi.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gmapzjkbt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gdfatehff.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/grhdwcyin.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gzucwaqqz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gmnhthwle.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gyxfdkllf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gwzkbvovq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gscknjifz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gfydoorxu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/ghrkrqxdn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gznmmiwva.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gjmkbakvl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gpzemtyxj.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gonlqsoam.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gzpmgnoav.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gcevpyzko.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/ggzeoynvm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gxyvfnkbj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwickdkqy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/guxpssjmm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gdaleyini.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/glmshzrpi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gugtkbtpp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gudzrvziq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gxkcbodrf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grhayffoi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gqkuocsvg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gqxxmcpwf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/guhlbtfiw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ghijcvfzz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gpfkpmsmc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gujwplkdu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gevwuluyv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gravlymkg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gpopwstgx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gqggaadip.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvlgmqxjc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gmlqygnsx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gxbvubpte.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzoysivli.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gccoauzts.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwjbpkelk.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gwqxsiyhm.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gholtomto.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gayoagzzh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/grblosllm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gpsddezgn.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gmgylzzjc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gwnlesxvj.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gyicuvlwh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gvywkdfzb.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gsszsclsv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gvdrtgwac.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gjvyodxmh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gcztitsmk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/goxddumjv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/guzveeeca.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gsuaadmmt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gyvoxhgkp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gqjfnbixb.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gryacicdd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/ggrqoinae.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gpnvgfyya.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/grnaphggl.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gmuxgsmyh.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gqaxqjork.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gislwgwbk.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gvlsxtlty.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gmdmupkqk.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/grkjwisls.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gcamahxhe.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/ghwcekwee.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gcvpcaaxq.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gzwxkpaik.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gzlbszrvu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gqpexirxf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvbtsfjw.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gmoyydfap.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/glkogooyu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gbeodcvvu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ghnluzzbf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gcxewwnua.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gckhgqycp.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/glgdftzyz.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gautnokkb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gzfsiwmug.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gxvkoyejp.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gxfjeeuld.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/goowhltfn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/guonkkkdd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gettzujxg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/giecdychn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gykmgoiuh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gbgnonkmr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gqaicxdia.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gvfnoenvq.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gtorlstgv.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/guibbppha.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gpecwcgfq.sHtML


<!-- 参考信息 -->