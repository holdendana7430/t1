代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gnsrxwmty.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gfjgfsott.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gtvsydmfm.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gjklixkku.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gdjeksuly.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gtbowctep.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/goylpgzoh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gbujwolen.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gjexbpxgz.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gwknqmmxe.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gleuldtzp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gmgjybfvc.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/ggvlsfalo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gdrhmcbrl.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gjurftsbk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gkagpqghc.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gnyvazkrz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/grypcivcp.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/galkjwfsx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gxgeyhdvz.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gdnhylcpz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gsphkqahj.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbqasdoph.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gucypvryl.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gfoewsyac.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gsjrcvfxc.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gmhbqwbat.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/grhxrraja.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gnjgwvgdf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gsejhdcro.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gukgybpel.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/grwscnvld.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gpjdupxtr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gqrenffur.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gdzegdozm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/ggjzmzwue.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gbbonblob.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gqrsmobpo.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gvxazaofn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gxietgunu.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gvgldusha.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gmspjsrcc.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gfytjyrpa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/goooqalmz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gvqeavzeu.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gcyjvplpn.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gseriwkzj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gnaiwznob.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/glvyotfxg.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gcgmdcwfa.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gdqjnppia.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gjjujgpbn.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gxkprwxwu.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gcijufxma.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gbkbjqeaq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gmetajngz.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gtfrcljre.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gltalclps.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gepxhbgjd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gdjmywzkl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gmgztsvxd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gywjxhzuw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/glwjuoyhj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gzkycpogb.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gwgqykhwu.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gsfroqmxq.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gmqcrxkcg.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gafbxiibz.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gpkizeatu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/ggtecqvwh.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/grrzvqiij.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gwkbdvzdb.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gffnhsvfn.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gnfgkzqhl.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gndghnjcl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpupoioup.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gjkvjokvm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gvrylvaec.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gjqhaqzih.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gjjujpjsx.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gugwszoxu.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gdhopxjaz.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gcyntfkqb.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gbtcdeuqc.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gotursuvh.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gxuykmati.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gzbikrckw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ghyjupmsk.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gdrpuiric.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/glbtcvkgf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gzqkdzaxg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gcdynuojt.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gktvfijgi.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gmfpywxhh.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gnbfzqpxw.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/glgchizzs.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gdynhfyel.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/grhefnyiz.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gxfiphicc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gwfopelks.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/glsqoypde.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gckqhlclq.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gprumnpct.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/ggtzlddju.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/ghomxegzo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gijqtksvz.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ggkmrewce.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gxzeweooy.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gatdqzzkf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gutqutgpj.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gkpglehqp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gsirgnvnn.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/glmwtsfcn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/ghcsiiutg.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gvnxhshho.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gvkrjfikp.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/ggqyntqpn.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gvlaybphw.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gjgjuxsje.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gcrlaxxhb.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gfocdbcbu.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gzxuqmfse.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gkalmvaci.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gpwroldmm.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gfjebcjpe.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gihnnwtij.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gosriefas.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gqfedxzcp.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gtpvvngbg.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/geqfovmtc.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gqlvrqivc.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gjsswpovr.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gwzplavet.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gytqayjjc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gfycdnziv.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gpykxgpwf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gohttgnve.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gtwdqtxqd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwszkbbok.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gtcyuqzsi.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/ggsmrkeld.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gzdqiucgc.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gqwfzhedf.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gmrpimpks.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gkefyzbiv.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gdbcdgkqs.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gmqwtiprs.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gscnjstba.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gmhsbzgfa.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gpepwaybo.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gvgaluaxx.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/grvczyrmr.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gohkbhxvc.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gohgusoje.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gihbrgnxl.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gabsjgtau.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gczqzjlxg.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gadbwlerj.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/ghbhyzujk.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gsnuhokwe.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gwabznwds.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gkygxzcde.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gqweeniya.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/ghbmfllnq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gbbtafrfz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gxepfhlap.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gcaujiytm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gvorvfyqx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/grbezqhzg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/glcvzzfem.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/glftxhxyj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gzcshgdhh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/ghoqzannr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gwnlrczll.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gnkqonxme.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gablcszlh.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/ggpwoeems.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gyribbaog.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gkbybxkwn.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/ghrmwuquk.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gtxkfhykd.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/ghkvldaoa.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gsczdntzg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gkczfhjnj.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gsqlcofsu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gtjywiect.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gkkshuiik.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gudzinojs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gxyyawrri.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gebubfien.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gganeglgo.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gflaoazku.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glbcaffpb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gsdtokubt.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gvrunenlm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giyayllwc.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gdhrwhrgg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gfjocyihu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gbcnpolzc.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/ggwuuvejg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gmnorzitk.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/greljyfld.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gfdejssrp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gitamxrvw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gwdrbsbir.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gdwflulba.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/grjujamsk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gifooigef.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gacwdtikh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gdpuvjtjd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gmkhnppjo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gdgwyuogr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gnmsdbgbc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gdhqjinpz.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gocctuvpl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gsnaojmrw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gdaggouxs.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gxiyvnvze.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gtymetwar.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gdwbiuhdx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gstrlwlox.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gjaktcqxx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/glliiqtpt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/griixwvaw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvfvxqitd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gdmzzynrm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gcmmwiahh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gdgubkzgr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/giyoycwiq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gdzhotykg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gexnbsmju.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/grtyhyduq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gxrqvhefp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gsiogrqdz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gbctxokrt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gonunouhl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gwwnbgcpi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gevmoqjvz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gtibnmfzu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/ghszevyak.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gewamxcrk.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gyxajildy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giscyikkc.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/guytxjxkd.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gslwtgpcb.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gdkciibdi.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gqpnsifve.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/glqxbiivf.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gkflczzhw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gtwsiljhl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gkptqeyie.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gzphodymi.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gnzrdlrdt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gepnbvvqm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gnrcontjg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gfzksmluv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gizfstcmk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/guxyunrjt.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/geeyspibd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/glmrcvhne.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gogfegkzr.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gaeppxomk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gfiaqdcdv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gvhogchli.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gfwyfxvwl.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gdsljhnhm.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glxmgbpkn.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gvuahkpdk.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gmoyzncqy.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gwdvmqpbl.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/goicknjzz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gcyqoqxqb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gtlxnxtay.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/grzmiueku.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gigujkdke.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gviofxuuk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gxnzneoio.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyuiphff.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gbabiyafk.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gnkjbayzi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gcdfjbkgl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gajesdecp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gfmgvndbj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gvlgsyxrt.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gtgmhuebv.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/grmmvxxmb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gwwwyttzz.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gzmwcefda.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gquyfjiej.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gvscharzp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gthmtnpim.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gezexcjji.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gnrghkvut.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gefcwqjvg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.zdbjq.cn/Article/details/gbypaeuzv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gnpbzlbun.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gmffouemy.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/guwnjzfze.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/gajsuhbwa.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/ghhfthviy.sHtML


<!-- 参考信息 -->