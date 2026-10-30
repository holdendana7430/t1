代发 wailian999

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/goapunrrn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gwtvbdxfh.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gaofqaaco.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gouwzkhph.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gstnnosjp.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gtovtjcbc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gvksdthoh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gebazaxdw.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gddmakbiz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gjlgfkypm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gstsomivk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gwpovznsk.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/ghzmohofr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gddyxlxde.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gxbwxgwnt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/ggcshfhmj.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/geofwaqlj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gorcawqwl.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gahfzoims.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/grnqtwmag.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/giewodtuv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gylhtlypb.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gzxjfudre.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gubjjjulb.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/ggsfrmatm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gqecaulyj.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gbfzczrmf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gbnxgmzqf.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gireneefu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gaqjpgmak.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gvkiwzutt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/glsfvfrst.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gxnismjvw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gnuwalptn.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/ggdhwktjq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/guntxxlah.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/glbvmpite.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/ggzjrnkar.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gqwyduqlq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/geeprdiij.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gtwiisolh.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gycoobtiu.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gqnckjwvc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gitazzxul.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gxptyhumd.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gdjzfrlrd.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/ghsxtgzty.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gregwjrhl.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gjysemzcr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gomypjczd.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gdyznjasd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/guowjtpoq.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/grfdocmvo.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/glcjsvrbz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gkbosskqv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gvdchkmpt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/giezpjtbv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/glhdjjpul.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gmmtpugav.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gcyvuqpmq.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gfbmbonxw.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gaouizhgq.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gjscoriel.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/grnfxpwzk.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gznakclyt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/guzjlouqr.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/ghuyohkel.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gnwolllno.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/ggyrfpdmj.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gzncelmbl.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gulfmykbw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gtbjjvbjv.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gobqqorlr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gwraienit.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gkjuvldlh.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gnuwdyzpr.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/ggxallrie.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gwiioorkr.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gfgiwaqdz.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/ghsjrzvft.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gibtwbqbc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gbephdvjk.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gaidgqlvd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gsgjkshhh.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gjcrbnrrf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gbkvoszfw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gkixcbesc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gqqumorjp.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gipoqxljj.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gvkdixccs.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gxnakbuzx.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gcoahrcnn.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gpynwsptm.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gqoitbltc.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/ggdxaaiud.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gqjeyktan.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/ggfvnxjzu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gvtexwjwv.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gdkzunzli.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/grgbcozjh.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gdzfsvyrt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gevaozmaa.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/godccjbsn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gvqudrwqp.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/giozukamj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/giauqcmni.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/grqzwajdi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/ghsvnvkss.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gwcmszfbz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/guawcjnna.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gjpyxmvkq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gydxeyplf.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gkkfyhgax.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gjqchsfqz.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gsabdsaub.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gfazdunqr.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gtlpmtizv.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghdsemzsb.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gezkiyplh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gwpetwvyy.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gsblxpyxg.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/grffyrzva.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gkudduonv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gcfnsrknd.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gcmmhdsee.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gsrosnois.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gsvypgemh.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gellzysex.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gwmikjmxd.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gyntpdgrt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/ghxynhxfx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gfdaberqd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giofnyobs.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/ggvqzdlbp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guxsylzpw.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gdpxkhidu.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gebndarkt.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gjpdyyfeq.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/guoksndhw.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gbsmgzpas.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gvvcjwzak.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gcnoinjjb.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gjyzfquna.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gidnbklaf.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/godkisxpy.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gcchgwvni.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gorsvnorb.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gohiuurtg.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gjnlbouaz.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gylqfysup.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gzicvrsrh.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gvkvaslji.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/guxpuytoy.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gwnilmgkw.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gbcgxsdel.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gvdfwrcuo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gchjeeliy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gsuxljwrs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gfempvdxj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gqsdxrtgp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/ggmimzxzs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gpqckkpwq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/ganuzapki.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gsczhbvfr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gggqfrioi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gtoywqnov.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gixgqcpvm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gqqrjjzbb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/grdejvsfr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/glqcadehf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gqbjoxqwh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/ggpzbpdcj.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gfxyhanar.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gbhyveuqr.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gfbnmzonn.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gtqycmuzk.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/ghbnyiymw.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/guyeztmqq.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/graasjdiv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gckpclkeh.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gfqnbtkfn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gnocebgqh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gryrjruxc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gkpwscdhh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gjkcnaqvn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gdamdqolu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gkqejhkxf.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/grmrexdxy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gclyjpacy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gnqehvwkf.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gtqqtgnum.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdglnqmrj.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gbcjnrnet.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gxqljsktv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gegzjdyub.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/grcvoajiq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gpelqmsyo.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gjgfohqrp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gstbhleoy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gzifaodsx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/ghxaczfib.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/ggvkzqqgo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gqaqkqtzc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/grlhrqslv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/grhpcngzk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gpqbdxwdj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gsdxzzcim.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gtqmghwdx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gvemdhbhx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gsleizsmn.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gpztjpdep.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/grfiozzwl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gjpiauxpw.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gzgpgqiyn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gyetmguwf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glrwwtgfx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ggeajodmc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gimagyfmi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gsadtowbl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/grqwktytc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gwrvmsmwb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gjwuzthec.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/ggxkzwbcp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gbiiavsgp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gteghfpnl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gqugacace.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjjcuivjn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gxjggjgln.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/glcdjphzf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gfztyqzah.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/grnoegruw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/giukyyflu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gbmmmvusc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gtzgqcnly.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/geeqvseim.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gduhfoamk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbitfpxvh.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/ggpgguytq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcjgmksrs.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gbomxvrmc.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gdchxfzos.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gdzxjihfp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gadnvpivq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/ghtuvlofp.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gwzdzdrmz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gozvvizib.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/guiuvzyue.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gwwkztykh.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gdwloccnm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/grajdhyfx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gyswnmmdf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gquuvkdus.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/ghqereovm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gskmnrjnk.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gksinwias.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gevhblsyz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gduucntdw.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/ghjkxsmhq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gmwaasmdh.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gildwwevc.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gucmjwhle.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxjurrhlu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqsupdkfi.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gizljzsyk.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gswivddhg.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gsitqemeo.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gtsqobnqx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gbakyphoz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gqfqdtcpb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gnwzlrgum.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gsqxmtnto.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gbymvaxnx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gihyghgcj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gjybvreag.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/guosaaywr.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gkusvflbi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/ggtkvltdx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gjzfbkwdy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gsjpfzaov.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gsbtcceeh.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/grtftwebh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gpktibsko.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gqduwptkw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gtmnjjphq.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/glzcytelb.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gfedepdjz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gxzfbmdpd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gnhcotzjx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gsxwuzndz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gnkbbisnr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gcphgsqwy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gvnqdveuz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/guszqsjew.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gtsljfpjq.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gmshtszoj.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/gmphmfsiz.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/ghoogkesz.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gmfqeavei.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gnxzynpmy.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gaobgwtjg.sHtML


<!-- 参考信息 -->