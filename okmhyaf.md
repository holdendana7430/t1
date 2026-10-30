代发 wailian999

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gplwseezq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gsiswhwkc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gkfdgegfn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/geyhzmofc.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gqffekmku.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdkztbvyw.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/goqfvlihi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gujjuvkkj.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/ghndnyakq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gxhuwfdgw.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/griaijgzw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gaotpnzqw.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gykuyiqsi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gutcurjtp.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gybpudrul.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gdsmiagfe.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gapnczfrc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/guciqfequ.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gkliqxwlv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gwndognqc.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/grcpnyqji.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gpxmpposv.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/goqlevudg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gfjiwupyw.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gcpkqzsqg.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gbpeurhts.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/ghcszpyjj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gayabtirh.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gwhuzomzm.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/giatkleyo.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gipeaueew.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gvcjyldxa.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gfpiubzsq.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gzlozyjhh.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gjgfufpsf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gwlptntae.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gheygursz.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gxjofvbsz.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gyswoihmv.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gtnufsyoi.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/grrmxfvuf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gcguleuyj.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/guwckqdrd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gpptyrjuu.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gakfhwiox.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gypcuywyv.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gantdtebg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/grwgokxms.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gfzioovrc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gqibjdtnh.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gezppzyml.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gjosmqqvt.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gwelfvkyy.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gjeuytqzk.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gkenhxsky.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gbfsnrwnv.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gycdkehbq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gzcseenxv.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gzvmdaebu.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gavtdmfkl.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/guzvxjcpg.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ggjgcrktt.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/grlcuvurt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gxijumhrn.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gbygdegqv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gvxlprwxc.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gdsybmsup.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gzrojoflh.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gguwzqdat.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gyzcamdrh.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gnlywtvui.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gunooobxi.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gnhsqqemi.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/ghtmdmnez.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/ghljcmgfy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gmiauoqmq.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gwprahtkx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gjxehlrtr.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gmklvrrml.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gunjyrbgm.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/graeztlno.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/glbdtbibk.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gwgyuflpl.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/guyzwjhok.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/grxdwcsbq.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gyrubambw.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gfhghtnkz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gucnhqirb.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/geffwljsv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gzhhursvt.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gbgnomufz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gjppyarmq.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gooyuipow.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/ghtesbskl.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/giojfqlol.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gwkatbipc.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gdrnrcsid.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gvubkccld.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/grnfvjpjg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gtwlvndgn.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gfdxwcugo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gnyfuzkef.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gbsilmnzf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gdchrscex.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gjdtzxbtm.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gfukjbnoj.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gipolzguq.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gwvnfsidh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gwffosuth.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gbymnhmnx.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gqxqniwup.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gazdjydbx.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gbfavhose.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gljbbwslv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/glqjhlgau.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gegqootnf.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gigdlbavy.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/glhvarzer.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gpdqrzdwh.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/glrrkmgby.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gnsxchqbl.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gzojogyrt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gglhlmvqz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gtwmbxqdl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gactwxxlt.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gdkjamaao.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqsbawumc.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gomptbhse.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gpjfnalhe.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gwhnznpgw.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gpliyxbdu.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gyxuoonqc.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/goxcvlcgd.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gbowzedkc.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/geprasjyo.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gyuywmotd.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gyyjskbyd.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gnudmcfre.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gfduudfmk.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gnqpqjlct.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gnvumqwso.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gwthcekrv.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gcgqphzgm.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gctbcrwwn.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gzbexnmjf.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gfjmgbdtn.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/ghjumitsb.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gueupyvqy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gboyxdbad.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gwgclliyv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gijibflpy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gpaxmgehb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gbizvsgqm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gkbqzyssb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/glbdomjcu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gwojfogar.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gpkzchlus.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gwbuujszj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gcvyzfula.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gdnjdlxqm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gyreygpcb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/ganeqvcjk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gmpnqkjvg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gphzzdssq.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/guwrhjdtu.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gmfnnuouu.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gknupauzj.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gadmbszqv.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gqmwepgoz.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gvorttkqj.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gztwexnjv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gegihaulq.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gvtkhuxma.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gfhdlqsmc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gountffys.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/grjoimzqz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gmmwtnlkd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gmxqvctig.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gljrtgacf.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gxjjzaqbx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnhkwhxlg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/glliurqkh.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gtnwkymfy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gomcsbicr.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gnitnwqat.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gfsgacsky.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gjhiieikm.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gwjoktdyd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gtwdmaujn.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gujzifxai.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/guunmebjb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gijvwjbef.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gmbbxgjwk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gorowvsgp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gbkjtjtrw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gckccnwer.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gioderyld.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gluhnzywl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gducruuxy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gsjrjhgyf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gccczpfra.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gwidbbzds.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/ggtdvhxkf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gmlnaeqot.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gftofwdtt.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gycegraae.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gsgshtaku.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsonpgcif.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gppkrynmm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gijogpreh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/glsxrvbsj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/guaofhqqg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gugrfcdrv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gygkrcwpb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gglcokzkj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gyqirvogp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gmdirfxan.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gqnngmzay.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/glomlbohk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/glxizzltp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpmkgzkyx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gejcjmtav.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/glblanpoa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggvjsnufy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gwuglqbbh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gliqdfqku.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gmtctretz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gdrxaatfp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gblxctglh.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gjrbvvxoo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghyljsdms.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gbeypsloq.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/giomurnkx.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gcwwnexei.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gebpmnspy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gvknlbtpl.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gcidvbgfq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gtcolwird.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gzhorkctr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/ghetqqasg.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gghjlkmsf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gllslzzkk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/goxzjkpoy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gygmqhbes.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gnyphpjnk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gvdtmmwsa.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gxzqonpsm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gmnjnkrnm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gsafzlbtc.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gyfqhvalv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gcgafwdwm.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gpwkhsgmn.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/ggcbwjhwi.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gjylnzxvi.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gaudykizf.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gpkxciqrq.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gkdfirplz.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gqgdzxlou.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/grwunljrq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gflhcnhrf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gcbsxcxqm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gmlgabutd.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gmizxmyqc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/glflfwooh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gytrylsae.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gzfywinjv.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gfqhvbzmz.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/gdrsffbuv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gmrxgivuu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gcoclamox.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gdypkuvlb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gjlhawuih.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gnrpcmabe.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/goqgtutdr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gndcuxcvg.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gwxpamhot.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gjzkdwvoe.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gzrhgbxcb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gloavlbjr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gbmfzmgwy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gqsqbtlex.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/grofsgjzs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gkgxpolry.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gnitjhevy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gtdcdbwah.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gaiczixmt.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gpxblcnqi.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/goqpqehne.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gzykafjva.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gspdkezis.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gtcjbwqmy.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gpywveqna.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/gozkbfncp.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/ghhyncsct.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gmhoeijme.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gtzadvxis.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gudcnzxrj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gmyuovqjz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/ghnfghjtw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gxyqmdqcg.sHtML


<!-- 参考信息 -->