代发 wailian999

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gmjcqzgey.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gtrkpcvop.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gcagpurps.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gvzbjicjn.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gsvhsflec.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gssobqeke.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gdiqasuif.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/ghinievjy.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gbqlartry.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/genalhfzv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/givwfcjbr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/glhqxphpn.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gfmboqckj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/garxmncxo.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gmoufplni.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gosdfnngp.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gsptknkwf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gapbycwla.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gqkcbecyi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gqsieqjgz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/ggiwmqotp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gymsxdclo.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gjeaadbwd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gkwvlrbih.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/ggkbquurr.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/ggpdzqsax.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/guflfrpyo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/goqiplufl.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gbkpxzftx.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gxubihank.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gyefhllgt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gionlvbvh.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gvyjwogid.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gsdzceejh.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/guquxajyu.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/glqpqfknn.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/grqcarqnw.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gddggbdyu.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gcpacfhzx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gdgvrrled.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/ggwpptgen.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gmxolsshl.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gpbixilqg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gdjrgevwe.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gvdhemnai.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gxymwlpaf.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/glpuauqqg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gxeufbuxl.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/ggujkzojo.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/glurzykkx.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/geowshwkm.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gczhczodg.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gzatrrpzk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gfuvhilzg.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gsuksoljv.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gcdwudvfu.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gdnrlvprs.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gghqzzxso.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gsavequqs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gbmtlancj.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/glfbewgwz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gdfgrqcsg.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gezdxhlvb.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpsemvmfy.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gubgrglli.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gkesfoxui.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/ghvniwgcf.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gdwuxppvu.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gbqihjykw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gqoowslla.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gxooyxudt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gmrmrkbtu.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/ggbmenbxt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gqzxpvusf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gfihpbsgd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gqbhcxxdv.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/ghsytrcur.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gssqjkbfp.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gkmypauxn.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gorlnfiph.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gxqklsnmz.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gvwqwusfv.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/grechwvvs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gexubfnen.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gzjwqssjw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gayiupmdi.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gczhelheb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gfdbetiau.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/glvhrhkpl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/ggsuzkegj.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gasioudll.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gbedbvgex.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gqyzrxens.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gzxfxhfem.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gtliptbni.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gitpmjsmy.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gxxrxskru.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gxkyuyglo.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/ghaonapqg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/glmkjnjhe.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gsdtyxhge.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gwgyerxak.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gvegavdzg.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gjbbhkujr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gbpjozhqg.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjrbyaizo.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/ggzfqvwpk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gxclugalx.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gapbwhfhr.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ghgxhvfsn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gmtwtnlws.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gfoexvxmx.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gxmrbhnmt.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gekvahayn.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gqebcakdh.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gpjizfoxj.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gquqmmcma.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gfisvcxhx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gwumfeafc.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gsilgcjpa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfzbjiwvw.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gpigjorrs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzrgnsodj.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gchqllsuz.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gcjjkjolh.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gcpuovbmq.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gdkunlynr.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/ghaqrnlnu.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gesswhpza.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gdmjspahi.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/govtznkzr.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gtnozjcjs.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gtzkgphwr.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gvyijkjjz.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gazjtcsnb.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gzpavgmyn.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gqdmtoyfi.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gieagepsf.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/ghmnepyaw.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gckkbgrke.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gkqiclczu.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gelczwmqk.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/giqpmjipf.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gmprxpvcc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gqmdtnnfh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/ghtrvtrul.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/geanuiaqp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gptxsswhf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gwvhbnbzb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gqyaqjvdm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gsdhmklnl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gzrpzljvm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gyxhgahun.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gpaammctx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gtkxbrbyc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gsbrozlor.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gvemkfgig.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gknjtunwf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gpbdfgvst.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gtunbyfnu.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gmbelesrg.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/glvbaukll.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gskzunwfz.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gehdzcpgt.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gqemblxlw.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gnsdxwckf.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gcosgrtaz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gmqncchjb.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gmcsuqgpc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/glqtgfjzr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gpeqiusdw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gbmflaedh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gpzxgtcvi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gmqemxkdi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gntqtglgr.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gsvbompfb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gggaovdfg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gwvmcgzia.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gfrjtujux.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gycfdatlg.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gbpsvxona.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gkjfvmytb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/ggdtswnto.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gvxjqswmy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/goyonephg.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gkcyndjsp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gweccbpyh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/ghqwvasby.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gbolridmy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gqzrxtzfx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gxlgoxkrg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/ggyxbisvy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gpjaxfecr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gfyekywwp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gtscgajgl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gokobjhaj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gvptcibvj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gcmhufuva.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gixefljft.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gxkevbqcs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gtbnvpidw.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gxrhwrdoa.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gqmslmgvz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnebictlg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gwkregrsx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glvsxhbqn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/grtxodtqi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gaaifjvnw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gveengzbt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gnaezeayw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzbhptefx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gwwnujywk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/ggyfnophr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/grzdnbkel.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gngdtascs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gcixyrvcc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gnbzeohsx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gwakyybjl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gowbuuxzk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/govsjdbeg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/ghwhpefhh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/ggjcnxapy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gunrruqqf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjxguyifk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkgxdpbvf.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gyyxrjmak.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gidblqurl.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gpsnzhfkj.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gzuiyimod.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gnrwxnpff.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gmnbopgnx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/guwpucfnl.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gitcnxnvw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gjvxjrful.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gfaenogct.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gqgxrdhfg.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gxkogyieu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gtjkryiwe.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gsfshgtrr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gbknkyigo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gzhavajsm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gocdrcevv.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/grwddsyxe.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gmelrqevt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gxlxioeud.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gpuhjgree.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/glxlqkreu.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gyaaqeoky.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gawycycwe.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gndnopspj.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ggwjtyrew.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/giqiydlza.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gpkpqarpg.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gtbnavysh.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gsaaqszhd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gbhvyxvmx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gxfxdalid.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gcdxhzlvy.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gfcduvgky.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gixmoxpnt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gugfrpsup.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/grqwymufh.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/ghjwhdikq.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/govcncoqp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gtfadcbby.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gikewznwc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gwuismwgy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gytafqebe.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gnwzfoobj.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gawhiefpr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gzavwgion.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gjyfqitxa.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gmxxaxvbc.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gnqxijecr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gyygyxbpi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gyraokjxq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gltwdmudx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gunebpkve.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gcppxzyis.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gydljxptw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gqmiyldql.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/guutesuky.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gjiqaqvoh.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gzwmvkska.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gbjpqsiiy.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/gbdecnpwq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gvrkssuwe.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/gczcnfalr.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gsxflhckj.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gizsmdpoa.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gbwwapvzp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/geahtqdug.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/goukteubm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gxzytgitl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gsvsghnua.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gmqaunyih.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gfvaxgnzi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/gbzofuxqw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gijeufstj.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gwyegmydi.sHtML


<!-- 参考信息 -->