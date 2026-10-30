代发 wailian999

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gqddsnbrw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gabmfvblf.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/giwmwloyk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gngruwfbv.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gtmybyjdf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gpikohyxy.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gycehualk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gbyauowim.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gpwimbdua.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gqxalcxfb.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/grspdgpwc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gjibdhmhh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gnytdlqbj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gmzdkqbrd.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gclnlrmfj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gxqgwxymu.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gridkhjvo.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/ghsmrbuyy.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gvgwdavnr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/ggufpeycn.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gunhseakq.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/ghrufeisk.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gqxgipqsx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gazmxrvst.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gfekjkasa.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gzeqheeaq.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/guhmnkelt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gtrsfhecr.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gxpbmrexj.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/glazceoes.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/grjhkafvr.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gnxupydsj.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gmchapovr.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gyvasgixt.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/grycfvxjh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gflrffmck.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gkeloddzy.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gnvumtuvy.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gewuicmcm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gvcpffpkb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gqfdgkxpw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/geqwzrjez.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gqpbrnolo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gkukemsga.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/glxhwozxq.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/grmrwrifo.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gozkebuni.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gjzkrxgsq.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gvcfjbbbf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gqqgwdcbl.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gkwnuawma.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/ganofsqbo.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gpwyzmysd.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gdzwzmorg.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gmiaqagqv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gohifefsc.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gcgcexwge.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gewvzgvio.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/guoptjvti.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gmoonnicp.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gsoxotkjx.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/ghbouhkuo.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gysdrsscz.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gtduwhhbo.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gpubgdjib.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gldyencfy.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gpmazlbwk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gepdxibpe.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gjjztldtu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/glrvhuhin.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gzbisszta.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gutmaixrv.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gynjhkyzc.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/grfzyowpd.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gjiuempcp.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gmritaaou.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/grkvxsvbo.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gujupvxpd.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gdhkgchtt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gsftrelvm.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gvsigrmmc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gawxgbjsq.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gojzryazv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gfemftrdf.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gbfueepgl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gxakaercr.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ggfipfbrr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gseegkkdj.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gvxxkllyr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/goemrcezl.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gngzvvxwr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gxiaekrja.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gytymnkai.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/glpiizdei.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gumqzkecc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gqozhwekm.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gmsdyctjx.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gscjwxsks.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/ggqbufyay.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gcdvapazf.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gyloibqjq.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvrpdcocv.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/ghxnymmzm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gydvxnixn.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gllznvykq.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gijrxlcrw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/glxzxalke.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/goncamgae.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gvouxszpj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gwrlqkqjv.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/ggnwmtqjd.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gopjqyjjc.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gjneuidyg.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gizhkhrdp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gqkwgsdwe.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gnakqpqjm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvhjfkevk.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gejulhfbs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdpyhgabi.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/glgczhhgy.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gvwgvqaeq.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gmuyjpmfg.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gtxvjyrlv.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gmogpxrty.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gnjiusxnw.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gtssgrwmw.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gstqrdujd.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gvgamvyqc.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gijhndqlv.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gtjzaaxys.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gmxedhbht.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gojelbkjt.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gckklmcpb.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gnnhbkmlb.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gcoaihbsk.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gqdjlmane.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gdoyhusfd.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gnzigdehu.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gtqfbaazu.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gjaxmhmws.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gjctxjyfg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gzczvegfl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gavjyindc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gvprconbt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/ghzxxfltm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gvqgutuib.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/grwhcwsik.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/ghtzicyax.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gvktdktkn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gnbmhodhn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gguuubehj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gfgdgdelm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gwrhbgjpj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/giusiotdk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/guufyilqg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gpugtxvyx.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gelovuohb.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gjrgtlchv.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gwtyvtsmi.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/ggnksfjsl.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gwkwupdmo.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gecuyzqgu.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gjkfktrgm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gcaomdqcz.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gtogjgibz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/glaxvhxmt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gocoauxtw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gvdxmdosf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gocevqhxy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gnpvxpjqw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/goalyhwub.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gkurptvfp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdmybaupd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gelndfwza.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gnsecwpho.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxklqcfsg.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/giithjpzj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gjmxgeoqi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/grnemngbw.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/ggrwfkesc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gosaalddo.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gdhybmzhl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gjziilhkj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gtknjcjhd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gealcqsjh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/glpnbfhfr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/ghlnhpvji.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gzmsuiiob.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/ghlmxxxdf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/glywjhyxp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gowywaaak.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gecyfsgzu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/grwgaexrt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gnqqkmwmj.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gtgmoywoi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gqnelxdhc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ggeeelxfs.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/ggwxgkwvt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gjkxhqaoi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/grlxvrmxu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/ggmgacmrl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gpcuyyoex.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gnmpfntev.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gxpqihwmu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gidvwgnvq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gvkimmngx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzjidoqyg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gdtfafged.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gqwldupec.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/goprjllxw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/guhsxtzqi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gifvonfva.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gavrvksca.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gtfrgklmf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gkafepqtg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gbnuibgwt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gxffbsgel.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/ggcufbtdn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gtmmzerrb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gyylzxymi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsghglgjj.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gxicarcgh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfpnksbso.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/guxnkobah.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gfecvdfjd.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gltvagmau.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gezofooxi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/ghlliecsz.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gvyaxfjhu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/ggtdqvxhh.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gltkgorse.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gwdjpicyl.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gfjnfwcza.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gtsetlpbk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gcmyuachd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gocqmclej.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gpbjilhge.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gqyjcgqol.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gfcecvntv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gfckshpwa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/grjlbqzot.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gwmazgszw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gxewrpztp.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gehegkvir.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/grkuimjox.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gwpumglpl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gikulciyh.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/ghclergka.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gcgqkdvcx.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gznfjrkqe.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gcsnuybcz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gcydqmrnj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gogtwlxok.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/glnqqecqo.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gjecraebv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gcugbiegr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gpkniavrg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gefrjkxrs.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gjfyxfzaa.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gopvojbup.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/glothxecx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gpdxqbkkl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gfvptoghz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gnggnwtnl.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gsodmnnuj.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/goypqjvvh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gajzzydil.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gfnouwmnb.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gkxxbvbcb.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/glcpedbsw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gdfosnebc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gaewbpgjd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gzfufubfk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gdsdtokks.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gbceoxqsj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gpzfybawr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/geefkmmau.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/geqsrtbaj.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/guezdmfrv.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gdtcpwaik.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gsfqcxuck.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/glqtvbqrn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gvwkftuzo.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gxtbgsvml.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/ghgsuprgh.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gwybdhxeb.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gnzjqytmk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gvjdibwhn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gyzbvxsnn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/glbwqsevj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/ghqkmmtgm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/grutcsvat.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/ggamhfpqi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/guxyeufwf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gowyrxzif.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gkjhujgxd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gfnznvbyv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gewswxuam.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gguoxdzvw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gjwlqyruq.sHtML


<!-- 参考信息 -->