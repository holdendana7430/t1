代发 wailian999

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gnrkczqrk.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/grhmectsz.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkymvgvfg.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/guxtmrjsv.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gggttwdqo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxerpgmxw.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gybrtbahc.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gekpmdvta.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gdalavyuv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/geifflvjw.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqewxhguh.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/grkbnvniu.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqxuxajd.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbhefabrw.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbwqwhjn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/glphpkxgx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/grghorpmv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmrdcvxs.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gaggdgkuu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gometwgwm.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/glrlijzgj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjlkkbdv.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwmyacfl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqpwuvnt.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gwekbntwx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyxiotrm.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/glingxcpd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/ggnswhiau.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gclshvcfe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmnuevina.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gwzvnermt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gbqtyaxvh.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjuwrixl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gznfujybc.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhhyyvfs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbgvhptu.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gdovgcvll.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/glfnnmbnt.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gfbrlpnuf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gchkjgcrr.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhqttofn.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gyxkyvthq.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyxlpyjx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/garicaclf.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gftmqxryl.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhkwhirw.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkeyllban.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiglpsbt.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkwfaxnc.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gdobhkwhe.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gxmiwhnik.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gaxdgvibh.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsvtcwsr.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiqjhkop.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gdrvcizzu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garjdkmfi.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/ghoaoffki.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gaxgoawaz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gjljzzvpe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/ghurpijks.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgksizeb.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gdzwugwbq.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/growqatsb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gbdfqzshg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklnlpgyj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaolapnn.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gsjawlpxx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guihbcdbm.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/grlovzzxl.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gmbujvvkb.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gyglgcaqn.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdsuvneo.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvawnewi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfikdrvab.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gjukbsfqg.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwueqsezp.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gtengenzb.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gapunhote.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxiucafkm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grelaxllk.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gvjvduijj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxsbkvgy.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/grhoiaosl.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gewmepaok.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gainvhviz.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gvqfzkhsd.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gelaqxfwj.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/ggnfhonbs.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gmmoxbsah.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gssdtmmmd.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfutcjhw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/grpyjedmk.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/guwzxveww.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyhfnjuo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlyutaso.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkqjpcgz.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhxdqrvp.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjqfzwmq.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrgouqjy.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gkntimivh.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gtvvpmjab.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsqgaztv.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzpjmxlu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxafvxitq.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gavtinakp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gvyllkurb.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbwvgtqe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnnmdneq.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/ganaknxvk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbccsnri.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ggmcdhsyw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gywocegxb.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaygtmiu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/grgjzfluy.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdozgrzop.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gahmvaijc.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gnuarhncr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmzgokva.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gvjjdvjxi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcrlhxnm.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnstngsx.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszhxeecw.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrqyfeus.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfnjhtzj.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gbzfwzmyz.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/grjrhtdbj.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjbaansv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpthajos.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgjlzrwe.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoxqlroz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdixtkxt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gleiwzxlp.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfmhizld.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckjrngcp.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/glaghqmms.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/guyhegeml.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/ghqhlvihu.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyodrlyn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxicdgrf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfsknsgx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsqebvlqt.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/glquatyuj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfmzzgsis.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzcbcphd.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gknglwjnl.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gzdfeyyfp.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gfohnumjd.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gmqqqtkhx.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/glpfhsbrg.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gepnwrzlg.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gencghxyl.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gnyhyzonc.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gvbjdtnmu.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gdfvjrmis.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/ghockpddh.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gichjujkn.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gatvicpll.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gysbrzwqt.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmromkec.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/guktlolda.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gopocijfl.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/govnfcxhu.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gltmjsgic.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gzaqkkzet.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbdgxyzz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gqigrbhhp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gxgzspuuj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrxvwnuw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/ggrnfwgbk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/guonwhtxs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gufkpfkoj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gitidbtzs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/ginzvmfhq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnwnzciz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfovsbca.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkytksws.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpvzuavw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdaknqhm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gmpzmosyt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmfmwoam.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfckeyks.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gyehvtjpl.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gwarmayhf.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllnfbgxi.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gspgvknfi.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrcivjxh.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gmvorwmya.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gaukbhidh.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggudorjfa.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyksiudvx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/glecbhphi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gifxfjqxt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/ggodotfbf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gconutwwx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdpvlluv.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyrluwbk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gthronstz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmygfjbss.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnixehmk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqqmtwkrq.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/gyewczbvk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gycpfdswh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqbkokdj.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gdapbbdzf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gpvrcxvbb.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkbefxgk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqtxadbu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyhumwet.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/grbnoobqv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjglyuhzb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gaulazgru.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaouskcm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gurwrmkqd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdpyyikj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gveltxyna.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gemhmcjvw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fanxiaobao.xyz/Article/details/gqdpjpclg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gsijeszip.sHtML

【文件统计】
来源：http://wap.fanxiaobao.xyz/Article/details/gazabkfqx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/guxavlttu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgghpvsq.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgcmqfts.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmvfyaxy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjjffcrr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/glyjcuczd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvkqvhug.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gbethwcsh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiusvxdq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gcrdmdqqh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gumkzkfnb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gokofdqvr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjlpfusr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbqjeoqt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glrdjaiul.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkawloiqi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gstaqfwxy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtswxnjlq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/glrveiknv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbyfzcze.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcvkobph.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghettobtb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyuhmiec.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givncumzn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gxrdxrvnu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutcuwyfe.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gndzpfvvw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcyochvot.sHtML

[A01] Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjanqzmv.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbldfqysm.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fanxiaobao.xyz/Article/details/grbechqgp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnfnjijl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fanxiaobao.xyz/Article/details/gzcnqfbrj.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gyczefblb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gromjjaas.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/glfnhcyiz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdamzamq.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdceglwff.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqdahrrr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuftykja.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbfdqouf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlxnbzcl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gtgjvobcy.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fanxiaobao.xyz/Article/details/grmlavmlw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtklsvtor.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/ghxrxegbm.sHtML

[A03] 常量定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhdtjryi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoolvedi.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcodqsme.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gacyqfoos.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkitinlxo.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkximwyb.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeyfsfgm.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpzkssld.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzugbjzoj.sHtML

[A04] 判断变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjkbgjnu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/gjdngdprk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gsdvhszcj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gseigagfx.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gxebrvmxj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fanxiaobao.xyz/Article/details/gyvzcppic.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuufublg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpmnufnh.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fanxiaobao.xyz/Article/details/grnogblqm.sHtML

[A05] 整数除法与取模
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpwomyqf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocolfnwk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfbxpwks.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsonphjx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/ggghyzpvu.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gztschnqv.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gioppzgoj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnvuevkiz.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/guoyunvhp.sHtML

[A06] 字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/ghjoggfpd.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gabqnlqxz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gjutftfbo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpcurpkf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gokwnzqvg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/gnhcaxbds.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxurxzcbv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzktjrhzm.sHtML


<!-- 参考信息 -->