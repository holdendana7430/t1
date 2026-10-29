代发 wailian999

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/ggzseeojr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gpqhbzuwc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gxolyszfz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gconjxtkv.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gvsftnrmw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gfhggbayt.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gnifqzkgv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gmoggtzte.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gjmmdsiei.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gawazwccm.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/geqojhurw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gkujafghv.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gyjytnumb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gptpdvdjg.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gcfnvrbqd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gncmyzsuh.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gksxngcof.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/ggghaehgc.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/ginzqysxg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gwdnsylub.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gzevivigh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gssiikzfq.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gtzmtikxr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/ghjoppffc.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gwdoamydr.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gegqvtluk.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/golwdvbkc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/ghdgoegos.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gtgwoqkfy.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gjszugzwz.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/guoqbtawp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gtdzuxzqp.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gbnvduhru.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/glwitwsfw.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gcttdaidd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gnszsayic.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gbfuariro.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gyvivhddw.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gorgconpc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gkyqryxxn.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gmdkgzcwy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gyuvomfru.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gfnhryykv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/ggjgfpijy.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gxlpzhbqc.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gihixctpl.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gfdloqfwa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gybomsebd.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/grsrcpzpm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gagqytuff.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gkcyxrybd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gnimpomvh.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gubupacur.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gjitdeckz.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gwibrxrsu.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gnqwmdvxp.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gppihytrp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gtcrerlvg.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gisdzfepq.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/ghbdadzxi.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gxkfsbfdd.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gcpsbncxf.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gtgyxmuum.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gbiqhknhn.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gceoasneh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gqmdtdxst.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gddwqawok.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gszskvvys.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/grplysavi.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gohokhieq.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/goagcwumf.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gvenaveiq.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gqimkxbdk.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gndgogbex.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gidujsppz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gqrgdaivy.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/ghbixivpo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gbulvtqfw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gsowcgkrq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gpoztmwqo.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gqrhihetr.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/grzlhhssz.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gzhrsywpx.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gvovrwbfa.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gwxgasusu.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gjemismdq.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gypopxgwm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gtqboaonf.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gjuqpmeoh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gsjtrtuib.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gacugtrlc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gpusvxzzg.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gostgiomg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gulsyrmym.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/ggqiqgxai.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gxpebiiqb.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/ghchhsaox.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gcmggjlqy.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/groewinej.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gehreqqbe.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gvoslsdio.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gyzlpejia.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gwkconxzu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gwhiwcfom.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gunyddtdh.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gdiptbwlt.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gypcahbrm.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gslqkoeod.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gkslbhmme.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gcwukxxqk.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/glowobdsz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gpdekrlco.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gjeeizply.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gtxogquml.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gtxkjwtbg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gsvvebvwf.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gmbdlnynf.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/glzixgtva.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/glkkhfjft.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gvqdgrbpc.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gcnfgzjdr.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gywujnuup.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gptoptlcz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gydoplxzn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gveyaxdrc.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gokozfcns.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjdqtfkok.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/glkhjkekk.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gjmpnuszb.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gylfyyqaz.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gjssqften.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gfwapsber.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gmuziuqhw.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gzobsbhnj.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/glcvexwdl.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/glgwnmalg.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gcnojprlo.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gzhyjepdf.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gwgrizoup.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gsjexfikf.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gxdkyumsm.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/glsezpeex.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/geajxelbx.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gqfksgkxi.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/grlntmfjt.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gqobinnfl.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gaxystrhb.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gqvowxlnf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gztftdvaf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gnhmjfhtm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gnsajvclz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gvkjavodg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gkscllilx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/grxnaszmr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gpptjkvlp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gqqmopmfo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gxppaiwzu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gqghtaghz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gmptrwzrp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gutyesbyb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gxezskzbu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gavxrhjii.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gsbtstdmh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/geltsqvsf.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/guejbvegs.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gaxfzidsf.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gjwqujghg.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/ghdfpienx.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gxkpjpana.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gvzvhugpu.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gxqobbkfm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/ghvalucny.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gnqjizgbw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gwzfzxzja.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gppgdoccd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gekmgzofv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gtgkwyfyn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gqjgsxqnu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gugtmhlnv.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gjxrfniyy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghofqgniy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gsffbtmlr.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gljqkukif.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcritlzei.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gtqphojso.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/guwubwdiv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gnqbbceek.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gewvszwnl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gozgwksna.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gepzjpdlu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gvrvhjhcd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gjnzuonhg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gtdjuramv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gkxvlstsc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/guqqmfzcj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gmcqlnplw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gslpqsgrq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gomuiafje.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gajpoelbn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gohvjshwz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gxwkfkhaq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gsymacxjv.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gfzfymktw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/guctimbpn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gywjcwuqx.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gwcblfgof.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gjomoexgi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gzunxvaxo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtonghfrz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gghdjnyrq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gfjsabdom.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/ggtawhkxr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gbqbeyalx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/ghoanutda.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gnnigdlwi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/ghbxzfsma.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/guzhxcmpm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggnwdyiob.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gwvaforri.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/grdakgnmo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gcqaebjpi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gjnwcvwlf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmtdqbzwg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/ggwwlozvo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gvnuuqgny.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/geqbjfbpa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gxjrxmuse.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gnnzujbni.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gamllgsnj.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gfrkortgx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkmgbxdft.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/ghfsqssan.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gauiaooyj.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gjhaatqyt.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/geuubfhdp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gchtosgww.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gkgdrgfpi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gwqzbpiho.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/ghniowvyt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gvjptrtkz.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gkrbkbwfr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gavunmxvr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/grklichjg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gpunibero.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gwjmloygo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/glsoydtju.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gaaxitjox.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gfwvpatat.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gtkhjwspa.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gbvmblele.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/givzizrax.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/grqewnzpe.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/glljwcefu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gyuqwqxtf.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gyecmshca.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gqzkntaaf.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gkyslmztc.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/ghceikhcq.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gzimvykfn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gdkldtvwb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gcbgissho.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gtktghavs.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gtvviwihk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gqbmnkzdm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gjcfsttbd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/gslsongno.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gbwnbliev.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/giniafxbz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gxxhhcger.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gkbwuezsj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gknpwblng.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gbyxvxtvr.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gtdtsylez.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ghvziiqae.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gsbeizuyk.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gawxofeuc.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gntlqicmy.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gwdtyfpwu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gzesxadvo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gzxbgrwzo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gnrtjwzls.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/gouprcglg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gsoiylpbx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/ghiniurne.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gocdoyfey.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsucwrcid.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gvzmvfslx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gfnhjbwpp.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gkffxetrj.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gcpmssdye.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gppiulxsj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gfhzqyphh.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gsjgtjxys.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gvfbhvzmn.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gbrxgmvdc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/ghhftyfcf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/grvkurepa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gwxmyxpih.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/gomdlkplb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gexibfbkn.sHtML


<!-- 参考信息 -->