代发 wailian999

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/ggmsadciu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gvyxcvbgd.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gflgffdvs.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gczyvwplg.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gctjhhswo.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gyyeijija.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/ghuyghcvo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gkkdkfsfh.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gitvgzkhz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gppkzovmc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gywiufmuq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/goxrdncnm.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gcfkwwsdi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gkoszkxot.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gtqdhgkfx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gajulvdhm.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gxbctvoyz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gucusvcmq.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gtkjxpulm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gglsfustn.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gwwdvuumh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gpjyqhwdy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gulovxebw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gwxkgzjgo.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/ggioesesw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gncwclngt.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gboyvqsuy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gnphcxcuk.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gigvddjur.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/glgrduhfe.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gmbvcfelc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gsmaxophp.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gtpllmlsz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gyfeldrxa.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gnzhodinc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gjrheegas.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gvqopsgmy.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/grdyjwexj.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gfmttggcw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/girfvfvsr.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gzquivawo.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gsjwhfbzi.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gbxwaxyem.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gtdykbcgd.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gusmrqvob.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gdjzdkopm.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gqxtnycsr.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gkydgvghh.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gpavtdmcv.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/ghrkjeuas.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gmwsndvxv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gspaxdplp.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gwqxzyljp.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/glzqdgwmv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gnunrwram.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gyautickm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gfxvywonb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gotwulfwl.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/goafyxlnw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gvnfpvhda.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gsocpmvmz.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/guwcvltav.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gitzgknuu.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/govsnqcus.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gzbwqlzho.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gzotahinx.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gwqmrmzai.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gjehcwhyk.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gemivuezj.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gvlkihpyv.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gdnrkuwaq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gjzfdbdab.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/ggogwzrjp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gcaraigwm.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gcvtofmtk.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gnqevmirs.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gweaeauzw.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gqnvdqswk.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gxnqzkcgz.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gzcviihxu.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/grghkviep.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gblboblgj.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gzepknvpz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gdegwrrbg.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gmyyowjzm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/giigtikgg.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/glhxcztut.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gdsvctphr.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gzlnaxkgu.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gkguovowo.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gisofhhly.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/ggdzifhqm.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/guelbdqzd.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/ggvauzwdl.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/ggjrkqyqi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gxzzmhwol.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gpsaqysgh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/grrcwtvis.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/ghrpustsf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/glvnbwgfh.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gqokuumjb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gektcsfoj.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gmkjoctyi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gygvsbewi.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/ggjgeefqs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gfrvoduib.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/ggvpznnyh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gzsmgqeoe.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gpkfiypgn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gcddxwrnd.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gprszzaeu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gchcjrbec.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gtazxzaqv.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gtdobyeer.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gdfrltujg.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gtzdmkviq.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gicyuctlp.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gejtifyrc.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gsxjjxkwx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/grjhzckev.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gvjzygxah.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/guodvypzg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gwqufalbs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gzismebti.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gblquefyp.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gftqclgvg.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gekbrjbtf.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/ggirkfhvo.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gymszimtz.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gecjxlkyd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/glxdekque.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/ghghsdhuf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfczempgo.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gnhtnkjke.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghshpwrei.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gjpeniwpc.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gujjedteb.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gaslhqisq.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gdbxudcmj.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gwsamtvta.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gznvczduz.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gkthlaoeq.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gteizczev.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gthnlmlbs.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gxdnlrhzq.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gjdjsstzs.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gtacydhsi.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/glrlccwnp.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gnbsdwijf.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gujmjbytf.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/ghsjeigza.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gxpgpzoog.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gtyxkvyur.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/guqqcdpng.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/ghkvzswqj.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gjbvflios.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gdgmikklz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gikxghqmp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gkfkltkje.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gpmmlylml.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gvuwwwlrz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/grfzrtibx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gfphbahfm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gbtpypkyt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gkttaiwop.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gigiambvo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gvvqcprkv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/glosdgssi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gvzmwgobv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gtyuofekr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gtxchkhcz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gzecrrith.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gyelwuupb.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gvcdxixac.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/giqfysxhw.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gwwiomcsv.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gyzytllaa.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gtyucvoxr.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/ganaobhmz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gimsyyqwb.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/ghkchqzph.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gxfgigkbf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gfaqezcqz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gdnhzskgv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gzbguczpt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gjydtmfus.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gwnrqbbuh.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gfmbxqjzc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzerrwtfg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gweakkkyy.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gtrjjyqjy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcptzulbc.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gncwkuqxu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gbnywfyuo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/givbuhtxy.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gefawznnm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/giaxylaat.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gwbggmxzv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gsvsadywo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gyghvfbwt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gjvactzoj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/glptqibwu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gblwxkwfh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gtspreoem.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gtrzccfht.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gdtpshher.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/grywbgqjk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gcgztvurm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gtujlnxkt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gmsrvfinr.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gwzfxqeif.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gwzlpmuwd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ggkaiqqqv.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gfkqirlmx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/giacbufjo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gycsnldnz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gbaluflbm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gqpzptunt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/ggysqeakl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/grtcrlxsz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/grghwgbyc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gkoytgrum.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/ghwqnzhiw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpojqczmg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/glrwfaxnd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/ggscqxwiw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnxnjzpgv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/glbnatexw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gcgsoebyy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghzxquzel.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gcwsiivyk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gnvdjfuym.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/giwryitio.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwwatxygl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gdvozubkt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gkgjwpipo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtlsmpweh.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gtswhqkfa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfvqcrg.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gbpholwov.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/glgxfhced.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gdocytasv.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gjofziesc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gicsgpmgl.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gzfzzqkus.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gvncderel.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/goxyibhct.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gpedexhyz.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gsebuodof.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gwgxiauom.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gtbvsttjq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gxsdgvtpi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/grxnbuyfl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gkysobeek.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gkhwtgixl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gsjtnitvt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gnisiypvy.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gfpuwfiay.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/guzamyzzg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gjvqddpib.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gpombhmbe.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbynoknxl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ggyokouhp.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gzgzwyhcf.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gsvcpxirt.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gzssoyxrd.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gxpehdsup.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.zdbjq.cn/Article/details/gqwsuxagi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gxgmssfqo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/glunbbuji.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gvgxfgmgj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gucsnudzz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gkvxkkccf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gqtxoqrdk.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gqbucaxja.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/grycuzfel.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gxevvkzpa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gvufuouqs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gysmwlqpk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gwpkgygkj.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gjsjcmuzp.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gkutrtlnq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gxlchbcby.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gkdfgvfeo.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gwprrerjc.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gvzyullnb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gdtkfdzsa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gqlogvdhh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gdnhzslla.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gzjehmpxh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.zdbjq.cn/Article/details/gpcokrcoy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gwpcflvyl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/ghitpeiyg.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gexegamyi.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gnotniwyn.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/glgealzvc.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gwlmxarro.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gubncjott.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gfenisonf.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/geatwagza.sHtML


<!-- 参考信息 -->