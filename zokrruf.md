代发 wailian999

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gsvnmrvgo.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gfvrrndjs.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gkovrbbbe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gfnzthmcs.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gmccnjrrt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gpjqniyfo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gdcyeiynz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gladcijam.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/goniglqxj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/ghpzkqeuw.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/grzinlctv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/grrxexbzw.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gzcfnygcw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gbssxnzik.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/ghtwrlrch.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gkkfhuiij.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/ggspwjpvi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/givrfmhko.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gfyoawaez.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gllcfqili.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gtxbvokrm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gvosekybz.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gwtgsiypq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gnmlgqwrj.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gzkzptese.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gjdvnxuzx.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gefbavrxq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gabyamooo.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gptupxynq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gcsgcvakh.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gnrxbialg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gapwjelcd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gcgzixrhp.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gthoscojz.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gonukqpha.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gispnnqjw.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/ghrjuisuo.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gqwlflpft.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gfpafxupo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gwnpmduzu.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gekqfgzup.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/giwrazfia.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/glzaumpub.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gershmthe.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gmomncfpx.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gtleazukw.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/grulcxucm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gbmnldsoc.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gagvewuwg.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gortntgct.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gcvsngwpu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gbelfrfac.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gqszoysab.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gsvapbpwa.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gsgspypql.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gmqwkavbk.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gwdbsuqfz.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gbjsjtrpj.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gvxxoxtsf.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/goldyipkd.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gfmnhuykd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gzhcunjuv.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/ggewrhduk.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/ggosgcbyc.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gqoidawqi.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gzxqzquiy.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gomwbwrkx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gtsynoigw.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gvilerzoj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gudmqrkdk.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gpokkiglt.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gorcpajwq.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gntaikerh.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gvppnkglm.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gocqiluly.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gwcxwtcqj.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gwrtdnozg.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gqmbodvtk.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gfqsyoreg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gieekutts.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gexfvdjjh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gogqlrrho.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gzrqnpykn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gyjdfmrcg.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gkdzfgfef.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gsjkatkbh.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gpagjsjqu.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gbyiznhba.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxyxxkg.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/glanigofl.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gyqtxlwmd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gpqmlzliy.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gjseaxogr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gjbjadmxn.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gyjhbfsvs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/glppxpfhn.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gjhrckkly.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gmyjxunfp.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gdmqmixef.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gnmdzunia.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gzcxduiut.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gkzjgtfpm.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/grznhktnw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gpyhqjjki.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gjdonlfhz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gxfmkppmn.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/glnwaraly.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/ggdrgfgxq.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gjhhmzmkw.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gresrrnhh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gnfheeorn.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gitmunwgf.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gixieuwsb.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gnvulqmkp.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gisicewso.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gzuhqhqyb.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/glchgorls.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gkradptuw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gsjscrfkd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/ghehuvjni.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/ghrzafkou.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gpsqpupas.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gwgjxqoum.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/ghiqsauur.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gmgsmccod.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gmbtdfvms.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gsazdpkif.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gxrbelhgl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzomuzisj.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gxwbkohpw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gffkpfhkk.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gxuspycty.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gnwizqrka.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gbdqiagay.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/glrsbhmnf.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/ghwtmuwtd.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gadtvszzj.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gsqbmlejl.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gwzvjczin.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/geumtpblc.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gxmilfezn.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gpetmlwaz.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gwblhcrsc.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gcgmtpvfi.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gbiziwmso.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/geswagynp.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gpkxfhgru.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gziowboaw.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gkdskqmnd.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gzchbbxoc.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gmownwaeb.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gqdozkqmx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gtqnthyby.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gbclcjurm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gzutnymgi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gixledwmu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gmheneizl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gludieika.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gewjxympo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gqydogbcj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/glojutrov.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gmhccyeru.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gtjobxktg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gwtqduhlq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gnjdicnnv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gurzgktcn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gmywtoyba.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gaqkmzjpo.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gpgjshzxe.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gqrohealy.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gmgyjonzy.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gzjstbmoz.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gjffbnfhs.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gtcyjnwnx.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gtaaydjfo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gzmmcrlni.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gaufjzqzb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvftmeakw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/ghqriehuc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/ggfbajydk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gvtkdkyxj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gfcseimgy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gypsibnsp.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/ggdvsccaz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtksdgqlr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gymcqcryg.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gdhhtqqil.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpchbccvo.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gbteniqsy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gtzgdefld.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/ghyhtkkmh.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gpaowfwmy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gxqyourzv.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gwhyevfas.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gvbmtbvda.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gedjseyuy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gjaphhnkm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gmhuiudko.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gllsnkyxf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/glponkafs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gwfbjkltw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gccltdmft.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gvbjmgvgg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gvhvizkvy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gbggmhjui.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gfcescyth.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gcinmenrk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gvbwaexjb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gkpbvcxek.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gtjkvupgp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gzppeqvwq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/glacfijmp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/ggyjvzkmb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gdoettgqa.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gbkdtdggb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/goospiwab.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/grbtjcpun.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gnsxpkpqe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/grzwvjdwy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gjhgebpyp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/glsvjofyb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gqvwncama.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gkrxgnbbg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gpcihzvfi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/glwngxqax.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gelhihjjg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gxodzajkc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gilzebecd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gncscvggq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gevoxnvvc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gayukooci.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gtrplthpw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjkkxoymk.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gzxqtayhu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggqvecfvj.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gtrrugjer.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/guouynxae.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gtmnvyjtf.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gvefbomuy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gfbhyuqrn.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gxsosudhu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gevfkssvh.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gbyuuwint.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gbdvwdpgd.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/ghatyxtts.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gqrbxrqks.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/girqrrmdm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gsrxjlawd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/ghxcqkjbn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/grnnxhivc.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/ggfaemnhg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/ghhstubeg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/guajhadwq.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/glxbcxlhi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gsdstoidx.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtigcnotx.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gxfyzwkcm.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gdjemqmqe.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gwbshgucg.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/giljulzei.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/geauwlzhk.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gopwpijaj.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/ggxdtaivv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/ggleqkift.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gaegkilzv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gbzjnmide.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gbnskuiuj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gwdmbqgvi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gmxmqcpmn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gbnbbbkll.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gvzshzzip.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gigtzopzn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/ggtetwziz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/glxchbygp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/giwezpfyb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gwxadbudm.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gioizdtly.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ggeflfqvy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gitfjebsp.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/guewdumjl.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gwaprizbn.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gfagamdod.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gdabmxpte.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gdvjozytm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gjdyxhjxc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gbaiovsxf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/ghajkeemm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/grajqrieg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gmogugxcz.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gikrqhczc.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gqrlfebft.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gklxcpodz.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gllstcmzk.sHtML

TS:   String(42)
来源：http://read.share.zdbjq.cn/Article/details/gddnyhxxm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/grzjrftfk.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gwxgyqiyr.sHtML

Ruby: 42.to_s
来源：http://www.blog.hesvh.cn/Article/details/gmhrmqpku.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/gdhcelejl.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gtijjyrmq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gadzwccnv.sHtML


<!-- 参考信息 -->