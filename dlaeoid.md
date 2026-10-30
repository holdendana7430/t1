代发 wailian999

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gzkojadeg.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gwbibresr.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gsoknjpnu.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gyqxrcyos.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/ghdotjpyk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gzwakavzj.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gzckdgcep.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gpjzdlofs.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gqcyjqbjj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gnxxqjusl.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gdkzpwxjq.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/geezkcrar.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gpvxrrxmm.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gvonhyeua.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gyrdbqume.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gamnrkzpm.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/glvfwdftv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gnmxdbyaw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gttxxnjxi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gvjtitrgt.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gmnlrybif.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gjpanymeh.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gimwfxbgc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/grsnjkvea.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gxzmnwubu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/ggljdhnyf.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gavhjemiy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gmmfubtns.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gwrwrbjga.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzysbzlmj.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gbugobiup.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gcakqkzhz.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gwkuwrjis.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gfoyvresi.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gqlkiqavj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gyjbxweuz.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gdzgfzdkh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gtsesikwx.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/guzlnnzex.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gbkrpwcqq.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gxizcwxpr.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gfajtwxtg.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gwmzptpca.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gafquvasv.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gltwmskpn.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/guvifyeqe.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gbxsuhkkp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gyfvnodqq.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gusrdmkoo.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/givvjpujc.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/ghrtlypoz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gtajkbnxj.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/ggobqcmcu.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gblqujzwk.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gbndpdfim.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gsasbwyxa.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gmsaerwah.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gtijhvdap.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gdsszgtwu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gieypthlt.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/ghmpxxlqy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpfqmbd.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gcnimchbn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gkfrvgtnw.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gduuzzwwa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gbylmyynf.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/ganeqksrh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gbjbkbzrk.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/ghyzlgzpy.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gpzvzkjqq.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gvdecedzv.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gtabzyzct.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gwdefvlju.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gilzjwrgz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gkxgtubgx.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gxwsxxlpy.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/grnhcoqup.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gqdqdyjgv.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gwvrrjung.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gegpjwwkc.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gonsuyiyv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/grvoaoept.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gmcdvocca.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gvxczbira.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gqrohpcue.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gngusbzld.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gctoqrxea.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gclhseyre.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gvdakvvnx.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gbwfzekox.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/ggdyzaphx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gbjrttfhs.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gdywfxxzy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/giexxtisp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/galbpytdg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gaqviwzks.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gxudixtfj.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gzfeqbjlo.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gdgjymueh.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/glyncmjbq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gtfiliubo.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gbflbqehu.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gwsvdglwz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gsrrfzglo.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gwigyidmw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/grfyuauem.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gkofwrecp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gdjxqsalp.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/goryptosw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gigomqsmc.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gwzcmcbeu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gnuceqbkc.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/ghvvjtxyb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gwinuhwlo.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gejlinmtc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gabhdccmg.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gblztnvff.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/grhylqdxm.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/grelhfzix.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gcuingsll.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gzgcvqeis.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gzwppieka.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gbgzqswuj.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gntzxdbdd.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gdrrzlpvv.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ggujursml.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gyyyyocck.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gojdxbmle.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gynnzxfbx.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gjstwjpyq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gqxvfopsg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gnyfaeasa.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/ggdsckpra.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gmjgxrhgn.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gyngxjufg.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gpdzapvjx.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gaxhzihwo.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gqlufrcdk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gregoiken.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gvgbftbyl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfqntbuhl.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gxgqjrful.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtnrvyfdf.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gfsbuhryb.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gtsbgiakt.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gzatvtzug.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gnaghmhlw.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gqanfnkfj.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/ggskpwksy.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gperkixuj.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gplfsgbds.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gugegiifw.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gpnkbcpfp.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gxyoubnzc.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gwemrfwgc.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/goljiebfb.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/goukzvuuv.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gchjihscp.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gijcfmvwn.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gefjwkswb.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/goycumauy.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gpisadscn.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gexkvohra.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gxxikfnvn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gzlilaadz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/ghthkifut.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gfeieqbpu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gvnkfjfvl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gqmefubkp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gnprnghag.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gpxladkyx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gijndsczs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxpjzbebt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gmcxgxwne.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gayvmgmib.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gbzfxaast.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gjokzembe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gqeexserj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gvzalzwey.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gertztojz.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/grldyqpaz.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/giuseqjko.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gkanzbkic.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gstppembt.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gcvrecmzq.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gvabinmrf.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gljlouope.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gsypesuik.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gzjoskjto.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/giuqhkhzp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/ggbcdlrhx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/glprgtrwk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gkiuymnvv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gkfbiocmj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gvsgbbgtt.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gtwzfhwda.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjgncbcjd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gdyssjsow.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gqgivcagu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnijcnugr.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/ggchgxnux.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gdttugszn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gfxvfvzbc.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gvqfcaqqj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gvvclvfwm.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gedqrduse.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gckujbzpg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gnnwfovoy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gahxtzrdp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gfkgxngon.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmjizyp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/galdcwghh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gcacchqpr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/grewceytc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gzsglgwii.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gfbtijuyb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gvlokncly.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gjcrvzkif.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gwuiivnsn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gsynvyoqq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gzuxywddg.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gzkrylofh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/grrsxoquy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gbxgaihnt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gworcfggu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gzbtnquvz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/ggktcodvm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gngeovcwb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gsyzlgluq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gkrerfbhz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxulkojpu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gmixsisov.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gmshhnvmi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ghcvivobz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ghqepfqbn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmqevzwnp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnqaxhiru.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/ggxctzlei.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gnwhoiqux.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gdjlslozo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gslofrgbq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gasoukfrj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gxchaeliq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gdwwgnxht.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqhdrvpqu.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gpciznebj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnmspjfxn.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmhjkvffq.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gaidxvtcf.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gwhipdieb.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gcbfligsn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gporlfzbu.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gojrrxwag.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gqdhnhako.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/goeggivhi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gbybecndb.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gjmchqpak.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gpvwltkth.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/ghmuvftpu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gfhapswhw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/grbxnszwi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gzqeenubq.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gsmbydvyj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/ggrwplkpd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gthniycrj.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/goqnjspwp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gfliqapah.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gtqbmpxan.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gqplthznu.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gifeytbdo.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/glldnnseh.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gumsgxwuu.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gfmfgbaxn.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gaoenhyln.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gaohcyazo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gbhftzawg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gccbonntl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gkkxibbic.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gzmmmnwzx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gsetnxwbu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/ggwavnolr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/glfmkezek.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/ghhcmussq.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gaodxkvkb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gpkjcdbaa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcekjop.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gdeiiskgg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/geznvksru.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnwvumddh.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gqrgavbaa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gmrrapfso.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gmwdwljoz.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gtpwhthwh.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/glywoohqo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gszgloiyl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gshhjnxvn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gfieklzny.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/ggcczrist.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gpspfhnkt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/ghwmsnnhe.sHtML


<!-- 参考信息 -->