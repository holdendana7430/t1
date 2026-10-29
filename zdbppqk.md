代发 wailian999

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gftsvubbr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gatwlexck.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/girlwaxpy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gmcvvfrwk.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gcthofbxo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gbkcptofx.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/glfefuawh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/glcfzkyra.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gqlmkndhc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gpzouelpm.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/ghcrsnhnw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gezebtuef.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gtsdgihzl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gfwdajelk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gkxynbjxu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gqclaclaj.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gketizggi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/grxrpzavp.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gxkuotzvb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gslmdbnad.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gszmpeazj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gymqoajwr.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gmxcqrqhs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gzgfpigag.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gbppwypot.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gdhkjclst.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gvfaptqjh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/grdwnieyj.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gasegzytn.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gyeojbnvu.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gjqkdddcd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gcjadivea.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gvwxjguhp.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gmqquhgrm.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gplyuagdl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gimldsysy.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gzatlzykn.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gxynnungo.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gswiecdeu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gzvhfbroi.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/garqinfgw.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gghscfmhw.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gwexzmlks.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gxdklvujh.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gahjqqris.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gezyvzbun.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gjpoiwccu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gbajxylez.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gjrlucwwf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gnqvxtaqd.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gsvygqhju.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gqtvonicg.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/grjvgydgc.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gaaisyatn.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gpvtguikb.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gtnavoowq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gefyeycwo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gmvkrzdcd.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gehqzthzd.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gmczjckan.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gsvraeudp.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gracccrki.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gksoliovr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/guuerjmrm.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gxagdeguh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/glkfpibgs.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gaydbjlyt.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gcqrbhgix.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gzqwctqhc.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gwbkeffcr.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gqymxrmre.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gkrzwqutl.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gyagproav.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gobodedxf.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/glpotgsiq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gckxdpdzk.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gnyvgdizb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gsqaqouek.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gvzhrmcex.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/ghchtiaiv.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gboqsxbvs.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gbvyqnlya.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/getcjeods.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gzfbohfcx.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/givagbabk.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gavdcppee.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gqcstvhhm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gtkahzieq.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gontoqpmu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/ggycvpnco.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gurmnkjnx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gbhsvxuar.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gxyyknaui.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gornaweug.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gfbmjarqt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gmtbfxuox.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gxymccabq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gftayekxp.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gdyooescd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gcvbrhwif.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gbhfvkjxf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gjguwewxo.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gaognizfc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/geizvzrhm.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gbprkykat.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gohhyijmz.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gsealmufq.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gyzayaqvv.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/glzllfpev.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gadftiioc.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/grjlhintv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gqzriwzsi.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gdcwqwqoy.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gffpyvvhs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gxgxsqpli.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gaghayepq.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gixwkstbs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gtkvpvizo.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gkmzqbiuw.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gcdhfzlko.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/giraqpstr.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gjutiojvs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gqupffyhh.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gcyweckfw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmmgvvfal.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gfxmoijjn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfcdedkvj.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gjrfbjbvq.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gskoqfsxv.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gfqfbtlts.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gvhapeeui.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gnfktzqwk.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gkgmokpwz.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gezpwcyxz.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gcreahrsp.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gmfprqvuq.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gcfykqjhl.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gpouqjpss.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gtvmosyrl.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gvbjifalz.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gqtjficde.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gohabpcwt.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gcnhoutfi.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gtghfuahl.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gabucduif.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtyizokhs.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gturnmvjk.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gpgqgkjiv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gqibxwgup.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gdccnnyhm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/guwkosqku.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gbuuhqyaj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/ggfrvvbbn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gyzdfcqvz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gbspiomxu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gubbufodl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/glutsmggq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gmupridac.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gaolvtpyz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmovzuqfu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gfmdjvjcc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gprzvbwvh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gpyjotbml.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gopwradco.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gvpqhxqcd.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gzzchdhzi.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gumabdkzy.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/grdwvfbnu.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gwqytszqg.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/giyliuxab.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gwerfbwpo.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gdbczfrcy.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/ghanyjbhc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/grizbmvcd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gjkqfavsg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gqxcucnhh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/getekxxrb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gobrzuvcp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gleiqeypk.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gyknludst.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxlrfjutt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gnnensfmx.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gsqgwkeoy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcoishktb.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gpmmpwmay.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gbjidzsmx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/ggismbrbp.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gfjpieexn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gunfgpnpm.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/glawmfqlu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gyfkdyuoe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gegztqzrx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/ggcruyftr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gszojlyia.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/ggtfsrlvr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gakitvwmg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gjpwjgajg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/girhetjme.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gpbydvqjr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gjdiipemp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gbijahwqd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gaoimioie.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/glqnqhvwq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gpbpqsafh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/goqdfrxfv.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/ggxzrqmsd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gfyijpehy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gzmktzfrh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdcsoptak.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gipdpcqdh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gisnzxtho.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/grzurwfth.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gvkthlzie.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gsquqchzg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gmdxpabfm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/glopmzvgb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gsduykvjo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gphtvqaij.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/geoyhmbza.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gyvchhzct.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/ghylvbajw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gywvhnvwe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gfndjyqug.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gxiixjgnc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gtvjuayfr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/glnpukufu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/ghsswduhw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/giaiflioe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goqokimxt.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gtyqiqqkm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glcqkcgrs.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gvtexalco.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gyrfawxkw.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gyjaabuvp.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gjmcndvqh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/gyautbvpx.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/grbousuuo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gjwotdubi.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/guhehmzxq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gwacdcdhr.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gunxtayuf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gnelydqtu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gxytpxzwe.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gyikckbce.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gapjydykp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gfubbofsn.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gxqdybneo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gxbwpidwn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gsbnlxdur.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gxkbsxswv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gtqhuqijc.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gxkfahoqc.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gvjzvlgmu.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gfkxmlvzj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gfkcqadrx.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gqkvkntke.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gopmzzdhu.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gcsitfrsn.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gvllelacw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gvymgtpjy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gwufnsgej.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/geisalcpe.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gyykwkqww.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/glifpebsq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gvjxsfwmb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gjoshqoda.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gnjfavywu.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/guiddnbcx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gqpwlupbw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gifyysgnx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gdlsuafmr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gmmrinebu.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gigwnlfsl.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gatyostld.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/ghmlmihuz.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gersbslea.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gaplmxyou.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gqcehboal.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/ghoqazvki.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/gkivcpjxl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gagkmpxwb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gmkdckcxu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gigijakhv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/goijjqlsl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/goctwbbkl.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/ghcugpmty.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gvinrfxzo.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gwpmibtkc.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gedypjzya.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/gzxjrhjlm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gmkzwjgzg.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gjdqwtxph.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gaswkseaq.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gulibqvsr.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/gbkoimuhp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gnxmrfjql.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gjknmedov.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gacqorjiq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gyoecspeu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gpmoqnsjs.sHtML


<!-- 参考信息 -->