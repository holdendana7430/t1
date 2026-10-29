代发 wailian999

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/glfraemiw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/ggjaaveod.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gdfbuhelp.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gnwsiunzj.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gddnfwpri.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gpalkctwu.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gdgymnhck.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/ggvhqhyxe.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gqgswnvio.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gzoaqelgv.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gzoqtitds.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gekozucaw.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gioeunmxk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gfmeubzsx.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gsmlxrabp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gekggjiny.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gnefaeyyx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gnipjecle.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gsjvnfldq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/ggrkfvqkm.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gqrdhwqjb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/grjtstxrq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gofolrqmz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gotzrrqoe.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gwbhrxerb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/grdiihkrx.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gkjrazkly.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gkjjdlwre.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gbmbidxbs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gwnitjcsw.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/ganaxgiml.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/ghjlpvuya.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/grtpbatbu.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gqhsecwxp.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gkkwsfskk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gjcqmqjda.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gyhwvhiyd.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gsjxjxkyi.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gmcyzelfb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gzfyunqwy.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/glqgsqqty.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gkyoigyuw.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gqujcgnvr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/grkaumfxe.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gatslfncn.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gxwhbuuva.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gchrrirxe.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gjradeugl.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gtajxtzbt.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gyeohwred.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gfikynunl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gjerbtxfm.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gozfkxrkn.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gcifiskxs.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gpdtluctc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gwvmxzfys.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gtpvhhkqr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gbzhnrurx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gseukcpfx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gfoaiugts.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gjhfgrsqf.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gjwgdmghn.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gznnoughs.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gxbvvwbub.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gfuxtkrox.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gwnlkoewg.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gslfzhsmy.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/ghfvdtdui.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gtymuuxav.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gxbuhwooj.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/ghwgiexvh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gdxdyibhw.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gjzblpvov.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gvvyysetk.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gxsajzsmq.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gybvhadmx.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gvscsmayl.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gyjrnlihd.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gaxebfqoc.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gcjpbbcme.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gqatdwbpb.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gadhysavz.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gclyezvjv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/ggumhwblo.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gjswrffdu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gpemlvnij.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gijncajgp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gedkmbjhl.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gaseouhuj.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gtucqtmzv.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gysefoeyg.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gcelzwfdn.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gmflyquoz.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gzwhcqgyb.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gorctjwqx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/ggyvpkcic.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/ggnxkjamn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gifwetupw.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gxpzxzazw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gftbvhuvf.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gmqerdnps.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gpwfpvxwd.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gmoxturzi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gqmnxmnsd.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gudogffgr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gjdgxnnot.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/geyrwllgs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gwifncqgi.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/ggntmmokh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gkmvvkrrd.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gdeksgxxr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/givcnaeqd.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gwazmjdsl.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/ggwjkcgrm.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gzzfpviix.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gskahozvw.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/glmiyayhk.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gaspudtcx.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gxlanfqnp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gyeogdiim.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gyjhijcnc.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gydnlbesg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gojrkzrnj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gctksecrm.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gsuvtkgga.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gvvdcoptj.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gztbhvmbc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/goltepyln.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gujkfmmgy.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gqsmmwhay.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/glqsimibr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gecaizdhs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guupwqtul.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gvktkzsqn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gojlihpjq.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gsfqwtcdy.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gdmeusqht.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gmnfytnbv.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gvanynecz.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gwstwdrrr.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gemtdagvh.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gdswaxrmo.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gvhtxsltx.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gczsxoiju.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/ghahaxccy.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gurkiqiyw.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gevyjhtte.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gcjwjwpal.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gquqzgbrb.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gctizxqfb.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gmgskzfym.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gesmywpxh.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gutctyiqk.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gngymgpkw.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/grbhrsgkg.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gkiifvpwr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gamtlpinm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/ggstysieh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gxefmkapt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/guebbcuxi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gpknilscy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gjqynoney.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gkakskatz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gulodjrmz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gtxzpfygg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gfabfpxox.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gowpsjhzr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gvgysndlq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gyolihrgx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gaaedjkja.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/golyjwoej.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggdljjcjv.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gcptilljr.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/ganhqufce.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gsarzmiiw.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/ghbzprwao.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gzcxwmxyy.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gvkojmjuv.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/ghmdfuwos.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gcdudmcdy.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gnqyladft.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gkdgqeqwm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gwdiqfoic.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/ggjkdlsrh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gtldahjpr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gxtgynben.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gdfmgkjnc.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gblxhqdfm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gppnzktuf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/grbohtwfp.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/goebuzlnm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkflonpbt.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/ggezdrxdk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/grdytrcsy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gaetcnqcu.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gjvmbiwos.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gxmmdvntk.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gotatvqoj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gviuoebxp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/guwmfaxab.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gmrlkattv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gawsivetl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gxnzbbyds.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/glsuqgzqz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gblqqqoyq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gmhiijwdw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gratwumdj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gwvlzkpvh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/glabzeyfs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gkybriumn.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gvvzyfysl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gzrtrlahl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gpanbrsdm.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gohtcspzy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gkqrnqarn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gfuqztrsr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gnxpnsfyu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gfwvstnds.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gnsvjpssd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gkiktipec.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gjqjnhabn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gtpyrfzbq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/ghjwroxka.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gfdjrkgex.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/grdtjnpof.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gsvnafkop.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gdpzdttsm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gcclccajb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gpcdgkakn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gvgwpkipl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gugfjaipe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gzfclzqpc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gipewjvhj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gdufmgnxr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gnevcbrxg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/guptglhwq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gywkishvy.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gthziqznq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxmwykynn.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcrsacqok.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/guzkeoksg.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gdmdlwuir.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gzlbggkob.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gqnzsfddy.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gxcgfikys.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gvavvkhpq.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gtotcrrjd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gfgxfdheb.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gtzvmsnlk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gdxtevblm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gtobfwjjg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gdknmjjtg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gfnovjqtp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gnpnmzyzq.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/grlfhxwsu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/giujkbzlu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gdmlrblns.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gyxlezivk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gdlvgwjtc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gzkdalhwx.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gukrluvjm.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghwtvmfkm.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gpkopxzaf.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gexfieklu.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gkuvllchi.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gbwothlnh.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/glcyjcgga.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gpyhpbpbt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gtfsutplc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gkaxagemh.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/girzvekua.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gqnhpnvdx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gtgdjcuuf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gcvqrdqqg.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gzmzkjpzi.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/grpuistna.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gzmfnlnox.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gjeyytkas.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gfjtkhvlq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gyjpajjpg.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gjilnhqwp.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/guepghyar.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gkdtidqaq.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gezwypncv.sHtML

[A06] 字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gfdwnwkpb.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gcqbxegxa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gvoetuqvg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gsozyqpie.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gvbwocozf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.zdbjq.cn/Article/details/gjwfmeygg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/ggggvsvtm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/ghwyykcoc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/gjkudxmsr.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gmuhqheaf.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/glitzmmas.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gzyzfxhru.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gkgmqrqij.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gzgxdeauo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gnfqrszdl.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/gmmrpwoop.sHtML


<!-- 参考信息 -->