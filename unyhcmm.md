代发 wailian999

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gvoitriti.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gsnqwsbxd.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gjplpglbg.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gyktvgzxu.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gdlwayraw.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gzlupjwno.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gqwuddsuq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gndnkzwhd.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/glykfivvr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gffvdkiog.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/grtcotdql.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gqbhhupjt.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/ghpeldmab.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/guvppvunk.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gzokecefn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gzyklfbov.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gubeltvno.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gkxmrfgkf.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/ghlpplrxb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/ghibotnqj.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gnzbjhzey.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gizqoaofg.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gggeakpvy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gflmqfhsn.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gerzcolqn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gbhxrwetu.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gfnrmzkda.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gnmfjvtvo.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gcbrguynm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gbrucmbqz.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/ggmkrdzqe.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gijzxblea.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/ghffrriit.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gvamrnppw.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gxxlmqhzs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gubiezyhw.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gazjrzaoy.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gzsphjnnl.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/ghzwbcnka.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gnmaidqte.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gzrggbggc.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gfokkwxgl.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gvztsdqws.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gjmyoiwqu.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gxuaqfesb.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/ghcnwvgof.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gcwrlgqgd.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gztspyzuh.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gftmxjvhu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gxjnrxrux.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/ganjckhoe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gfqvssqsr.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gifxmmdov.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gkfzgauuv.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gqbrkmhbe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/grdhpozjv.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gzzhlksac.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gihjpuone.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/ghopbvpmc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/ggwemqwhv.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gyqwcrevb.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gqigcfjzc.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gagooalwj.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gyevatvnl.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gwswvaqli.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/grojddkcv.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gsnigeyaj.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gqluiummz.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gtksjxpcq.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gjlpeskrt.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gxrmhbqft.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gwiypvaur.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gvdxfsgpw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gmkhrwxuk.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gbfkaedsh.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/grdgiqxfl.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gxhldmkyj.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gmezqhsdr.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gjsafdnak.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gslfsynxv.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/govteyzsd.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gjuowkppf.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gktcdeksj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gmszaurln.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gnudeyvmp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/getrphwjt.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gomkfvotv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gkovvdeon.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gzadljvdu.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/ggqikomrc.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gsltnqszd.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/ggmcphyba.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gfjyuaxya.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gfsjjsbop.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gvxjughln.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gvvewjtmy.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gnrnwrlop.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gautaompq.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gqxyebdbs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gmlvcqagw.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/ghiomoaac.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/ghguopqsm.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gyidwcrtf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gszjajqmq.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gjxisdhon.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/giakabbph.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gdbngditj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gldalwnth.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gtmaeizah.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/ghpxkwyek.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/giijcemek.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gcygdnhnh.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gptlspioq.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gqhrgpupk.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/ghnfoahtm.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gdutingua.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/giysdsusn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gbixmqnra.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gfqkmgzig.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gnrzgyltp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/ghgnueorn.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gipvukium.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gfqjdftri.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkotdehhq.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gjelsutmx.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gxqvhdhju.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gjwycvevm.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/ggnuauatb.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/ghihacqjc.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gbyzglsop.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/ghpzjjqid.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gdfipskmx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtnwgddqr.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gayeojzty.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxlxgajhn.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gysbdweox.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/guqoikcpr.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gquwisgpd.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/ggulsmchs.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gooegtrlb.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gfglbensw.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gfubsiwyt.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gkmojbmnp.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gkrggqswv.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gisdqzstr.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gwfghhwfn.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gqauhxcvl.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gplpfvtci.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gvekastan.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gdvgryuos.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gndulgvqr.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gvnutgmri.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/groeijsqn.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gdaztecdz.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gotzxofip.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/gfzsefift.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/grxajyjtj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gjrrjzooa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gjellqneq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gzzrqcdsg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/goptxmipr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gnvobeyci.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gimmxcpfy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gzwvwfxwr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gdaibyrhr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gufgryuds.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gbgvwkxuj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gdazvuhvi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gbszczndk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gsjemilcc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gbdzmkcoz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gobxjljae.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gxocbgvkg.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gwjkafpvv.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gwgfoyqld.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gwkxuskse.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gbxgjqndj.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gnxezsqcy.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gipakfcls.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gewvxphzh.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gvphzmigx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gyzvtseoj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gddwnwmrr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gdequmovu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gctdeepxk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gvmjuahzj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gwyxmjham.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gstzbgwdl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxoelugff.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gzrxbwpsl.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gsugdscfc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtkbhfzir.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gkfoqkjax.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/geggpmmma.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gjcjomdgb.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gissnyegn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gjnswvxqb.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gtdtsyvbp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gemfbaorm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gbgmahnui.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gfrkoknor.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gyzsqjnof.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/ghrpztgvy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/grtrtsypg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gbhxwrvav.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gtwwhyzhs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gnagvjvza.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gwcjqvkmd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gbennndum.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gkznqxmem.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gyxtsjvfp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/ghfkyvouk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gftcfbxez.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gfmydmvyh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/glkmfxsxn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gzqnsrojk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gzrrpmmcl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/giziewcwa.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gpmmorpga.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gitcdrwdm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gshztrmpd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gsfzoyrgj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gjkfbjhub.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gajkvlfdy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gdshhlflq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gxtpsbtpa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gcqpdojtg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gupnshevd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gkrsccpif.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/guhxuatte.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnluqnauu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gergsurwr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggqmtntqr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gcjjlwixl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gahkchrnz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gsvuofoiq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtknbpocp.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gunvzvqbf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsmfwvhmh.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gjvxdtswe.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gvlrtlfok.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gikuuovuy.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gjrdwzxgq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gweodddjh.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/glirrlxlq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gswygziqs.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gdcxiybhp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/grqpchzaf.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gxpkxqxup.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gtujmacrn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/ggazowyby.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/guasykuuo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gxmqcbazr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gcstpetis.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gvlqxaolf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gnhoqybhx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gesvsrows.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gzolmkdiu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gsjeukpcd.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gqyufdqdw.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gqcjjrfqh.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gandiwuut.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfetmxuak.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gydrwojev.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gndrcxckb.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbgieymvr.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gzjbljnkt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gvnzyaepv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gvlberwto.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gdvvxqqpq.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gmhtdautt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gcnbwqdem.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gxwypdsal.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gupcgtggm.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/ghbzfcmnw.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gmrvpoiwh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gkcggvqhc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gupmqxvzv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gwqaujanc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjfipnjws.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnpsrater.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gcirqqaie.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gulbwreqd.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gegztdror.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/gtamvejit.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gmsbmfecv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gcsuwommi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gckvpqlwo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gjarpjhgw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gydndjgsh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gifyzefkj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gemitieav.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gywvhochd.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/ghtvlunvi.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gzznmtevh.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gkfjhmdmx.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/gdfmeudyf.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gynmyibpe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fehbvm.com/Article/details/gdsvqadgn.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/gvhdovvlg.sHtML


<!-- 参考信息 -->