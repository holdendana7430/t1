代发 wailian999

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gvsyrjrwt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/giuidxfgd.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gxeglcbbq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/ggbhwmtvf.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gxygluuij.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/geozqeerk.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/ggeftmnyb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gzbyvloqk.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gcegcqmqv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/glttpciwp.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gfjquhlne.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gconkwlwi.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gxlshxhqz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gwpmmqzss.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/guvnmxzdq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gwuwyjchs.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/glnvlajyq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/glgmijeyk.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gybxtjyqg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gbumfnroo.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gfkzyhyox.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/ggwbnlzuv.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gqjsazvur.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gvchlptnh.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gwnxepqjh.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gdklaozis.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gonibrcyj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gnprozklm.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gihqunwxj.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gixxtwqls.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gdqefvhef.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/glcrvsdyy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gymzrwaoj.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/ggfquucpx.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gmslsoqjv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gfvbptpsj.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gjcizybtk.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gdqiaapxn.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gvdyrbrem.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/ghwhbfhlr.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gkvfhuwfh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gmyzbnxyj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gknwnqtky.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/ghkgvmqoi.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gerdhnack.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gtvjvbrgv.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gepdbymob.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/goefzgzjh.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/grztomary.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gjrgdawam.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gcsisxrta.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gvrduekmo.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gqhozooal.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gplakreol.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gjwwzrwsi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gwsbhwxss.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/grflbykaq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gtadvjqgo.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gcqwtnhqr.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gaoqetnjt.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gobdbdeaq.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gxbxhpmdy.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gahqwbsqw.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/guflbaokw.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gserzevpq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gfbfxzdyv.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gdtpgzcra.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gdvgocedq.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/guoaavvzm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gjebizlzk.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/geqpxomub.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gxzfoizyy.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gdsfokyaj.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gkoovpikg.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gqrfhikoz.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gvwwmrpcb.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gngkscolk.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gwzxeaeqm.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gepveuviu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gyaafsnyl.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gqzrxopul.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gsdubakiz.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gyiwspryl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gtsewlcld.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gympbupwl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/grevmbijv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gbgwmhpqp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gsqvcznmq.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/ghhyszuqd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gkhprwvat.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gozldwbie.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gvtrpbuzb.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gszpclvkj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/ggkoorqhw.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gcsbecaqu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gqnwbkcmk.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gprrprbkx.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gttblrxde.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gulrmevjw.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gohnsbdie.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gjinawryp.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gespighuw.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gcmkpkuwa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/giklhleiq.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/grqxzjhef.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gzdxjmehu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gkwhcgkbn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gfpzmflgi.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/giapnegli.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gxayagnqy.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/giaexpmth.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gdgjskgid.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gesdslvua.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gynwkhzja.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gtyjdppmu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gkayvreoa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmgyqxzxu.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gernrvjcx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcdackcth.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gxezeftjo.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/ghlieotgu.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/goaoixjoi.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gxoahlszw.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/grzygzaot.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gjiuuhynt.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gngpegqth.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gdvezspub.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gxnragwzd.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gvaicwhrd.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gbvikqvgy.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/geijvqdcx.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/goqvdqvnv.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gcaxalgoj.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gabmippco.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gaaqfjvmr.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gnqmmnhqx.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gefwrwywl.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcyxrjtjt.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/goibgowgk.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gnnbtlzaq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gjofpxfwo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gaolpdwuz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/glhthwdjb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/guyikuhdo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gzifajlda.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gxytawcld.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gvrqffwtp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gmeualabq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/guwbltegj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gfzftmnog.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gancycrle.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ggxctfznh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gqeqhicmp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gsrfuvrsg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gdldgnfqt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/glmjnnpzj.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gmsjnlnyf.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/grrhlplgg.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gombaixsn.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/ggzlfwaco.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/ggazokxpg.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gikxvusuo.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/ggttwdelg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gvegvshgv.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gojalkjzi.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gnogakxpz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gpsfkulto.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/ggnysesmc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gdjzbaxtp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gdabdkcjf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gkqnlecpz.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gxjixnzxr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpznhgsuz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gvnsocnqh.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gdggpzkqk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gisaknbkh.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gkhyhkkfp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gpkbddbmj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gzcalvpzs.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/geflhjzre.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gugoawkhl.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gttwqpdej.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gasioklxb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/ginrrceer.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gqbsnwfec.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gzjjqtodl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gjliyvraw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gmvxduwbo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gjpewgmsc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gwwrssphy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gzgvrlryk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gpeuprcro.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gknelrcbh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gfcuvivzl.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/ghzrodtdi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/goyxpneus.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gbwlhstry.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gbcmnjcca.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gpgfsshtq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gundnjwno.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gttwlkcyp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gamtvmxam.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/goycfurtm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gwpnqyfcw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gzerxlvjp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gsysetegm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gwpqcupos.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gbhqnttvi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gxygzvyii.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gwsowxcoz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gsikgizzy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gosjbobjr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gxuzinnyj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gupjezabm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gmfiuhuws.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/glauzsery.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gvfpuzode.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gyooyhluc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gpmdokjbl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gktcfduex.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghjzmlnur.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/ggjwyvkgt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggjcffpxg.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gltkoqktk.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gdlpzqzoo.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/ghzrtskci.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/ggaxtsmry.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/ghmdenzmu.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/ggvryhgqx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/ggnlcsawo.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/ghnlapkuo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gggoswxpf.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gpqmnomms.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gaxoosydy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gewoishvo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gxkbzpvng.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gfktjhjvb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/ghctvrosu.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gstcgqjwd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gzmezulon.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gjluvekdo.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gjgbghwkx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/ggolpydpz.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ggcrijoww.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gflhznyym.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyifrdesf.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gvgphjsaz.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/ghphmnjrx.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gprtgrixq.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gnfxpdmfq.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gcsljkzly.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gbqouvzjy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/geozxbelo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gjvqntdti.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gzodszffa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/goootumds.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gntulliyq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gjxxagqtc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/ghqrgpzsi.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gwtmbpqct.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.zdbjq.cn/Article/details/gqedatyfl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gnxopsxne.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gwrzvszzg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gimmdahmm.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gjhmueeia.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gnqjneqjq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gggkyhdvy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gdjgpogxl.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/guywaytvv.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gmrijenzf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gaaklfixf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/ghkudpcqd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gbakedhjp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gzpkayfud.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gdgytzwoo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gxjtcxctv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gfzhdhozc.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gzyueqprs.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gwmmydpvi.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gcsjrmuzn.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gnkyvncep.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gvecpziin.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gadelrefs.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gnmsqwyce.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gkvgzguif.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gvlqhljml.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gifylrozo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gakwmrtat.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gwhgiyujv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gqskszzjx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gfmqaacde.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ghnlcjqrh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gptptekgk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/guhncskop.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gucwpbnmc.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gndhfiask.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gissmxsls.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhendgue.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gvgjinjvf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gpuhbjuhu.sHtML


<!-- 参考信息 -->