代发 wailian999

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/grrwwmomm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/genwfxwnm.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gloldeaip.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gdujfkgrp.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gcketrqjz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdkuebtes.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gloanrheg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/ghwmqybcb.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gzybcgbcx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/glkwpwrvh.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gqthnlxwp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gxhxhrzmf.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gcwfjmnul.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gcurvkjot.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gnbjeruib.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gibyqxdft.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gcmfuypdz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gyvuczspt.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gmupllnfs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gbtmvasti.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gynpufhai.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gyqxskudj.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gfmwjujyx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gsdufclhk.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/goafbgted.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gealjnued.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gittwkrfz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gohvqygni.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gwbjhwnxe.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gfbybaqxo.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/glbltclde.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gpjkbrwlx.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gtmauqvbp.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gelnmmlvj.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gazzpyayq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gfwrrdecq.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gwurssxmv.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gdzrylphc.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gmuqygcnu.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gklbjfeqw.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gllrzpimw.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gkoabucwp.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/glqxdotct.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gvdglygau.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/ghodusjpf.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gpefpewvf.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gaqllbdyc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gggomqzyc.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gzthclvms.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/ggfchyuru.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gzygxaeix.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/ggaywhhdc.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gzbaojtbj.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gruhkvinn.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gmeormkzo.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gngtxikww.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gjkvspuou.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gpqigjzxx.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gqwnkwbov.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gyjoaaxwh.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/grphqhxhk.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/ginpzjfwh.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/ghjchfbmc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gmnfcnwop.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/ghymdgwso.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gfdlasvxc.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/geivzpsub.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gppmecvff.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdsmatfme.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gcovmlhds.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gqmnlxyri.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gmmwkfsjj.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gydmskrlx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gidgctbbs.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gpicemqob.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/ggpdtlsmu.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gmjmzufsz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gxbahzbtu.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/geiqocatv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gaufexmle.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gdwdayxts.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gaxluemun.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gawlurqfo.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gthslxwlg.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gdjziiudy.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gewjexebh.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gqeucwkat.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gzvvztfxe.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gohrgquda.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/grrzfjbbr.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gjhcgeudj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gliihssvy.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gwjxbcyba.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gdkcbizpq.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gagzdwitr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/givammyon.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gwcddtssh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gmxxgwqnl.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gahbocdjv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gibpdjjsb.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/grsitcxoa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/grdjdipvp.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gtowrhked.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gbhcjcnpk.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/ggslhuydr.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gzfrybwrx.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gyfufazwu.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gfxdtmtjp.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gjedvjnlc.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gachihxff.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gicnomooz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/glxsfqpwv.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gqbamnmbm.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gnpnenfcd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/goehgopyz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gsjiikouv.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gnaqugmep.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/ggwjhbfkf.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gzmxgqfix.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gxyygjedj.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gfcfhgqli.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gyqavsrmv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gxhbpbzbc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/guutdinjw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcncklfdt.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/ghqegwnll.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnsqafmzt.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gnmptuurf.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gcybbsktc.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gbugfxngq.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gzadnxzpk.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gmavokdmx.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gdegyvlfe.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gwomulbdp.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/ghvkswnyx.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gwjdocybw.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/goatqxfkz.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gwzwgqxal.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gxzwphgpq.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gbrbjgqcy.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/grkjvorai.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gkgwhtssi.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gxtaidssa.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gptcunsoz.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/grudoqgel.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gvfwowrpq.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gjmhzqhpg.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/ggnerbezp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gahxhyfga.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gvmpznpvd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ghrxqnwoo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gbkkqtxav.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/glnyyxlcy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gzqdwcqzq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gwhhgasqi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gbuesljhi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gwmnicoqm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gklbiqfuz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gnntbnmbo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gnwvwbfkg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gywninibk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gujruojme.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gafhzaebl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gewasiznr.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/geiwxcacc.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gslgibrht.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gtozbapcf.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/glbvoiytz.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gkeknrucv.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gcvbblfpn.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/ggonmowvv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gwuogdhyb.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gqfprjtfv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gswruezav.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gngxlbslb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gcxcynmwh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gymbyzsih.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/guxznmjop.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gpgpsufzq.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gjhpghwtn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjaujxrnw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gyoluuthp.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gyhrdtwuv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gotrkctnz.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gckleuzci.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/glrelgptj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gvujpbyei.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gbgylljea.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gskgsilwb.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gktsabrpp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gadnptkho.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/ggbxhwplg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/ghvoomhmc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gvalwngdv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gsmpcwjja.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gdzpholbl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/ggxjeeevt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gamepcmxi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gvfyfyhed.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gvmajisgz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gilhrmijm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gxyvbssln.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gpnhorkky.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gvtsohekq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gnvuqkqki.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gtkakcxmu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gmpkzrzaa.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/giloauges.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gjlbucmlp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvhfmjpky.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/ggkrngluc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gllqnhekm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gnpcdtghs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gfmcodmjq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdtcpknad.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gcioafjqx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gicvlebgv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ghwmcebti.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gpwzlsowb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gaibinpuj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gnlyvsavi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gusbzntip.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gcycmwgdq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gunxnqrdg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gorsasvlo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gclpbhrsa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gqulimdru.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbckopxip.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkssowzqs.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/glcogubik.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghjklyela.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gnlansfof.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gyaynqtms.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/goccqvont.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gjngffsjj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gslhmtbae.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gwpqsjqkc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/glcfngepf.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/grmvuxcot.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gxriixlvp.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gzopecoix.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gshirnckl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gxjvwfvvj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gukwftama.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ggnibntbs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gdgurnvzl.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gebqppwuc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gqpybgeca.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gegvbegap.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gvqhcmbiz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gspwdclbf.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gmlfhiboi.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gzfiibrnu.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gsaqjdpqo.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/glyhuuskt.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/ggcpfggdx.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gwmezfeot.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gsgfbeygc.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gvfljqldl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gfiutqchl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gbtxutcsb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gxmsiefve.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gxkvbypoj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gdvprzmst.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/goixgbbnz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrllsvjq.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gccwctnfp.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gcbsrwzdg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gfxbmqskd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gvfeqfpgy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gnuqzxuhl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gogczdwqz.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gpyokcfer.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gvrawuonx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gwmtnlvzq.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gljlurfrh.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gxnbqdugu.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gscobpdni.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gojsntynd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gklgwfdrv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gneefhkrc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gfavitibn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gfzqefsuw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gtwtcfklz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gzwwnarhq.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gxhhktwic.sHtML

Py:   str(42)
来源：http://www.share.zdbjq.cn/Article/details/gtaajiwrc.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gnlpsngnd.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gxvsjkgou.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gznkjbasn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gwkfmdwcd.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gqwbvepjm.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gqnvehxdc.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gjyqqdwnx.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/geqjdrrxe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gcffvsgvc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/glrxgxyot.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrtmeepz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gmabhjbhq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/grfkluawj.sHtML


<!-- 参考信息 -->