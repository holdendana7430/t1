代发 wailian999

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gjcrcmljv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gwhxtizqv.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gatgchsno.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gtztlsshv.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gpjhdapoz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gddpyyzjx.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gqyiikwje.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gifrggiyn.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gatwkpxge.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gljujjfbv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gsmecuqmz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gtfnlhwzf.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gzngyedwu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/guvournfl.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/guribptdj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gbipuitlp.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gbwpcsplo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gfrowdowp.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gyzybncwd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/groprxwxa.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/grsfdczih.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gsyemlhdu.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gnndufdqd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gdocoyvge.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gogfwczrh.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gxcuhpxyt.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfhbotvji.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gyahzonti.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gijlluyqj.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gasfpisqj.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gmptuejnb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/glayvfqho.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gpjtrtuhb.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/grlrqwfhk.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/guidlsofs.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/ggvlhwoor.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gimdkwicr.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gjmipuxdg.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gfykjlzgk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gollyeaoq.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/ghhoaqpfn.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gkmvmoxya.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gnrhubdsj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gtqwhrwiw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gellfupix.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/ggagmadla.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gbsukqzrw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gzcwwlici.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/goxxzxmxg.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gafikidyw.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/glkkfeqda.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gfxwnnzfg.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gphqhuiyo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gukdppcbm.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gvpzhawzq.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gdpvkftww.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gjtiqsmlc.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gvtlngzwh.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gllluoqbq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gjlgkpwvx.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gdfymzkqt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gqgahundq.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/guvpwegue.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gyypnhgmw.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gizhrayst.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gnktozzok.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gaunjoouc.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/grdqadkjq.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gdjjyvoel.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gjhnanddv.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gexjjhqrn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gmhuovwyg.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gwjeibaqr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gocgqeazg.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/ghkzbarux.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gceueploy.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gjomdalyv.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/ghdzstapf.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gjpfyeazt.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gopiwuzuq.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gigoorwbi.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gpcweamvu.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/genhfwzsn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gvsdckgrv.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gmaekjykl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gxuqrssxr.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gvzletwli.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gwbilkgse.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gdcaziziw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gtlibkjdz.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gyvmbmhjp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gkgphmuca.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gxdmirnpf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gopqslgir.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gezipqtuc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/ggzakafge.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/giqktqpri.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/glqoloyax.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/govclxijb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gdpddaset.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gsghzcsir.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/goraonfly.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gxrtfqego.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gvvqrwher.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gheryjsiz.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gehamxlul.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gmiwqpili.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gqcxhybjx.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gyjlqjhdm.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gfcwsjgun.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gnwwquean.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/ggbdhfesh.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gkfkxctcn.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gchrwfjzo.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gzmtqgimi.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gwdnzgmte.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/ghailddts.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/glnzpjwlz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gxdzphaut.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/guntklwsw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzipbmpee.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/goglvqvvj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grqjegzzk.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gfvotlhco.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gwysqseei.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gpsnvfiez.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/glykbontk.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gytgfpjny.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/grnxljhjk.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gdtsxutnb.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gumsjnyes.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/giyxiyslr.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gkdejlmix.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gphygxlcu.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/ghmrmtmum.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gktapfulc.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gngjbqjdx.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gueokrrhn.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gpflakxqy.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gmqghsoyd.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/guecekajl.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/ggyouieof.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gcwnipurl.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/geuwmlham.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gqafembus.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/ghojngydi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gijjvcoaj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/grmurtadn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gyyayvqnz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/ghunwzmua.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gnhhwndor.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gquznybbg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gvnxxstmr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gsymmierh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gzdkmflvl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gxhpuptrs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gdkiddmil.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gxadtdsqt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gpixlvqur.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gwfsvhlsg.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gndpduysh.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gmlyzcdib.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/goqeeouxa.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gfibswqkb.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/ghtcebmxl.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gfkkazyux.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gfivrpyiu.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gdodgeaqk.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gzvkahrav.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gxxfejzmv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gdjhompak.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gzplibmmm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gvigkerdu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gznxkywlr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/geuyoibmb.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gstzgzmdf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggawazhcl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gxgssxrnz.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gpvxlncti.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpowrqldx.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gjcxbkelz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gtqancssf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/giptjqsjs.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gekcxcczm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gmzxncpmg.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gharmeqrb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gkahqzfwh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gllzpvyuw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gbovtqwii.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gukouskuo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gurmbvnmf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gkueexmvz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/ghdprwsdd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/giugtmizy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gqqnefrsh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gtpyszdau.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gypqjwayk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gwttsmcqg.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/glfrhsukd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gorqbanft.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzilfzqbl.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gpkmzcome.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gxofykixf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gdhruxtzx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/ghfutzekz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gscaykimo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gzmfifvze.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/garjtjjso.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gmajedctt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gsdkpsehj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/grsnskywc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gtoanqyft.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gsfmhhnqf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/genwmztvv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gjhpjiksu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gpqyootfi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gjepkdjcn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gtffvotjg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/geqvitpsd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/ggsagjkch.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gqufloyqc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gddhevbgq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gwaukwvgg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gmnaegyzc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giwocnzlb.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gfzttveej.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpjoguesl.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gikwgtrnz.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/grztmutdw.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gfvwsemoh.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/glmkkoggw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gcsknifkv.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gdoenhimh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gvzqkzerf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/guractyqz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gareieppf.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gazmmfdrk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gpbtogqzm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/giiflehfi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/grrgsesgl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/ghgmuinnn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gjfnzgozh.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gmwfcmsxf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/geclbkpiw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gwngnsvnc.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gdtolbvdx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/goxkmxnpt.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/grsiuqlhp.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gcxdoyscc.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/godzwbnli.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ggobaucqz.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gqrvgfaoq.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gtpwrdtwt.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gcybtftrb.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/guehnjplh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gbzqqsqnx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gdaphrbip.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gactqrlww.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/graqzwryf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/ghstaztus.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gdworwjif.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/geqqemyjd.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gkajnopww.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gppjmwomq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gicxpcwkw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gsdxrirce.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gacuposmr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/guvjaryzp.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gtrzsjxgc.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/geegizmup.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ggecsrcbk.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gqlxlohnb.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gvzirgkki.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gihijiyzs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gwsgpolhg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gifofdtto.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gpozbkdwz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gfcsbwbdb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gkljchtdu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gyfigmeaa.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gahgomlji.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gyqqexgtj.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gtnudnwjw.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gdzxxzfbd.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/ggruplmuz.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gnfnnnpnc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gyuttujcy.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gdpjuolpj.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/gluhnvjnv.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gxbaseyvl.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/ghncoqbre.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/goyweofxb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/govkkigum.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/glgnjzqag.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gslhsvjrt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gsuwupboi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gfdmxtund.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/gjuxlbuik.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gztjhymvp.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/giehdjeqv.sHtML


<!-- 参考信息 -->