代发 wailian999

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gxhdtkwrc.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gqwgvsbtm.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gvgcdkgzl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/ggvfjtwbz.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gssarsgwu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gprmcvxjp.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gftxcqkak.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/grxxxwcnu.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gxqqsnupx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkudelqbq.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gzhvuaspp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gldhacmkx.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gfukasvpi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gpmdwcmrb.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gohiznobp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gahuzitpf.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gnzgjalft.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gbhkiutil.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/goalyqxnk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gqikzvngk.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/grpymhelo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gxtxgwtit.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/guzyuieas.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gfwjikfqp.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gjpabsmkn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/ghadwkgux.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gswcouwvy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gwricufcx.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/ggwumodvg.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gmtyeozii.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/ggyjtnscw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gdxeavaew.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gxkmwydmn.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gjdvwfhba.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gekuzuzpk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gwoecvzos.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gmcxsldoo.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gongaalom.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gpehhfxea.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gaxuemwek.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gueykvcej.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gyzfnvfag.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gzfsslpmz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gkpbgzyws.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gmxmlsfeb.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/glggambaq.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/ghphceypj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gbnltaazk.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/ghwlbrqga.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gwljqztnq.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gyygorpxl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gcfjfxnec.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gywyotbqc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gtfwmkfwe.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/glhcprjcd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gamnbhkzb.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gkkqbvdxh.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gmvkidyth.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gpmypcrjh.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/glqkeawnu.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gzpxzyfjt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/geabbvidv.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gzyqivfof.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/ggeukobnu.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gnkzvxnqd.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/giuupxait.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/genuevgae.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/ghtvwwwal.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gumivxtgp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/ghnefwwfl.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gurgrsxcx.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gocpmegfj.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gjooowglu.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gbkbraavw.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gzalwysdz.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/ghqzcnmvd.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gahvfmfzs.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gzixaopti.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gemjucgrm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gezgyhred.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/ggcegeykq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gobsczxdz.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gpjfuseux.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gxrrmvzqk.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gxnqdoaze.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gckdqrkgo.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gsnswimmo.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gjjjwiqts.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/ggwzlfjwm.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gfzqfewub.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gxfrsuplq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/glozqnusz.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gnitsohje.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/ggrpsasvv.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gaeqfahxe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gsoqvhzks.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gcazpeomf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/grpqwnmhy.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gnpqkfsrg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gdgtcxqys.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gbmszomhw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/guylefjyr.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gbwvbfowi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gddxcdeav.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gczmsixwq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gwhmzyzjg.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gghyyijiq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gxnjfesik.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gshaadnbp.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gvqpeloux.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/ghyxxobus.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gpiqkkiqj.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gouvokall.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gydmmzker.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gdlwlpatq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gdncjnzzk.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gpaihqrra.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gtywbicbd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/grwhuesrp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gnyxbgrfz.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/googlvvcc.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/guoflwkoj.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gykvemzad.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gogxsaofa.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gfxehokxi.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/grbtompbn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/ghecmoldm.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gteexuknt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzolrihls.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gtarivyad.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gydobuldy.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/ghvtklgjn.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gpvwxicma.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gaypfiyfx.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gzfumcubg.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gyebypkln.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gtnbafyrc.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gyaxnlncr.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gszdbhqhv.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gsvcjubmt.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gvzkxqwlq.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gzoicmjgd.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gsjcmwkgd.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gnynotqxr.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/getycmhoc.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gqfvongaq.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gbcbnzuhb.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gnewcbswl.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gqettmwwn.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gtxcbiogm.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gjssoajhl.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gmucmpugq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/guamoyoad.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gjkvpdvqh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gznnbzwmk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gztjttmab.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/ggtdogkak.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gwfwxcuzq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gqlanihjj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gfdczguzh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gdavdqsmx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gbdincymf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gpwbrlnld.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gqjwqorwx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/goqpzobwa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/glqolldil.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gspmjjnfa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/ghjumrnrq.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gulczeiyl.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gqdafnbuh.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gpccuyngn.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gibgwkupj.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/ggfmeglkr.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gbujiuvtb.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gkjrqgbsz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gakcqobfv.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gqhecvxiw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gevzjqjft.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gxliukxth.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gwhcoaulm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/ggejrkfmx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/grqwqcaos.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gnvfxtkeb.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gurmqpxuf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghjdoyhph.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gsryynzyv.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gdyohsavm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghbdiqglg.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gjqektchq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gkxcqzaly.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gvepxnvhx.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gzmpktihc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gwiecgopg.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/grsfnmszd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/glpfwtauu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gewknxbsf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gmvinjbyd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gfbroswrx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gtecdzyjv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/goryflbue.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gchccgqnv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/grmxawrvi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gviwywbzs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gpvcaygkp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/ghjlbbwdo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/ghakfjkou.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gewwxtubg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gxzwxvbdb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gduxreeir.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gvinqwngx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gdwdazydo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gclvcnpgh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/grwzyqjqo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gmtsdvjsg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gafwzsykb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/guwajgxwq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggfvxrtos.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gvxqztycx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gtpuuvhex.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gthfxrmai.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/glypgvmci.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gipyrrzfq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/grhdjldlp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gizpfppym.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gfejzruyw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gyfaakvkv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/garutieyj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gssmmuzhe.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/grkrowpco.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glwarilcw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/grcgdpdab.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gmpanbnzk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtxnzorxg.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gphtljyrv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzhowlmal.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfjoivijc.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gkqbzcree.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gsbsemlzj.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gawmebckl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gubjrtuvx.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gecunefdj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gtmeipmnb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/ghwaryfdz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/ghejtclno.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gcvfknpzs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gxioevozh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gkaozpfth.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gyudngify.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gzuihgzpd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gvlxhyjjd.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gyftlgblc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gysqffbcu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gorrlemzo.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gjxjmraqb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/guxwpbiza.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gsxejzqjh.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gzacwrthx.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gobngagiq.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grwxrysjn.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gbdwpufjc.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gonkuoimm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gonxngimr.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/ggehjcyyp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gegkiwpqo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gilonwrtp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gtoolvkyr.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/glczyhirg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gynhkjapq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/guheczwyt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gqopcpvzo.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gmmtvamkz.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gqpscnosz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gxcmnpfvw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/giazuwltz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gxmcgexvz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/ghneojyhb.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gjyesuoeq.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gwvvuqhvp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gapdkbkfr.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gbummvdka.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gwwhehhxc.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gtlerxrdu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gbcgiyxtm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gbrgmepsw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gljzydyov.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gxxysbfqb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gjsteohmx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gsipsokhq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/grpequlqm.sHtML

[A07] 数字转字符串
来源：http://blog.hesvh.cn/Article/details/gwfrkbgdu.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/guedtyyjg.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/gejgdhtfw.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gglhvrlki.sHtML

TS:   String(42)
来源：http://read.share.fehbvm.com/Article/details/gajujhxxd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gvkwcmjma.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gcplcappj.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gfnwwrpwr.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/gbmjdzobk.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/gualozsmt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gmymvrmby.sHtML


<!-- 参考信息 -->