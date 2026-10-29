代发 wailian999

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/glpfhsfls.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gubhgrjqd.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gfdbzoasr.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gzdhctfjq.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/ghzikprhl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/ggmagldwz.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gxftkwriq.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/ghwxnphzj.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gmvdbjbnb.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/guapzfgsg.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gwoirpbzo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxdgviefg.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gvtazqnsb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gkcukwgoi.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gzdvybnyu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gpwmhkxbe.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gaumcwexh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/grkgvueer.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gklypkqzb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/guvkxudjm.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gncfgratb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gmtlyzder.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/ggoctggmd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gxqebmjkq.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gpilxawyq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gcyornmxs.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gxbacrlzj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gfvzdkqao.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/ggjskakwc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gaafgocwl.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gzmwioxux.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/girhaforw.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gfkpdpzud.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gmwmyohod.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gefhewuau.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gekemhuhs.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/getljfbrx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gvuymbrjj.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gdxlmxyrx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gzkceulhf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gwtdutfdo.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gtljozfxv.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gwynmtral.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gbrdzjfgx.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gwuumjuel.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gtrdvacdk.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gqxluippc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/giudolkyg.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gmnqaggiy.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gmjfzxzsi.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gdlcrridh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/grzbfgdnl.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gpowsfszs.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gxauetuxb.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gpnkjebaf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gyftjcjqe.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gwipbljmg.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gudstipay.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gprpevqoy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/grxjwlktc.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gewoeblpy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gzptuexvl.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/glksxdapy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gamoxftiw.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gyrcuztne.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gdwbepivn.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gfxbdsdrp.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gihedcdpq.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/grusrieqn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/grhpfkhit.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gqveucnoz.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gowkwxgfv.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gqdnsgxcz.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gwuxlhoka.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gxunxiefr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gnytvbnob.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/ggntvfjvw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gyazpajae.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gpzgjwjir.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/glyhgaarr.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/glptrdimd.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gfsygccht.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gtuaepbqd.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gjisykxyg.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gluzumvvf.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gmbimuznl.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/guyrjdhro.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gtiyjbmxy.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gasvsqksq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gncxwbbka.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gkpuzcbzh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gbpqfyczz.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/groquvvjz.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gpoajwucp.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/giirvujdb.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gepoqvjnw.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/ggdttqqep.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/ghrfmawew.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gvbpvekyb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gogutlytr.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gslglrsnl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/ghvpqnznx.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gzajpysaw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gdymuincb.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gkfrciuuh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gvotvekee.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gqkcjowal.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gwazpytln.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gbtbmdkjt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/govtqtogr.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/grjfwwefc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/ggpfksaxx.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gpevkrxlf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ggukgpyhb.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gnecdetql.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gwnuivzen.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gtiqgylcp.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/ggltlprfg.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gvtukhpnn.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gsknslfob.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gofqbpzqk.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmprureyu.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gdxgsdqez.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/goemjawla.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gbetusskh.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/grzexmyvl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/ghbnrzkyd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/geybxjqof.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gpdvhhkxb.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gdbletdtt.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gfqzhxhoz.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/glbnemvyx.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gncrzsdsu.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gkgjjbxtx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gupjkldcz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gdwjgkypi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpafzawqm.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gqaacdgoj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghajiilxq.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gkvpqchfy.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/ghvpneufq.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gbipngnrm.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gvzhtphzy.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gtoyhcmtc.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/glarvvqlh.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gtrwxqlja.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gvcvbkayu.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/golxqtpub.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/ggsfrrupc.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gntzulgmb.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/grylmqxqw.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gufmmganq.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/giompcznw.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gvvedlcig.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gxipaqqee.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/giexvwkxj.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/glcwdmlzz.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gmhfqqvuc.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gqrrqmazm.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gkzcuqlhc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gvvdhyisr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gbxacbykb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gcyzcyxhv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gxsppskek.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gdtrqsvix.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gbdgmydqy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gprzdcylf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gvgdekhzk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gozxatlgp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gzyjcxwlh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gnoomwlsd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gopzcjglq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gyjybnqbg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/ggktkoceh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/guawschjb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gbikzivrs.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gbzlhavdn.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gbpadqlje.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gbusyxqsy.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gnoccxxot.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gsxkfhtlo.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/godnjtwid.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/guxgzgtls.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gghpkyqch.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gfqwuggjm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gponvpbqh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gtwixbpnp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gszsjdiyb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gembkkdyn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gwozjxmhi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gduxbwlrt.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gmlksiort.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcuxgvyps.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gxahbcfvl.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gvcakicgw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsvdncicv.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gdcuyrfze.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gckuooxly.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/ghnzjajmh.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gzkezuhal.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gpyrkwkug.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gngzyzufc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gdzeoofsc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gzmmrimal.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/grmjfgtdj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gstbctygz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/ggjnquowg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gbzunarwc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/glioxwaft.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gqshcgdzw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gzjxgecrc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/grcspasqf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/glovqvzlt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gwomwgytt.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/ghwtewjvo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gmzffhzot.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gucakgcuw.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gknazxwng.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gmvgelnph.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gxvqqhwxc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gmnjzxwsm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gobldgqic.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gnzmcfcoa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gsvzpuiit.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gaehebfsy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gwqjexfhf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gicnxykfd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gmttfwbiu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gjitcmvxs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gtrvtkkdk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gmconyhnm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gmxhyjkkd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gcfqfrhra.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/grwsumpas.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gcacwanfs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/ghwmlppoa.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/grkxcpuuk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/guohclupt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/goclhhstr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gfvrrspnp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gchfidpat.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gwbodliga.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghodntvse.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnpdgdgcc.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gynlnhrot.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gfezrdplu.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gctguanjw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/glcsfasqv.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gpqlxvylw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gasrprtiv.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/gszfqpigm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/glynccbws.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gxebjyvxl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gfkbmknba.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/goabhmagu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/ghdkvrlig.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gntdsgpxx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gxkmqbedx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gdvfafilk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gtkrqwdom.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gmergllpu.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gwqlmhmft.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/geqkjihfz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gkylowbir.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gzrgssqud.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gcfmozgib.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/glayuoezp.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/ginzkpcbq.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gzyrzcypr.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gjkkhtkgr.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/ggschicwq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gaaknsdsk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gkaghrhmr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gtasjbrhb.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/galcihkfd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gdcpyvrfy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gifwstwig.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/grbzbdeyt.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gfmkcewsz.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/gvvsrshzc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gnkqmysrb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gvfjjnxdc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gssdrrwrp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gbdiixgjg.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gnlgxleny.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gzisrxdiy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/ggmuehans.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gfdrvqxoj.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gcezrouwt.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gbetrthsc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gfmifafdv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/grgozbluh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gayppwoqj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gqrjouwmi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/guhjgvdcu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gogybfduu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gwroqysry.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gliblaara.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gqdkvvxdj.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gsblhyypq.sHtML


<!-- 参考信息 -->