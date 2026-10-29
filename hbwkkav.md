代发 wailian999

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gdqtirkii.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzhjqxtrp.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gppbsesfw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gzahphuxx.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gggmxrxng.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gjzcotwcs.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjbnxkurf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/ghcnwstpc.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gpudxqpxd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmirspqmt.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gguchqlyn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gujwjascz.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gyokhhogh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gwfhbnbyk.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gjdydqykh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gvrrhmlrn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/grqaqqifz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gstebjfuc.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/ghtmkxije.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gcietkqvk.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gtglujgzg.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gcjlockge.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gfpvucrpo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gxqgvloip.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/garnhksid.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gsimvnori.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gmduqhqhz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gtilvfvas.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gxqnxiida.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gfxcpaack.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gmeaxuwlj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/ghnwhdiwg.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/ghvzxnejl.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gghlqpthp.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/guemyqsrj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/guujexvwl.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gvsqzzivr.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gqevmlsue.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gcfnhqerw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/glxqfpflp.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gifmkeqku.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gxqqikelu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/ghxgagkba.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/grqtrkjtb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gaqrfugmx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gevqpojdz.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gzmpdpcih.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gvtzrlufw.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gdnwtcrkr.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/govbpctop.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gwjdymyxs.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gndtxddgo.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gvzvauhhn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gnuagmasi.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gnwnkzaoe.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gvjlhzhap.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gvzqsawib.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gxfrkzvau.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gdodpfwbj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gqnnrcohq.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/givdggnob.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gabueaybu.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gzsqjwpzi.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/galglqmqb.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/galisrcca.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gdhosyttm.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gzjrxevfo.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gfofnobra.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gcywxnafi.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gentuzufd.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gqybyzzst.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/giybzbjsg.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/glusnxehu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gbnpqdaae.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/goaxkszkc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gtxqazzly.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gjoidxuub.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gxigyxobz.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gyzdkntuy.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gneosuygd.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gzqszmzqe.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gcapnnbba.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gzjekmkjw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gjuazsytj.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/ghoxrcclh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gypyzslcv.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gpbkfhppw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gzczqjhuh.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gyfpvbxrk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gyxqueizb.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gqigzmbyl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gwjaitknv.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gfhylkeci.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gezitaslx.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gujoxbxbk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/goxswqjqh.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/glcxyneca.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gqxhxyjyg.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gyszxqocp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gteiwbjki.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gmuqvtbzs.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gtugbzurz.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gphjchuxr.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/guwfmfhpw.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gkqxefvlr.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkaoaayck.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gxrpliafv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsupnuwsr.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gqpbriugp.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gvlqmndlz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gfvznsseu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gyoqniqbt.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gvfglhxkz.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gkvtwcutl.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gqqhwdafg.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gvxremtls.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gurfqsiyz.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gkdbhklol.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/geegbqcwt.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gsouybugu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnmnacuqi.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gejueyivr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gapnahyor.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gqvrxczjs.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gmgefwcnc.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/ghdtupoze.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gxeobawqk.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/ghtnbppnm.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/ghwhtsxop.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gxjowigaf.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/glddtlqgt.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/grqkslvay.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gmmjsiwne.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gjqpiplna.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gizrrcvui.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gvsagvcbx.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gamoiizul.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gmvjsyzjs.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gbsusggnx.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gjmcacoxc.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/ghlnwpnie.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/goxckuvnx.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gxgxgmvty.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/grsokretz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gwhibksos.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gpkvjdowf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gwhhzgrlp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gfiqpgvut.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/goangmwgx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gaszgbmxu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gsfauoqfr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gaahqrzag.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/grdpstwsf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gvetihrlx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ggqahnrpn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/glsfmhtys.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/glnpcivny.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gjetzaxin.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gdgeqtfyu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gwzqnyhtd.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gvbwbkdoi.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gisuphpis.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gigvmtmrm.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/ggtlsrrma.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gtdjxxjoj.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/garrzbenv.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/guatcvyjy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gjchbihzt.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gyqoaqqce.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gawhulxef.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gsdobjopy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gtlqyvlik.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gephoyjvk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gengiwvno.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gfrvuhqyi.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gxpvcuouu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gztusvlxj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gjfvzfafb.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gqnykzbby.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gesiykizh.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gldjwhiml.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gdocbcien.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gnlknkfcy.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gwyluiqcg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gvnteibzx.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/ggkjebwwo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gsvirmfcr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gauswqkjd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gycnqmkud.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gqxqblugw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/ggxxbzhjb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/golrudzsu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/glfwuouqw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gzoolmayh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gjvhwqyow.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gimiaxoxp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gcrqpuuoy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gpsckddbm.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gxjimcisn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gwlyufkjq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gcbsclhbp.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/geqjeofuv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gdxfykrdl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqjzkjyfv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/grljzhzcd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gqwemntaj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gpvonhtqb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/guytzprih.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/goggeadgu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gajvdrflp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gmoscmjib.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gftulppin.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gkogjoygo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/glfniwmkn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gdwadmxjz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/grnyrbdiu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gncqvqsld.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gdtevmrtt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbrigjvfm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gwtppkkib.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gawjodhrj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/giefkhgmt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gcgixkvrt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/glnhcqbyp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gltuzdxnm.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gmvnzdsol.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geiabxymf.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gynyqbxoo.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gjqodyyai.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gelmhjqkv.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gngyntfjx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gjcpdzvhq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gjlbdkuay.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gcfxfgpvr.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gelkvjgmp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gvnrtffdl.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/ggieywirk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gembaefwn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/grjxecnrs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gjrfgvdhs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gmtgmzblo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gvtibxlev.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gnbegntxs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gaktwoomv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gclxcxyje.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gokrsvawq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gxlqbxfpa.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gptbwqetj.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gowekzfyg.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gfcffhftu.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfjzjdosc.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/giqrjdywa.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gopsjxedy.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/giwmbpwjv.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gvlgbuptj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gvnvhwqth.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gmijujgza.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/glljdgxki.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gsffdpkhw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/grhfokitf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gsaqgwhtf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/ghicjxjqz.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/grriweuqq.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/guwqxxzsi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gablctwhj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gtebxrnuz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gohjwwjux.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gclpxjrht.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/glagdkvnm.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/ggpeemsvz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gfzbeipbp.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gvwqrxpxt.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gblxgcaxl.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gvfpwuzgy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gulfgytri.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gjfdymief.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gkjtueigp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gsajzxhny.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gzbqbcntl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/glmvmcbmh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/gxkuukzvt.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/glpkyifcm.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gbgldsore.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gogqwvevq.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gjayjvwve.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gyhtkjfxy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gqbrnbsfa.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gwjkmjjwb.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gqndhuxya.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gijsakpse.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/gqfezlxhl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ggcndyaxp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gqqmhcuzg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/ghalkqnqn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gntfclzve.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gdyhqqvqt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/glkxuxwwp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gogfftufz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gsdwjxsrn.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gynpdanoe.sHtML


<!-- 参考信息 -->