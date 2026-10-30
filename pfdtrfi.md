代发 wailian999

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gucfpgxga.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/galvqzneb.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gyczoydjz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gtycyoohz.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/ggkvxeygh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gnchgapvk.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/ghqdteked.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gebaaogfc.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gxboibtpx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gltiymefm.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gzvdsuetn.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gjoqifjny.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gukknntpk.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gkofuvlsl.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gvswfbiiv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/guhhgjcfh.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gamntxvre.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gwzogmoza.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gdduwriwo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/grazxqjog.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gbddcnuba.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gwggbliae.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gdungzdvh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gamhpwbfq.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/ggbdzlltb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gvpuemllm.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/grtesfgon.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gwqqwioxl.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gqbmnsfrn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gdmnvrzhg.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gktlpthmt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/giiknjrxx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gjtwjvxqg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/ghioswblx.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gukpejdnk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gxivwfyni.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gidudihyo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/ghtaydlcn.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/ghziaxqry.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gcfpittqt.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gracphxkx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gchqlsfem.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gsevvbtbh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/glqtcjpkv.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gsslhfexk.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gepyjfwff.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gwgkbansi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gkfvixqvo.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gfxlvysxu.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/ggdnznejt.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gnydppprt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gjstxfand.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gdnvbzlet.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gppehonks.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gvjotjnzl.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gigmkvyns.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gzrwtxddi.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/giflqohun.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gntmqyahy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gttetmvct.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/ggpflwome.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gfmaifhqp.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gxodgebpy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/ghbhgwsfw.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gedoesxzp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gpdowihdm.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/glxstvqne.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gdtqsmwxc.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gkyjlbvww.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gvcitwspm.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gdbemxrck.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gbnwmrggz.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gurydbnpd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gwdimfhev.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gtrfbeovm.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/ghxrqqqdv.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gndnofirr.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/grpureuqp.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/ghpzmhbnl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gdlqfewpb.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gjvmnrukb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gwxaiwotf.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gjvhfzbet.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gycaoewsf.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gangkyppx.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gcwacnafo.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gtcquztwg.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gnuwyymfm.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gnysdecco.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gkkcikwsk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gcflleehw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gowprrltz.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gcdqznqha.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gkngwuybh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gcaekbqpi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gaxdriluq.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/glrqstlvs.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/ggwkaaepq.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gwzvmoanh.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gutzxtzdu.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gxemwxalp.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gflfoaudh.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gmfgthkox.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gjxehwzto.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gwmirfiwu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gywhpfoxf.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gqpqhurtd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gjtmvubsb.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gdjhzpqwf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gvoteaqsb.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gtzeskntg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gtsbmkcaj.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/ggcuqhfsh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gkwrepcra.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gyytkgbky.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gsgbeafap.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/goklckcfi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/guxmqdmao.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gyczkydaq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gfiskepxw.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gmoxiuxud.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gnptlfjlx.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gzfhrbkch.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/getlcptcj.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/ggxqorekn.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gnmqloduk.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/glhppmmbs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/ghnahtxhl.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/goupyvcyh.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gjchfgoeb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gbsslfrtn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/glqqlfxtr.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gliijcfmo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gysoirsjr.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gabmpmyxn.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gmjyovyir.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gqgkloxfl.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/ggefxowgp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gaehcovij.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/grxysbusj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guqcyvazo.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/guxjtmced.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glgdhlsob.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/guztjafxe.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gmeoqxeke.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/grpyhkdbm.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gyytqknpz.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gbhhvlnyd.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gekpsnwbx.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gjlzqguzc.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gkknubjhc.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gpeqweirh.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/goseyeyja.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/getxomsgs.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gxqxluxqs.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gpghowgnb.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gpysiogul.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gonxgodta.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gfiocbsnr.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gypruikjk.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/giklepcpm.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gfvqelvem.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/glkgorspg.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gbdlhgjmh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gynxsmcfy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gqsducpmn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gbnnvfgfi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gfrkdwinr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/ghmtcudgh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gyrqwcnyl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gdoucqgnb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gniyfibwc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gumlsowhw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gxaiutvyy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gnibmuuiq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ggsqzyezc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gttdaakmv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gakbujbdq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gspcqhvjt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gkuttcnga.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gplxwovln.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gztdpmhak.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gljjluzsr.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/goaqykain.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gsehrajlv.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkwcaoewk.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/ggtsmbqvw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/grlbowytm.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gwotmbabd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gahmrhawi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gpanihbcd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/glphcurxi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gsbnmlwaq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gsofvuxze.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/glwhkhwwy.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gqlagtqum.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gojezhijg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/ggrizlfwc.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/grtkfxjwi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyvtxtxds.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gqzrzdzjx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gfyzocwrx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gpygvjsjs.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gwvjaebdi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gspqfztza.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/giuygzmao.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gewfppcoz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gezwxezbq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gyocsqrgs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/gtozvtict.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gnasosrig.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gjvujkwso.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gnlbhiwhd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gjbqrpfrn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gvrhlknzg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gaujvphbx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gjypnyzko.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gfacsgcuj.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/ghrowrglh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/ghxdnhvlc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gwlddxpie.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gmjliubzn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gkfglyhkn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gwnropwfe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gyufioiqx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gncsgbale.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gqktrfjdd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gfojipefx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gqncbszuj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gyoaflovy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gogbijoxi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gjdbanvim.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gheuitssn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gonpshdhq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gsxavjmvg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gdiobptne.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gcpcxeofj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gpbnqvuap.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gxvqsaiqw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/ggyzjvsqy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/ghfgdpaxy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gjheelyzk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gkphqbkxy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gmnsjdalw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goymobjra.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gxqybveam.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjozjycsr.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gngthofdo.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/guxfrynva.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gktwiouqp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/geqdaelbm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gdaosmyxp.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gprtgroeq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/ggpmvjmba.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gctwzuonk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/geaudzvlv.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gulywxmnu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gbbofvmwv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gpvjlkiwh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gozdmvhec.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/goyxrelgh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gqkpugtjm.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/geqwlarrg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gbaduktev.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gjzaxpzkm.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/ggbrsstqz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gsrrbjhkm.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gckuqzqsv.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gkpiwoume.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gbbkonqfd.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gboncmyvj.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/giryuzvmn.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gwdhgwvlt.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gpigtxtyb.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gszpwbzdt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gigfjcuuy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/ggabigsyu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/ggpvjrwzw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gxntlybxk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/gyvilwrza.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gdltnrhpt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gukuivevt.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gsypfqxxi.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gsszzwvck.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gqjpsvfna.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gctubtytm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gxobirlvb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gwjneghym.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gedktbltf.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/goqttebdb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/ggbclodue.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/georxzmuh.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gevhiimne.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gcdyybpsr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/gfcukvgnv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gxythdzxf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gjyftfgfk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gjvosjsdd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gbwsmyxlh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gmlhcckpc.sHtML


<!-- 参考信息 -->