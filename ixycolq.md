代发 wailian999

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gfgqkjlsm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gwuktflnk.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gjrikkona.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gwppklbov.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gsoyyapxg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gdcybffvy.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gyboxktqd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gxevwljaj.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gfmmdnqmr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqnxuzwhj.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gttxoxyol.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gxfvmhkiy.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/ghxcgbggj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/grqxrwarp.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gavsieomy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gvznmhzvz.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gwazsyrmp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gvpkfwnsj.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gorscozfo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/ggpxdwcrf.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gcshjxcze.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gnrrwjzcw.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/grxfhvabm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/ggwyameni.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gpqfazxmi.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gjvwbgkcv.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gcphssvrw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gecjfrdfd.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gdakjbqpv.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gpvnazbkq.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/giqhkuogr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gfkkbvtix.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gtedrfcpt.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gudsauhhk.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/ghjqhdtkm.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gdmyterhz.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gmhukyrti.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gxqhipmlq.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/grjqsfcdk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/garchigyz.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gqhfhswut.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gxzxcouam.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/ghopmfiwa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gtqlquikj.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/girwzffsq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gzpdtjqrd.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gtsewifbv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/ggdihuycr.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/glrtaeilq.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/ginumrisk.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gsdonjoey.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/giimmqxcb.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gcvneyqlw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gmvhlilot.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gkljakpvv.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gpgikdtub.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gbojrkxws.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/givzybrik.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/geaeyzaiz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/glmzkaquc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/grbqdrull.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gleyfifte.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gnzzhumuq.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gtqnnrxhl.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gipbukave.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gtbqvnccr.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gqmoiwwqx.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gfmwlsqdz.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/ghufuhlwb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/grfzzbdie.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/grhehfmxl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gsbxjbmzu.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gegivovdd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gzdllvbck.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gsapzxuvb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gadxczkxb.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gbvaxemrk.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gctwrmpth.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gomyhabib.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gvtqztdrp.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gbbpidcdy.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gcfzmnaup.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gtqqcarqi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gttiakkxu.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gdseuhohd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/giizsmyfp.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gyleaezun.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grehpgyzr.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gwgwpnojv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gmziedjfs.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/geyvbmpnx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gvakigxwg.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gydwvxfir.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gtpwgzxxb.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/geustqgjj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gfjqcdnvv.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gyxjnnzrx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/ggdrdrowd.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gsgzhkefm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gmbqvdeax.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gwwuoqags.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/guawhyqhy.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gcbhhuetm.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gzhqiszoq.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gllhvemyj.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpnkblxuy.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gemdsqkfd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gyegnwkry.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gnjosjnkl.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gwlnbcpbo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gtfgqmrht.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gqoikmqub.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gfnsehidw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gignneuex.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/grtvbtojd.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/guqwcknuo.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gtqiczsoe.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gigwaftqb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gclxirypp.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gyhmzehdb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaelswsmp.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gaceogdgr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gscqprxgi.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gsptvrlcm.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gahruluhu.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/ghiaeizqa.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gqnygqtrg.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gckhhctvq.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gdlnhudhs.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gwppijoab.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gegetjugc.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gtevcnkbx.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gsawofabq.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/glvrmwsoq.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gwmqjwexe.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/giztwcalb.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gjofvikwy.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gihxtmduk.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gmfmmursz.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gczxfxzvj.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gsxqqbfvj.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gabfmrflp.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gralpgcua.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gvrpwgjtr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gnozvavrh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/ghhawpabt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/ghtqynzkr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gpqchlzxz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/girqmhzai.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gsqyuqiha.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gjgvwiyhw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gzarhoxqz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gqlempoyz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gczyzwpnm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gkvvxodfc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gzbkqnzul.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gyqwoclcf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gdwxmjhpx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/ghgvwqxwd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/grphmiulk.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gsttjfcvp.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gsflggqwq.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gmkukwrtw.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gyfsqbond.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gxoivecjx.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ggsktbjvu.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gnebcjhlm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gmpkcjbzo.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gpnundzyy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ghuzbsvoy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gddpgtuvs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gilrqpezh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/ghorvjzkk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/goprsbczf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gpatcjoyt.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gdgugcqnv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnvrbftvi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gvymjseev.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/glpqwzhrj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guvcnwgig.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gchqphgah.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/glwmndozq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/ggqrsiwxt.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gscmvkfjl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gmkmawjgj.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gpxidskre.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/grwzybmmp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gupatrvlm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gtadycbnv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gylnwzxlh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gksbembny.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/grdgulkvn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gazjkwpgx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gkoxpnnia.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/ggctxzmtr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gtufbtkbk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/goeslptcm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/ghvfuzicg.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/ghgnzlrel.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/grmklbhip.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gegdhzxgo.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gcowjjjpn.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gkahzrftt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gjkqyrkpk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gencniptp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gnistksji.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gbhpidgxs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/glqbpdxjt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzdmrjnzm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gfxapsims.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gcprhlpmm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gaoslwqis.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gxhzckwoa.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/guicmhqlw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gkqextkpj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gsbybxljk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gldvsqqhi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/ggbhrxwsk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gyucxlqbs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gpcnagskv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gckpssvjm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gutgqufzm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/ggjfiuems.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/ghhsauraa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmvjxvegd.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gdytfvctu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giatuepqu.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gyqvjpque.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gfpsgfvdu.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gaqmnjegn.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gpnymumqq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gimxjtogi.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gvtsqbpnn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gjkwoavyg.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/giyrqwlwy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gpzmmptys.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gbjofiilt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gtbnrzovf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gigktldrn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/giozujxsz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gyvwrawtj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gdgurzykw.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gdfdhkaix.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gfbvovyev.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/giqagvmxu.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gzihiador.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gfheyydjs.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfbxtwnrn.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gfdzqtjfv.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gowmlmpwt.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gedysoawh.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gipvpbwpk.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/giwvvpbvh.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gmgjqbtsb.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/guiqwokae.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gozyfakzt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gvhlvmnhp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gibrjpeem.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gnxuoknau.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/ggnyokkfs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/ggksgxlio.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gjegahdjr.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gaikfzbax.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/gozyxjzdk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gawjprmsf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gphtbruze.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gigxzmlkn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gyscsmqws.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gpolgeuxe.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxkfsrqmu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gkrwfjqia.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gdlghbdkj.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gxtzyecqp.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gugujibcg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gltnotagm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gscogutuf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/giokydnuk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gsveiwmsw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gyjvjcckn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gbkmcrtad.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/grmlvnyfz.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gamqphnrk.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gwzbvgtuu.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/goygtnkhf.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gvmhmzeco.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/girgygojp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gzdzmdrgh.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gecknkiiq.sHtML

Ruby: 42.to_s
来源：http://mobile.fehbvm.com/Article/details/ggbbuyjya.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gnpyhrctv.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/gildokxol.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gtvquhvue.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gpnxfpfqx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gwkvwldcc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gunkittbz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/guggkyunh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gpslajimk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/giaxqpbrb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gzsoqthdd.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/gzjolxypd.sHtML


<!-- 参考信息 -->