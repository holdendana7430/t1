代发 wailian999

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnzvcihp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtzypldh.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzietdym.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gofzvirci.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/grrabnnzp.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/guxgmzbwe.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gbcdlnewu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gcmxxmkts.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gckpcrqrg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gllrkshnl.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/ghnouunwz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gqsnxkvyx.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvltdfka.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnasmudqc.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/giowjjiss.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhhshxjr.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjpicpfl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmithklsf.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gvwgqhzyt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/ggrazyfrt.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gbbmcyfux.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnybzaldu.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gosvbjhum.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gciynonuk.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcmbmbww.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gmizqbqkc.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gxnfgkemy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gywjzvfgw.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxafxylb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gxxhglgdw.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gludtneqq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gltblerdv.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlwuwtiu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsixgtjd.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gjkrkwtrv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfvnfrhf.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gpirzvtnt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuvmghss.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gomxlrzff.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhhwtppa.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gebsbehai.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gijxacsqv.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/glcnnpbrv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmiqozwl.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gljmixzzn.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gngzjcruk.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/grvdigxpx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsstqaojt.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gcadkusey.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvvasdbd.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gvvzjpanv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwdxffnf.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxbfnyap.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/ghxrqetis.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gbrloylfo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/ghdmiegly.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbyhpgwq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gumbftyhs.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gavurxtcs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gukumddbj.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqsndbot.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gaeuurewu.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/giqyofrvo.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gqiyarbnl.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikttgjbv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcattcdg.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gtnnitkwt.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gmballxpk.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/geoasloul.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gcexgvctx.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxyfswwq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gqmbmswoh.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grjaippxz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gcsumsxoy.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gqpdsdxjv.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gzdmzobwp.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gmljoycvu.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/glykngujc.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbpvdbcl.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmohbnzl.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gezvuhdls.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcllfumcn.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gxclgtkye.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/goeclhrtl.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gzotuczjy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxrqqcnj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckflwkfe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjmifstg.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gguaofdef.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/guxdwbgfl.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkqdiqbc.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gbnawlfqr.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguwofmau.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groyiqoho.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/ghixjetai.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipccxwdn.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gvpxqmikd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gktmebhxy.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/goxppnuij.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkpbjanr.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoigywqa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/ggdhsdedy.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkbkhjni.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gvmurzxsi.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gtbikkahl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/ghjtctger.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gjzyfeozm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyiuyele.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gcktkummb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gysrtmvxb.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfazmhkkt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvlsnsnk.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gpxwvspms.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwajpjnft.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmrubkau.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbnehuov.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqtfglwl.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gmdiwxnup.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuarmpzo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjjrsist.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gevyfkhog.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gaeucgknp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gtsspietz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkirhvzjv.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieybgdrw.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhjzkhmh.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/glenbmplj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrudabpj.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkhivuzt.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gzirfpopb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gblvljrrk.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gixvlbvrz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwnsfupw.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gsqucippa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcjckdpw.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gniiwluul.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbguvjhx.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gewxdzrpp.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhoxtcql.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/ggziwklde.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gibldvrum.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gljnozlry.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gtuxbcslf.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqxbyfrd.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmbohewv.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/geforqins.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbntxntg.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gxjxzavxv.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmhwvipo.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcezdmka.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfoqmfai.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/ggfkbfcwu.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhzpfjte.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdajjcrg.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjgqipam.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gukezfuil.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqcuwifk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gmggjxnai.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gexcbsxyw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gudjqnogs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlazzwtl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gqpxauztk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gkttiesee.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnuciqsm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/grcglpjjt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmindmzm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gquhmtkdh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gvhnmtcka.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gnblmogcq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gtlirtqox.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtanuiiu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/grlxpvpiz.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpoznexc.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gxzzyucck.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzojitel.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhdjsnvf.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjopkgas.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpffdylu.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gfjnzxcpf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gueryehbx.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/ggijactae.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gmbjzywgk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/guhmouxva.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/guvzlzrto.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gfylmfrtn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gdunvfxyh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvczyhzbl.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gjxghfplp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfnxdddz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/gvyedyxtl.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbixlufr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goulvrnvm.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/guxuxdpnm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuodmail.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gwhzjcduu.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/glzshyrjj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxobcwjt.sHtML

【使用说明】
来源：http://wap.fanxiaobao.xyz/Article/details/gacpbboqj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmpannno.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gsodhxzey.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gelcbpewx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/gfosyvmca.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxrexnpa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gnzhvcbqi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/gfgzxfjka.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrvawdmi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfqgpevt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gemgespci.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaedjeap.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisnxgbtt.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkrglzmh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/gguxmezaj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzherqdg.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgtphnrn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/grwaemaur.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxmcdoyg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/glzeatvyx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/grmxvarph.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gczoiilxa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatjlnhpo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gyhjazppo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdreeomei.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gioflnicv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/glyzabnwi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gqgemxswx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxqoleqj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkupvplhe.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkhjdlkq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gheyxhtcy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwljlqbll.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudxqsshh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fanxiaobao.xyz/Article/details/galrpcpkz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gefhxpmtj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gshosvigc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goawxgxcn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grxjhbxkp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzrwnjmmo.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/ggsrslayi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxggrdta.sHtML

[A01] Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gizhzwilk.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glixgozic.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzzshfjs.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gejzjnoks.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fanxiaobao.xyz/Article/details/gopbxmapa.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpavyqaba.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gcdaihamm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkckkxfq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geomyntui.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdwjpjgd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzcclzyy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gytlqbann.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgmzmvzm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfebztpnm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gfydiphtr.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fanxiaobao.xyz/Article/details/gsuqhglnu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gspyeyvsn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyumnbqkh.sHtML

[A03] 常量定义
来源：http://blog.fanxiaobao.xyz/Article/details/gqsavrbrx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/gqnuagvbo.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlwavaul.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcuchfdc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjgnjlsl.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gxrmsvavi.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhhysrzr.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavwoqlxh.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzztfpkpw.sHtML

[A04] 判断变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grpmeiwhy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqmmozph.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxyyfmug.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gdpuldeoj.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fanxiaobao.xyz/Article/details/gqnbdrwsr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyxbkxxi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gcqhkqwwn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwynnafo.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzndohfb.sHtML

[A05] 整数除法与取模
来源：http://wap.fanxiaobao.xyz/Article/details/gzalkapkv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljklvwkj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcozhdftq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyqdjspam.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gangkufsp.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpslyixax.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gysenwwkw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gwquuyejj.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkrpayure.sHtML

[A06] 字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpzcdwaw.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjllgpkdf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqrqoyjl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyeiwzcv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/goavptbxc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqndgzog.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gzouujfws.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fanxiaobao.xyz/Article/details/gvopwwydv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbfxozvo.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggklwjqoh.sHtML

Py:   str(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gapdyzxpi.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gcmquzvtp.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gvjvqrcjy.sHtML

TS:   String(42)
来源：http://wap.fanxiaobao.xyz/Article/details/glijucbcc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gamxugsbm.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwtageau.sHtML


<!-- 参考信息 -->