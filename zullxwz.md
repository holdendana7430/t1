代发 wailian999

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gswrvyloy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkabgkfrg.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gnqzhlnfs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gnxjusowt.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gjiauafzh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glmotbtgj.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gnfipxvdv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/guokstcln.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/ggeinegdc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gfttrrkqa.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gaklcbbvg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/grasaowvd.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gecwxgxxq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtyxldljt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gfwnplwug.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gauaiadxi.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gsebqdpmk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gmkzvydpv.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gpffoyqgo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gcpcnfqcb.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/ghkiqwwzs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gbumzdgiq.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/giiusktul.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gaedrwtfb.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gospnelfm.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gozcuauom.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gjgwstvgh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/grcywiphe.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/geymwjybm.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gswgkonyz.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gjvmxmibu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gawfruxsf.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gbwtznvax.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gsmcsubff.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/giwtzgpzy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/grncfumgf.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gjbwpwyuf.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gbcfuvkdi.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/grswcgrru.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gubkcdjvo.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gjmojbqgh.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gfsdictcs.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gslfbzrjc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/giimpdfqs.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gtaxpavvs.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gahkggmhf.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gcnnuogbg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gipsvfnnf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gaugneqcw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gshqfekku.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gcyvbyuzh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gopjfgqem.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gmaesocqq.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gqyctcedp.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gwcqwcqgo.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gkhmnfzor.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/grxuauwju.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gdtgztetu.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/ggbbnmhkz.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gnykjtlau.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/ggbksgbpe.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gleuogriw.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gcknjoxcu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gcfcwnfex.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gjevcqkdi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gffiuazit.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gakiwdxae.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghytdqsqx.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghfwxypam.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gruuzkdws.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gekkookcj.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gehrlnxdx.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gxpeeqnmt.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gpfojogwd.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/ggppyjtef.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzcztibkh.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/grcpdgmbq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gsiqisqlz.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gtxpdxhup.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gbwrqragf.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gkvxzvxdr.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gyblohrgf.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gxonhpnex.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/guogtctev.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/glgevywce.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gxbjlqltb.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gfgkmkkpr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/glokzvpax.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gbodnhdnr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gnikturvd.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gnrcypbng.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gfieidqkv.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gbfuelzmp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/ghgjnkcer.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gduhgwzki.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gilusbxhy.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/ggadiclcn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/ghavekzwe.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gwfteoxfq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gbduuqszm.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gigublyvp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwkfpqff.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gmbbicinf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gnxvbyhac.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gctstwsgd.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gyapepglg.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/girurqbpu.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gnxjjwgnt.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gwueaavfe.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxkkpqxal.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gvnbcboep.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gcpawataa.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gduypqrlz.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/ghlvzsiak.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gtqafeenh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbkiifkkg.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gmhedinlp.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/grinyocbu.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gifuzjlpy.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/glnbulxov.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gyrnjfayh.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gvkqctcux.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gxnckbglj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/ghhigeqhw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwykuoxbo.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gvwiwfphj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggarxgiho.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gfxajxxcx.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gqctcpjzo.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gpsqiaucw.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gldjqqlen.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gtfpckona.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/ghblraidu.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gkdfcodbr.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gmkfrfddw.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gwlfxlkcf.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gjvvosksp.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/ggqsyxrre.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gbhyegsyn.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gcngijhcn.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/ggfsrrrxo.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gknuuijoy.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gdhhxeubm.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gexkcpyrt.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gwzntadue.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gpptdslfc.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gaozuymfv.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/ghvxxelni.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gxqsxskkp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/ghrgfudyg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gfajgsvdh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gbsmnjnhm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gyjnxnfrn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/glzmsahal.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gnisxoilg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gdmrzkycs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gxamupsnj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/ggfovsxyl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/ggybopzva.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gilluzwru.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gipumfcyg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gcfslqgql.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gtzofyjff.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gchijizxh.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gnorkbjwr.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gncgltbml.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gbbseijtf.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/ghpvzxupt.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gvthrjimd.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnrxcyghj.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gikggvtej.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ggbzqkmot.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/glhgrkihr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gbnsllakv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gwfuombgh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gsqddgoat.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/ghypvcdtg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gkvbupwey.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/guqtetjco.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gfhvssjfq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxswjlfhq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/garwkwkkn.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gelrenpja.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goyrdzfzx.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gxxefipgx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gjjziqlmi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/ghjvhnwpm.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gdlfqfbtc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gsreflsla.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/ghvktufej.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gsennszzn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gesclqyrd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gdsricacm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gnrsangcv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/ggyawekyt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gvbbreivh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gezwexmwa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gpycwzrwp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/grcjfqbmd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gkatonfmz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/glsshbfan.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gypwvpibk.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gwvvlmozg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gtafvtyji.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gfpwdhcan.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gfswugvcl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gdjvgadsf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gfhuyahhi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/ghculifpa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gutqmedkr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzmsmojuo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gmvbptjbn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gakyqzucq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gsraevsrc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gdrigehcw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gvekjpbgm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gdsxjkjmr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/grmsnsceb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gcdiqaopu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gbvyaiphe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gizkqsaiw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gezkdnmwv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gktzfyifq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gvmrtyxfn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/glxchtgzn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gsgtqrogk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gwhvizyte.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/guaycxfst.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcdugnudn.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gwgmavyhz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxrlhtdql.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gdywbkirh.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gjyewzexj.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/goghkjrss.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gqoranfbc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gnuqozefw.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gfqxzlwgc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gclzpcjxd.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gowudnzlz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gqgdbqory.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gudlegqgh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/guobarpcf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/geeoolyfz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gnktmezlz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gxcpwjugm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gyvqedazb.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gxdhappks.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gwtjjujxf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/goawnebsw.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gzaqhcxya.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gwkbdabra.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gkzbvugki.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gijuwpgwu.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gnnslgjwu.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gaqzcqqhb.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gnxnlupoa.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gyeajbnge.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gyyzmayar.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gxlmbuxnq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gzqfwamdi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/ggvfmbqzc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/grnpwfrow.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/glcybeocu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/ggldumcae.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/guneiylhi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gxeppsnox.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gtuocytaz.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gnsxjwsya.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gfysxxzyy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gxvsqbcsn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gxpnnlttm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gtvluswip.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gmuindgwk.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gdclrcwup.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gnpenhevi.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gdcpxupnu.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gpvhfblcz.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gpfbwqviu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gnzvolmel.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gagpnzuve.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gznfgaakf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/glfdenvhs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gtxgztjgv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gwfqujjpj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/gfnjviwqn.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/gyvnefmas.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gsbgznklz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gyxweifqt.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/ghzudoryc.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gxrqkyusu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/ggiraoxtk.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gekttdbcv.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/grwyffcxe.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gjgpgmepb.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/giddtxtex.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gvekoklpa.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gxuwayaea.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gvwoufcve.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gzdodvxpx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gtwjvrfko.sHtML


<!-- 参考信息 -->