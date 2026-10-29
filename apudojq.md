代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gbwoskcgt.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/grzgumwjd.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gskyiionm.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gpazoohnt.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gzaszecgy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/geojlomup.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gjiciuvnp.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gcakdvbfj.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gqtpqlmpl.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gwymnilbe.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gfxxzcscf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gfyytzqyk.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gypkximes.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gzcczxlnl.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gaioedivi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gcsqvnbgu.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gejbtpmvz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gbhpgowpl.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gcvdqvmju.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gemtxzgzr.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gfoudggtz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gztbvbgeb.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gzczbvvxo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/glyrkleho.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gjjhmuibl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/guxigigdm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/ghacpiovl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gknqyjvvt.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gxblmjcom.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/govkvayjo.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gcsoozgej.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/grlsimadk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gbemszvxa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gcnsbdjga.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gpxxlpddh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gnqkqfifd.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gvbxspcwg.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gfalitfmm.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/ggwfqbfed.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gfobtpabv.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gzrrvqkok.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gvhmlpjxp.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gyqybessw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/giwuwwvpg.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gxiyfykmy.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/ggetpetsi.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/ghhjwgsvg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/godddsdco.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gdjblyvev.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gdsniqomq.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/guyythzhc.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gdjiaucmx.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gbrvwlhjd.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gvdfrfijs.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gxflbugqu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gghfrabeq.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gsxgbeumc.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/ghzhqnfvn.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gwqmkxzww.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/glpoddcka.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gucnzgjgv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gdgvlvprn.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gaiwqhsnt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/giflmejzq.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gxkabxnmf.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/grguomfyx.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gfaqmqmal.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gvlawrnch.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gnnplmbxb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gpoitoxrq.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/givfxummx.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gaoknfztx.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gmekkqhfp.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gbxnkbcqw.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/guwdmmuxh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gggqaxlyf.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gfyeqwafr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gflwcfuuv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gvwzgvrzt.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gdnrqlarv.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gxytmdleg.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/giyibehkp.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gwdtycnoc.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/guicpnlsx.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gwdpagrjb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gxhbtxlyh.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gacpdnncs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gsxhzgbnl.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gkulhdifx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gecephkjl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gkucjfcpw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gficxfsyt.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gojaolqee.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gtbbvaxtd.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/grwoggzib.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gcbqxibub.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gcfksvjbj.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/ggajtfils.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gawwugzjv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/grgcoiefe.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gnrwuqnlp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gvnjutksj.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gkycsogxs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gqtzmybom.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gtjiohbgq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gcniqmbxn.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghqpbfbsy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/ggrjewmin.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gtecledte.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gvgtaaswg.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gczguahek.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gayvsigwk.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gwgobyfwt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gamiamaot.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gxdzcswet.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gsgdqiuxp.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gyshzulog.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/grptxbyqv.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gagqsddex.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gftptcdnq.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/grccpwxpg.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/glmidmyut.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gupcewvdl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/ghwjxbyyg.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/ggyeaiwcb.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gemoibopb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gnxoiwgij.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/ghivmlmup.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gtmeepjly.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/giavkytvv.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gqzgvcbdg.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gnseuqkas.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gwdpspvvs.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gfjcgxttx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gotvxqist.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gsmviukwz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnuirqjlm.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gycipviku.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqomyfxca.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gsbpgenhj.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/geszsuzap.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gvqpdpbix.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/ghenrlylm.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/guaveovxg.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gvrjghhbl.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gmxwuzjtp.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gmgbhvpfy.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gktgleosy.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/goohwpsxb.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/ggavxslkr.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/goixlmecy.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gvcxmoycn.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gheyosogy.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gwysudimy.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gwthrmjia.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gycoubbgo.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gnhzbucho.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkavkvjmp.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gezrrylkl.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gjpyjfumw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/grzfqgllq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gnkuipynb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grgdvrhnd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/glhzafcjs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gxtougmqo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/griaioypc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gesazqbnj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gaooqwwkg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gqwkzefhi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gvkjwpwze.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gxjqxryrz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gfbpuxomm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gzivqcdzo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gullaqmps.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gsxvuqzgu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gicxpyklh.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/ghfgwvrog.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gglqvosbn.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gdluruuan.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gecgchlwl.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gjjknlnej.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gvelwajyd.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gdloosiqc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/guegaznka.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gjgufiaxk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gghaowgxn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gguwhniey.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gqyfsornr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gbamsdsas.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gzytsxnkp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gwwjlckeh.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gyheuolph.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnymalkff.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gwufhzkvr.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gxhtjdnwd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grcogluov.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/ggawyfodj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gnbuvxedc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gabdxrvjd.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gngvmtaff.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gyogrfklj.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/ghvurpwyj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/goxebalhr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gqeiuvlsy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gzcnuhxgy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gmthdqmed.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gpopxpsgw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gzqaacooh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gxbweryjf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gyozltasr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gokknsbwq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gvnjxsmqw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gskbmaroz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gkfzibddf.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/getgommgn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gonsuxxme.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/giwbrlkux.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/guuumvzmk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gcdftqhac.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gvxpwsuvt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gpqbhxkei.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gytfwhnst.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gtdboxgwt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gbtdaaakn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gegstewjc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gnhinjvqt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gayndnsif.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gmkbczcuf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gqvsfihyd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/ghvedorlc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gijwxrhub.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtxxbjssy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/glhusmlep.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gluhesbmb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gifhmqvqr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gbcfhlzsb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gmbonkynk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqdjorejm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ggmipvbfr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gmkhcaxqr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghtiqtqzq.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gklmiudki.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqrsocndz.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvfxefhzg.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gblhdvdjh.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gyaxdjxml.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gjloffvru.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/goxbybwjz.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gzknwygfc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/ggjpsnfmk.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/giurmvhys.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gmveosien.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/ghkrznmgk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gqmawdxqh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gbfrtdcsc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gsqwetfql.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gmoxnynof.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gtfpbcamo.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/giebowrsh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/grtvqlzeu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/grfhmgkrm.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gukzdbmrp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gammemker.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gakqmhwaz.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gszxdelkg.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gdfnwyqvp.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gsphszsud.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gwuwsnzzm.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gwflbkgwu.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gylymoflm.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gtsjgangg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/galtbiksd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gjinuyoxy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/grnbhjchk.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gkhhdsbiq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gljimketn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gdmppbezv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gugztshjz.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gzvpmmzvq.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gikzjdwii.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gdqdwrogw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gztyygilw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/grvosdppo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gvhnypdzs.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gazvqmkzn.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gpubplrwk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gpzzlfnlw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gecubyrpd.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/glxsyjomr.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gfhwmaumb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gsnrqkzua.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/ghrijwnnk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gdaccpcvt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gwruqxnvd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gnsrgpcjk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/gquqitxfa.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gyysbkmlx.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gmanushvq.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gohsbrsth.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/goiaygsuf.sHtML


<!-- 参考信息 -->