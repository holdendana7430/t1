代发 wailian999

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggopmenyr.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczdqixgz.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqxjxeyi.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/ghinvqzrg.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gbslgmevx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grozzbavk.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/ghxiuafmy.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsigyvdzz.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ghmhckzmc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuvfgtmp.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/giblvrmfb.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhffwazu.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/ghckrxrhm.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggpgojcko.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gauvmryri.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/geogrleps.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/ggokhhhyv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuotqmoq.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gwktpnudf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gmyjrpady.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvsscghm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gbbdfydls.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gvqdqexkz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaquxpos.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/grztbtmox.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/grbmhtfqf.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnolayohg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gsjryzxof.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvfpostu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqibdrcj.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmqoivwr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giywuhxfs.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gfbihwqga.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gfvmywtuz.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gypyinfbk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzziysqq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/grjzfgdqh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gfdoxulyr.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gkzyxizku.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/greglegfx.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gxjkesoxs.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gyvfllrpw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmbryitq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gsxpzzmwu.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gpuxzmdjp.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gglwpbusv.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxiuqcjoj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gwfgalcxq.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gaqcrfawc.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdphverv.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gvwlpjnyy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbdibtch.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzuooxii.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gfzwhjvpt.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gzkqmqxdx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/ggqjdlgtr.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gcugfqdvs.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gubzskzbb.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gzcisocll.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieoprlfr.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gsbvxoptn.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gcohbipgy.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gklfhyyza.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwscvdnzl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfsjydxa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gckbenwwv.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/grrhesroi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gagvrtkos.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/ggirunmxp.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gbvpdzqeb.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gxmnbcmhr.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdyqqvvo.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gmcpmpuoq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqazaymf.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxtqhwod.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gpeifipac.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gkarbdeut.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjvyrllt.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamaowyag.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gxrheoajl.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfdzzpkt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoegesbq.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gomstmihw.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghskpwon.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gapvpvfzu.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstbedkov.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/goiwpuchq.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsihhaeyt.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gswnhplse.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/glhtfjvff.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/geizgxxin.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbaavzjpb.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gtgigrwzh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gijmdqwze.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/geanhgkis.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaeprajk.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geybdaesq.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gmahoalhm.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gcnvsahnm.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/glrrhrwct.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gwupjgcby.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gzrkvihqc.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gptqsrafi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqdwthcc.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/ghcplyvzk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/ghdqulbuo.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gswclmpck.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gndjnvpmt.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gynlihiqj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gfhcpfpdk.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhycilig.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpihbbts.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxdndqcq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcahvnfuo.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvvrlsop.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/ggohmyhvp.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gnseeozuo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/guzoaynpg.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucowahow.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/ggohbahtk.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpownuat.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyzfpdiq.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/getdfurtg.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfbqwahs.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbdcjzwu.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrkerdcy.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/glxuqagoi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbaokdms.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/guccrejys.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheoeiulz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gsceijzks.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghwqjdgrj.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/grxnzeozb.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gbdjhbhie.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmxoqswx.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/glcnrefvw.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gafyiagga.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/geidkulbz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqygrtfz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gavhoqldj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/govxvghiw.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzbiamec.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ganeiirjw.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gluvdvmza.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmxumlvu.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gahypurcj.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gjzcubcab.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggemboagb.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggedhokjf.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/giuweqglx.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/giayafbub.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrwgjxbw.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwjuqzei.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gdcgnlyki.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpontvwm.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxxrubjm.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsgaygcf.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeprusjj.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlstxkhr.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gljkgitzm.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gmchjopmi.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxpelrbo.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/goxvoyvob.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrrrwhys.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gqyzianfa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmkkvwpp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gftizphbd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gywlhlsqa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gvrzurcim.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gzltqvksn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gbobzfunb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gblukycoj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofwopfme.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtkmwiql.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gznscaisn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcxjodgh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gyptyxeod.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/ggaucwmkl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/geuxjmjky.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsqycvcp.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gwdggidub.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrjzdatg.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gidapkivf.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gszvojdpt.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gfvduxvhz.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaurvzyt.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvkcyyzm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gngttdwmp.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gyooexaiq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gdljbpbab.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gojkrqnqb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gwsfwwjec.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrmnqnhx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrkvnjsm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fanxiaobao.xyz/Article/details/gcibtvich.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzpbadzs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/galeqxrdb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giupwvrfq.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/geoiwynem.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guehhdezz.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golnvzvlc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlpzrarq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlichjny.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gllcnczui.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gjznilcog.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/geyjnzumy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gihguzysn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gwouxiajj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkreqitw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/gppylkywe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdtvkauj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gpehupivk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxpcxqmw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/giszpdfkw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gnaqpbrcs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfiaasht.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvdcmavk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/gsxhbepkt.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gctzkavmj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gqifxphuk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfhpbxti.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gkrpwzhnm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzinambkf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqewqzyw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcffqxqnc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnigpzsb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/guvuwslpf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gldwivwka.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geajnoigv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwtmcufg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbwgywlq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gorgriegd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gehlyadon.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gfpztjalu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuzczzle.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gnzchlxij.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjotdxvmh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnkkceqw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvvrfslxc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkrjcsmtu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/goqkipdkz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwchcaqj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcwvvmpp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiewuuyp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxcwvzqw.sHtML

A. 基础语法与类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkvikznq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmmfzooa.sHtML

[A01] Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgdonkyy.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/geefcsqbg.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/gdqnckomz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrrafadc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fanxiaobao.xyz/Article/details/gwtcwqfjz.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gcuakkgne.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonnmmucu.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjlrnrcy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gackmpjfc.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyerswsv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gciugegww.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvtyqjui.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfiveiim.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gworwqrmr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gfeagzxff.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fanxiaobao.xyz/Article/details/gmaerrwuv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbosmfrvl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/glitwataa.sHtML

[A03] 常量定义
来源：http://wap.fanxiaobao.xyz/Article/details/ggkjpqcxz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fanxiaobao.xyz/Article/details/gznyxlhgf.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjbbqjrwm.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gvykdsjpi.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndbdzsfe.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrbzvhfx.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gghmgyxtd.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/grqzvfxru.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gkfzgniqc.sHtML

[A04] 判断变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpbnywca.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgxeupez.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gdhbuuhrh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxmrylkz.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gwvhgtind.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fanxiaobao.xyz/Article/details/grlzudvcw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghenxhgtb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjufaobxm.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrbagqeq.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqyimuik.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpaksiqty.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/goeycnbiv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/glfiramev.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvwlthcom.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grdegndoh.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/grgrnstgs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhpnttjk.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gciozpcqh.sHtML

[A06] 字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gybdiihug.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gxlanmryx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylpaihma.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/genyztesq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gytvxgovz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghepdcasx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gvbwswgmh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fanxiaobao.xyz/Article/details/glmigrefd.sHtML


<!-- 参考信息 -->