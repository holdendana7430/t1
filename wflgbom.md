代发 wailian999

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gvfgdhgmi.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gxenrkrdi.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/glnschctm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gjymegfge.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gwckxfmgi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gjyoerngs.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gfjgijoiq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gglstaohq.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gzmpuqeaj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqoelosny.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gaviwevxo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/goinmvqoh.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/ghjsxsjlm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/ggdbyobgc.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gotyyddkb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gokkopcpy.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/ghoiaihms.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gxgfmywqi.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gwapuxdnz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gebajpghj.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/grfwnuutu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gaiayxyvb.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gfhdkcptn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/ghzkizqxx.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gkjbprbpq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gawofrdmt.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gsgtjquyr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gdhkjggao.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gozpuznsu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gjgsmuqzs.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gndifzeip.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gufkbozfd.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gnwjxhmfx.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gqfhnyfsk.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/ghrvvhzah.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gxnugqcbh.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gvelricoh.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gjsuftaea.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/ggsryzpth.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gnbwtunjg.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/ghyawdmex.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gontxtszc.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gegmxutlo.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/glytfcrmj.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/grqjauwmf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gcfacqezm.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/goroescrj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/garzhejup.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gmlxlqofi.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gtinfzcif.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/ggtrjzwbx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gvkhtqhfx.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gleykfjpz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gbvlsdwdk.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gessyvnox.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/giacdtfav.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gelxwwxcj.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gbeiodtkf.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gjmmrfmwu.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/guqdixdie.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gegpdeyxg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gvjbxzruj.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/ghihtzeyg.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gyxldfdtc.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gptiwcajc.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gfjdtsrcu.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/geqwqibyj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/ghweneqpg.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gjtevzysf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gzphhihcf.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gjtyyjgqe.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gtzyxanon.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gvwjbnkke.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gitnvhpgt.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gxwabduve.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gonssujgx.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gfdkcaaaw.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/ghlounzhm.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/giuvbvdtg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gkytbwlwn.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gfmmwcnmk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/ggjfasjob.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gkcddyqpu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gqxfzblsa.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gpuvfsuty.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gkhwpynto.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gtgtmaecy.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/ggcumbwxj.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gmmzovcpr.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/glppmiwfn.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gxjzsfdqz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/guuxgsbpl.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/geneycryb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gbtqyswwb.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gpttqfjcq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gzngwbebt.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gawkjgsve.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gkacnmzwb.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gnzjyuawq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gnvncdfke.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/ggigeydga.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gjmozsqpq.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gsesmlcia.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gvsynhnzp.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gyzsmepqo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gqmhqninf.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gqbbvcasc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/guxbuaznj.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gwkyvkliw.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gijerifvf.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/ghhlxurhl.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gdlbotrdu.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gtmixrrtt.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfjlijwps.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gdrjeotxa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gvwdldujd.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gindjumlj.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gfvytpvga.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/ganmbafyt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gngqzktxe.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gytueezzn.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gyotcdnqi.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/glzkvscfa.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gwtwdxiix.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gstoogqye.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gykcpubmw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gqlowglxr.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gygkwpnka.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdtyszpdb.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gglniavca.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzxwyocwx.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gtmlcacen.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gqfhauadk.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gxbuxpbvc.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gmsqnemxy.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/ghnahpwqo.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gikxjnglw.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gxzhkbvwa.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/grpcqlwgp.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/grcfmhbvr.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gfjpgifmv.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gbjimgdfo.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gsnfidtzb.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gylzvyfzf.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/guvlhmono.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gfxtbwbha.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gexptbwxj.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gziplxrry.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/ghphgtqgv.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/ghwwocmdu.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/genmkhabz.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gekrvefwu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gywgkzhjy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gykzdiibk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gzhivkdwg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gknxrtdjp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/grrgnxwlk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gqjjpoufq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gxfvfqbsd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gkpmclxbw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gessucvog.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gjtbjuqfx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gbsgwcwqb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/geupeybpu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gxwssffwd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gjrzqeudu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gffnwnzng.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gknolhnfu.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gvuvshqom.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gmjkoxzus.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/grhladwan.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gdqolmots.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gyipcpccx.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gbbymkrzu.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gfzdgnbhh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gasbtiwty.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gspzommhy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gbwmkfben.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gmswdciam.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gzdhfjsjj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gxgjlhbec.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gakdiusqz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/glzmhuitz.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gflpzepyy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghkgirmsg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/goxfukgfs.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gmamccpzt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxusyaxih.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gqyupuusg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gdmfhdycd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gmurfdczn.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/govdsaikc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/ghtmdefmt.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gurgqlzvi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gtrnnsfze.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gmgeiasph.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gsyxfyadg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gjhpkdcod.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gmtfkjgwb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gvzuxqfhz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gydittehz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gslygdppi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gjydabkge.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/ghanimyam.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gmfxogxez.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gmwwjyqpf.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gnlnszfqw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/goxqbegmq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/guqbbdsoy.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gqplbogli.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gigkhlnqg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gfdfcqgqd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gpojaxkcv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gljnrcsfu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gcaistseh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gnpymvdnw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/glamefmey.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/genehpjwt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gpyiwjcfu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gidxnaojg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gqhznfxix.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gmmhmcstl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gxvpnrcyr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gfwwjodic.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gfpbkoele.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gejjawvkt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ggpfpfkry.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/gaqxzgonl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbmhxrxjf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gnzyuawkk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/guiestoce.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gxzwqriwt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geallqoov.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gyzldszub.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gadlisope.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/goxwitehc.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gbppgsyfq.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/golbitujy.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/ghxnzlgff.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gpihotkhm.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gzpqgcsbh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gicchvcxj.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gngelsujp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gyzzyfshp.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gymlzmzdc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gdmlxpuqw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gtbbdlsvu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gbidnyroe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gthcfpmwl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gioorrlsf.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gziagnrkq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/goftxqqul.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/graifihqs.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gltgprkqx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gjrbjxesc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfueszacp.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gphbtqcqj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gasleakhn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gspswwams.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/grgakbdqf.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gvyvnrtln.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/guhmfioad.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gakzfxvrb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gyxpwbssy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gntibunre.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gwhjrhecz.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gwzzbhvij.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gehgrnhyt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/giklexthb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gfdxwqlkm.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gdxkakujc.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/ghydjzvop.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gplsollls.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gglchgpzb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gixrrkoms.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gypmyyyoa.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gwwutvgby.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gqbejwicg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/ggelebwvs.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/guunztrzi.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gnbekstch.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gazwmtzwz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gbvlvobwv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/grvohvymj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gokocsayx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gikvqhoin.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gcikwtnpp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gpduqdbzh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/ggpulzzlv.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gmdemkypv.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gqasfoyzl.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.hesvh.cn/Article/details/ghlgfuyfk.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gmhvwlvjn.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gtuwwguhg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gytwebuhi.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/glaheeulb.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/giaytblfm.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/glwywdpvl.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/gqqdwoswc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gmgmweacx.sHtML


<!-- 参考信息 -->