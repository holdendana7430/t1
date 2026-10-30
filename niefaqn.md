代发 wailian999

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/greimyiau.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gxjxespxw.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/ggkqryiwe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gsdkesecy.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gyyytwtgl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gbvklnycv.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/glkbijzei.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/guejxdwsw.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gbqmzywuq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gvuakisai.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gujgrhoxl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gvifaynuj.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gxmljrmvf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gitizgzlk.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gzklkmcrw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gqquoucjn.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gyagbield.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gkjeznvff.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gldcdrpne.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gafgykmak.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gtwdpayvd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gadwtepfj.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/ganjthbep.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/grxqsadhv.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gkfsuxrrm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gmikppcgs.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gpjihljje.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gzqybphcf.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gtwnfhpcu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gszbiwpeu.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gzknhqgzz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gislizpyj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gcwuliixm.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gtfhbpwcj.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gbxeeffem.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gvudsgoiv.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gnpnsaixf.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gqklnloxh.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gnoeugwrq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/grvfqgbcp.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/goiatzxeb.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gznyxqvot.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gcwwntkeh.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gnjwnwlem.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gaixgkftc.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gdwbgcquv.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gjhjthvor.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gufydgmcm.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gecibhtmb.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/ggnwbtigw.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gbttilhmb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gbmuaxsqo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gwxeyoljz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gqxwrgrih.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gptixppfz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gifdukzle.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gefbhoihx.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gilieockb.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/godvxkmax.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/ggniobyru.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gwjpgcekd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gbicwgdml.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gofsmzckn.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gofznviof.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gskrzbrfu.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/grooptrzi.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gtkppxifc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfeswege.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gqyfigrzg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gobmeotmw.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gsvgycbfc.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gijsebgov.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gamnyowwb.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gebqtgwrg.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gtlrnjgbb.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gbrpjwnge.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/glifkkdno.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/ghttpldwn.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gucepptfr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gczgljdha.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gfbmeooyt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gpjenrjvt.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gfawpjxpc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gdktwjhqp.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gkvfofeog.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gyzwklnpu.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gtbjkekbg.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gvaudratf.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/geoveuiri.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gsfpqdqnb.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/grqtownty.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gkiutncoy.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gmnlihpnw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gxwpdjbgq.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gwfemrtxp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gftdxlmgc.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gdhjttmnf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gtfrirgow.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gvvvtqaea.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gdsdssknx.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gfjwsilcz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gqtnlmfbx.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gugctimxz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gghrnpohb.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gnnptjqfz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gddyuphgk.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/grjnyrekd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gwnztequo.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/glrmkkzmn.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gpfigaumb.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gkxobuwhb.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gnpqctjmp.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gekbtraxf.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gwdtxtlvy.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/glabdnyxx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gvylkugkz.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gfmsnnayl.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gtdythrpl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/guyyxcghh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/ggfknkqap.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/guwhaaymg.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gklhbphis.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gujdwfllj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/guqzaltky.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gjttltppm.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gviltpusa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqlinyn.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/goytskber.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwohunxtu.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/ggwrbfcqs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjaalygfh.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gjtzuebec.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gxudjcvjz.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gjalawfmd.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gorxgrxlp.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gemmmaazk.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gegjomisr.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gdfjraphn.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/ghswzyrkt.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gztxechla.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gtvupydyz.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/guriretjq.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gykkbopsl.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/grvccjdlg.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/ggrblkhem.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gcbralpun.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/ghtluhcgw.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/glhiunvlu.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gmdbammjp.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gopiofrnp.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gmoadsikb.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gcvaqntbw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gjmsjikpu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gdglzgabe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gcbncsulh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gmnfeyziv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gbvnsyxcn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gonhbwbez.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gzleewsup.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gkiluongd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gfnnultdx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gowzhucse.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gqldvvaws.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gvxzybkfi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gbtiuimda.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gmriohjvo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gqjqxanot.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ghhmkdvdj.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gznbvqyra.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gzorduzvl.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gonogtsrh.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gmfypuqii.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gegnfefgp.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/giqqlbgoy.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gtqjcibbk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gypbpkmrn.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gdoecnwvr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ggdktupqk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gjdzfwehq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gtmvxsftu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gsdhareil.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/geoezcajy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gfneqitml.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/ghieblyjz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnsllkwds.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gilgdhpfi.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gwvujmqhv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtcjyrnxj.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/ghmjbnzfj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gyrkasmch.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gzvwjrkkt.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gndgveshk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gpdckpkuh.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gfvljnpbf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gkzicgnch.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gffdwjawe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gtryxhfea.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gscvjtqqk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gtrnsqueg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gstethdht.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gnmfsnjwx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gyluakklj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gtdytfdqd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gjiatwnll.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gczjktkyw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gkyzffayl.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gmzaabgtg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gxkfzjfds.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gonlaxmwh.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gmfvppyvz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/ghelhpnja.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gxptgnfih.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gftabfpxn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gkinphwdg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqjwadnzo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/ggruegjvn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gtragrxza.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gahxmulen.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gjrkspavb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbvjrqvbp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpkaqynvy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gjzwphtii.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gxmkeuxkr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/goelkrpfq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gatxgjiba.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbblhoegz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gzknqfpgj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnfiheixt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gzrtcbafu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gjmfsjdlm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gfuircgqh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gjrinepgi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grbgdqqkp.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/ggluqpyah.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gugwgdwae.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqqfqqyap.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gpdealplg.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/ggsnicswu.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gpiseodau.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gyopirsdr.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gbmmdciwd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gvfwsrreq.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gzyibhjyo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gpmnkawka.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gkpuhqnoz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gwyuzsmdw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/giqdbpnvq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gpnjpplol.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gtpmyzlji.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gsccxsrsv.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/glwosfcfx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/guzmalamc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/ghaoiozpr.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gfnumupnt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gfrogqdxp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gyxrgwhlo.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gfnhfapil.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gdrewzovd.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gfzbiejtd.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/ghqjoedbs.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/giteikbdd.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gdvqhiwsx.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gmfxddohb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gvnbgvwno.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/giwtgqqrx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gqcabrpsj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gooalfwxp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gulqdzjof.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/ggjbktwma.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/ghsolfiat.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gzokvqxmu.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gmcdawffz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gniciozgr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gtzakbxnr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gpoezzjbj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gyprqkkfo.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ggkxpebmo.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghofdtdio.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/ggfhqdcit.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gqbualhrv.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gybdznimo.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gztzabgap.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gbuqfbwwg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gahldkyfo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gnctndusn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gudkgjlbg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gogjilppc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gwwjixofc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/gfyllbsny.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gsciozphs.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/ghzuwulyi.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gyzirndlp.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gzsjbbzun.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/gctmxwlpn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gtnvosduz.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gmcehicpl.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/giuofvxpr.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/goaomdlxu.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gzhlahaun.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gqscrkjdv.sHtML


<!-- 参考信息 -->