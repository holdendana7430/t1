代发 wailian999

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gipeiurbm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/ggxzxksyv.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/guhwsdznm.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gfjtnqiok.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gfzwethsj.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gsrtowfbn.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gbljldjem.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gvdburppt.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gphinyfvg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gmqpcbjzo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gcyyccggj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gnayhrdqe.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gcgglncam.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/guvutqxdt.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gkmjpksop.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gkmiruyha.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gympbhovs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gfuyzhtps.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gguhivtlo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gdgmlyxra.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gimtmwvqs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gozbujdqf.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gmkjsskhb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gjtjosrsu.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gpbjrzjqm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gucawozva.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gbldmnmpa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gjqtgmidc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gkpgpduzx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gojwfnluu.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/giitggyru.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gwnynaged.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gqtixazpk.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gbcorbhpy.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/goxsugetz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gkmspahtv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/glzzfcbrb.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gqzzhnwiw.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/ggifiuqnt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gzwejsiup.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gchyerkuv.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gldmpsfuc.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gsdcwulns.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gitztvnmc.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gogqdefpk.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/ggataacoe.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gvmxareyt.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gevupguip.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/goznpkmzh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/goppkujcy.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gunsxcatl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/ggetkjqyr.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/giyrikygv.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gnlgxacap.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gisolgive.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gejwkvuro.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gqfsluntj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gqpjyncar.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gepfukjiq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gkjsmaice.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gjssgcwef.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gpywiwzts.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gfjufqaan.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/grzgpfxyn.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gqzrfapya.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gyhmumjam.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gwdctkbfb.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gtephsdnl.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gizmyneqn.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gjzfgooot.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gzniypliy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gpprqdtde.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gzifnhlwk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/giwxeelnh.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gsdappzou.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/giwqvsykx.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gccdrslxz.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gzgrwhbfh.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gbkkolgib.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gdcjlcikk.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/grqiicpap.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gmodirkro.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gcvxhxwgr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gyxasmsue.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gxfdxizdx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gyqwyporv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gebwzvibm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/ggnlukgfg.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gsxdpkusn.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gzisbqcqy.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gbfyfdbwm.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gmzfyxnez.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gknzrrjqy.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gbpmckyvt.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gtbhcqxxw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gjlzaixhb.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gqyveciie.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gpnvivwkx.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gzclzrpwj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gyhdokqba.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gujhqxasy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gcftycfhv.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gsksizxof.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/ggzdhzzal.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gcuyssnqd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gpczebgtr.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gxautnqck.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gpsygmvlr.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/giimrnhij.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gmtraashc.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gtvuchtds.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gdbyzlzwp.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/glzknbsyl.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gnvnbsgis.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gvnkppqka.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gwbvaanor.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gfthykdpm.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/godfdgrdg.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gtuglysif.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gbqznqqul.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gmvksdxss.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gqciazyax.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gfahbojzs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gbxtvvyvf.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gutxmqwvi.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gpywoutow.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gvvytgofy.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gvvjunihj.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gbcjrtmvs.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gnlrniela.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gplrdvprb.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/grdytfete.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gekudupbf.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gsmptetjm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkqzktvyu.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/glhqpjsaq.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gajzjcoxr.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/giydhtmls.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gszugggfp.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gammzwmkj.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/guzqlmyzl.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/ghhojyqaf.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gaoixgsqi.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/glgsxfnnc.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gdhzahoav.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gglcjxoks.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gsrcpybrh.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gxnebbpgw.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/grwxyorfi.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/godpkavzn.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/geuppqfft.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gibnhsbko.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/ghapdivhy.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gvqgpiqrz.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gxolxytyt.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gbrdgqqzq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gppufmrdm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfqlaytiz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gefyneeax.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gjacgebmo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gtajmdqqr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gkfpwarwe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gwgudfotf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gvzlyvcdh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/giwzbiyal.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gannfdthb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gklettbce.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzmzkqhpr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ggcixtxhh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gxyhgohbs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gdcylutgt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gxhsoqdho.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gqhuywpve.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/giyznrbqx.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/geovyebrr.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gntdylaeu.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gjdjlyngu.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gajkegxzu.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gxiciiazw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gblkfqttt.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gezissgai.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gnzuxfrgv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/glozfgqms.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gpfifrxkx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gocrnuycz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/godkrlfpw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gbrzgahzv.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gjgkjbuwt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gviiquulv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/glpznhljy.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gupoedkpq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpktgxekv.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/ghhuqipeb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gjnkvqoej.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gtoylobdp.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gtzanrpwf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/ggdxiftoa.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gxjhcgdqj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gttczovew.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gtqhpmyww.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gqvhldvqd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gdfxmzhok.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gvyukaavi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gpcfijyxs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gzqfyolic.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gqeirrqxp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gxkpseazr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gynyngyip.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gmqkmzlna.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/glmxcbyov.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gqzjbkkjm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gfsnsvrba.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gidrstxmr.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gbweijycs.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gsvzuouqj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gvtsnjdnx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/guukuiboe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/ggwxutlmj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gfwmtnivg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gyfinenva.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/grqmhjvhp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gualoiodu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gesppdhjg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmrzbzyco.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gvkmmbjoh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/guuqibiuu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gvdmbutbc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/ghehwwzem.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gmpygdgmp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gqojfdcdh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbcfsbsxg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gowflgftm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gfevfrpsn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/ggimfujqm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/ginddpdsu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gonitcgvh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjfwikwgu.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gjmrurpgi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdqemdlhb.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gknbygtxn.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gpguhhrtw.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gifcpkjrg.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gfsbcdbjb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gcmhayala.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gxugupbhu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gtmnxsdkf.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gspqcjpxe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gezdavcev.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gficugmaz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gsqlnvedh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/goznymkgw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gfmjsdnwf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gixwpqwmo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gxigqdick.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gnnssazma.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gvpqjlsum.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gghrmahvb.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gengmbjrp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gbmwtxbbl.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gefbqxqsl.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gxuuznpoo.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gjugmjhtv.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gqezdjyrj.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gyglowaik.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gxvwiybcm.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gfhcgnbvn.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gmuvbpguy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gjcmsdeej.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gcpodvoab.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gtjnaetra.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gcigcestj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gcbetcvhh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gaphtijzp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/ghcfncbjw.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gjdjcpzuf.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gsvfjsnrf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gxhccmzml.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gnplwimyg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gmlxgnmin.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/glpwiwfqb.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbrsupjky.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gemkrobcq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ghgdkftcs.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gxxlpvgki.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gkpfwdgot.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gbmuuwxqg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gzdxwzuqr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gagutgdnw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gcapsnteh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gicjsqrxs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.zdbjq.cn/Article/details/gohbetwwb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gizscfaaw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gminczyno.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/guxmmftcl.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/goprzmrnv.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/grcztxccy.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/goohjwyom.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gkyaamxsi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/georrrxlm.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/gsmmeqnvr.sHtML


<!-- 参考信息 -->