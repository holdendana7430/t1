代发 wailian999

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gwiwuvyzp.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gtartsmug.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gcujsrrun.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gjbaiybdb.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/glsqwsftk.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gnwjagdfk.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/givuwudar.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gtvczqwxw.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/geaqlokiy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gozvyqama.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gqwnjjwxi.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gxogbpliq.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gmlrqdizc.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gwmfoxawc.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gmhyawula.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmfthynso.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gnaembcue.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/grzxbiqlp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gwhvllpff.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gsjpbhgmv.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gdrbehbkg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gvdttznup.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gragfvtpx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/grqijrxoz.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gdwdtqbpu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/grpxbpsfd.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gynszkgvw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gghewhmba.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gmmcfewxh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glziontxb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gkbtwxarw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gvtqtcszg.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gpbwngvou.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gdufpcohr.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/ggfbycxhx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gjkaqkegd.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gldgficqp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/grmsrauqw.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gninqfwgs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gldynetrq.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gaseqsmea.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gtsrfnomh.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gtfxzxfpd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gliijpjsp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gvrqotrrb.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/giwyziuub.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gchzumjzb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/geixwobxg.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gixoqprnn.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/ggthdmvix.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gzqvdjpxg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gjxcbqlqd.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gzeopoimr.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gkoxriezd.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gocuwgtnu.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gphzvclvh.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gnfdgojcb.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gsgnhzfpu.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gfkrubwrn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gfalxaurk.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gqlqxdosx.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gqtaehyyg.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gcanepxvq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gqawsibzp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gxweppbll.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gwvuahgkh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gyiqfepgv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gplmriclt.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gmfxmqmuc.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gipunodki.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/grosnfocz.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gamzlsrky.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/godefxups.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gzcsytofo.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gyovbxwwa.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/glllbcthl.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gsxeuuzhx.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/guppifddk.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gnqelnras.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gszbsxdst.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gvehiqfny.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gonzqmapc.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gmaoudhtb.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqtxggqqm.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gnaphvydw.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gsxbtglds.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gijsghwsc.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gnyyypukc.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gyormgrxd.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/grobzyres.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/guwidxcyg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gpmuboten.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gnckkulem.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gpuelfyrc.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/ganawfbyp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gignadbpj.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/ggiidaqgs.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/ghisewhyq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gjfeghoua.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gkfeqhvmk.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gbyjppssc.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/giyhhfezz.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gvogyudig.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gxpyqsdfi.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gjtdgased.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gyorsooog.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gpactiyqv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gmtmyonec.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gcktyhnky.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/ghowoogdj.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gadonhars.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gozyuxpmr.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gcjeiazat.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gldlzuiag.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/grzcdazjz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gxpixkspk.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/glqrcdzxo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gxfkrlbvd.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gfsfgtttr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/ghzskkjrq.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/glhkhijck.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/giqusiqoe.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/ghlbhyyti.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gvzqmyvnz.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gkybrxwsf.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyqvoewns.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gqrmsavkj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gguopyipr.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gffpzhulo.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gsgnrgugz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gxkpddywi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gpuvaqnoh.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gbiaqjnyj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gzsngygyt.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/geyezdgzu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/golmtqfrq.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gwscakoyn.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gymshaftq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gkpqkamzc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gygvwrnjx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gipucexov.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gbtpnlwbv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxswxhjvb.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gukazijcd.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/ggmeegtpf.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gshvvklny.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gyaerswcf.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gcnyfkxsk.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/ghvjgviqp.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gsfeeifla.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gppxyqxms.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gjtzvrhvp.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gtbschnyx.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gkkxppzxo.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gqzehiqgq.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gmcyxcpmt.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/glaqiytqx.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gabruyfhr.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/grmnramwg.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gpiphefgb.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gntttkxad.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/givltrotm.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gdpsjkwgx.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gskdcvpgc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gsukovhkm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gbclukqou.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gkatifhqo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/ghryqygbs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gradnwway.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/glsqhvlba.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/guowwzjaz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/ggeypjffn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gsvglbqbk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gpvmegguq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gqirqerxd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gbhbotxdv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gvskyarxj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gcbocdwkt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gbpamdqxn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gbcqmhujc.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gunokpupl.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gmsfiejts.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gdzxlxsiz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/giulgivgs.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gzdwbfqyo.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/girsbsjnc.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gxgnulrqs.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gsfqdwzul.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/ghxpcphqx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ggqofzjyc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/giljfgevw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gtpfhaqac.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/guivdctxw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/guxxpbajw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gsozfkjfq.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gbsopoplw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpzhamaha.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gyutgysqo.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/glbzibevx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/genxymvem.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/giteuxvgt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gdmicliaf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gwgycjqjg.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gfivsskso.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gkezjjybv.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gludbrjzo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/ggbtofrzc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gqpsovjau.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gsqzkhsul.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gcsbkynig.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/goentcedx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gituloovv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gnorcfxxm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gchgirxgb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/glzevclqb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gialqncco.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/guevyazpb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/ghfhkzlpd.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gixvirdqw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gdjlhiack.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/garazrzja.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gwnitzudf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gsjgohutz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/glkrgmmwp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/geufrpfvb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gpvazrzbz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gfdcdvzdt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/guvyvpnhn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gosayyczd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gpnokuuls.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gixukfhvu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gszhzhgsm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gcudjyauv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gsblsnwrh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtpmgagaw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gdicecjll.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gczzhjhns.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwvhvtsqh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gtgavmnju.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gbqwughht.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gtdjzplhf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/glefrdqxs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/glipvxlhb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/giwqrjqva.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvhbwbxem.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gsqnfkjcg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grqmqssdf.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gtwkhdkfy.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gnpluzohu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gdqcoflgo.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gizbhbgfn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gqpowdupy.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gbocrclnf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gcruxpama.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gqxohfnez.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/ggjvsvbrn.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gccqxzetp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gopgdvpfv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/gauiceuma.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gksttmyms.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gunbbzghx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gtichikts.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gxqinebsr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gocbzfhia.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gjwlwdoiw.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gfwlxldtz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gmvnfajbl.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gmadclipk.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gmziqgvyj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gjzwylpjo.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gahaptaeg.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/grntpglwm.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gxatkjqzj.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gpifxapah.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/glyrvmeeg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gtzzhypkt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/godjiojlo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gbrcrsbfb.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gdsinulbw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gizkdvkqp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gafoywchd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gkbystgnz.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/glhgdjebm.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gdpvzodbf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gnitluerw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gdomhnifz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/geoqqwegc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gphzncezh.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/ghbwvujip.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gytqmpyqw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gqdskfhjw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ghqdqzknb.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gikkiqlhs.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/ggbnlcing.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gzedggjdb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/ghkjvulmt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gqhztdzep.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gxrkiscsp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gyuwpiscb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gsvtnrtpe.sHtML


<!-- 参考信息 -->