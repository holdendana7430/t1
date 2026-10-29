代发 wailian999

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gsbgctmdc.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gvuovexby.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gwknecrqz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/grczfnpsj.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gqazsblpd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gcxjwyowf.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/glppnbgww.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gjibmcfpt.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gqnhkzbgl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvrjvnzoy.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gbhtxjevf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gsvmsqogb.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gjkxsomym.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gouyutcim.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gmbncsqaw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gcatmogef.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gnbqthezh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ghbhqefny.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gvjzfukld.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gjudxdznn.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gdasnmshg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/guzpheaso.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/glhlajgyo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gfgmhptwj.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gvzvedqne.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gbphmsain.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gdcxkthoz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gvmkrqnhc.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gxsojtdwe.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gyciedpjn.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/grhfdbjcb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gsfhxmbyx.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gfzbwvvip.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gahnsvrbc.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gnxkcxhmo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gxbvphirz.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gtyveykms.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gjnoslbhl.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/ghqzyxbdq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gikmjnecg.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gwobdmgzb.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gotdbfmgp.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gxxpwgntf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gkcvsatsg.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gjwridwqj.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gsfytdbdo.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gftkppjyo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/glxgkoufh.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/giqsoyzpi.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gcwpmszpt.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gpbnprwer.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gdtayzkrv.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/ghxvkchdb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/ggfzmcvvj.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gmhwiqwwn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gvcpxfaac.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gcmpqfgyh.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gbeaqdono.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/giolbrduk.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gzxlhrmcb.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gqtmgqmtw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/grvlgpbls.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gfpmavhsy.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gwturzhfq.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gulbcxnlf.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gedgchbew.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/geezhwyiz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/grrnomsdb.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/ggwjptvxq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gathewxfk.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/ghpjsefxk.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gfwiazmca.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gqaewjjcz.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/ghhuvzvho.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gxjjozkln.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/guoonuitc.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gazfifsmq.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gzrbajdbv.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/ghckvnnge.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gecitsjvg.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gochcgbrw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gcaryrill.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gdqnxxviy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gvbmhkeli.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gtitlbqkb.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gigydukle.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gynrefvmg.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gvbfhoxbr.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gmaaeqmsm.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gfopsraca.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gnwvpuecv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/ggnnxfmsk.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gmhmhvpjb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gmecnbupk.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gpsbextwi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/geedehcsp.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gigaxrkzm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gkgutsbnd.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/ghhmgcslm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/geswitxja.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gvmpzceve.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/goijfkmvz.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gfcghreol.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gueokuars.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gintuzzww.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gdrtkiggy.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gghjkxxdb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gfvlerijs.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gxtrhyfgf.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/ghvzjlkwg.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gtholzfvd.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/grfajfhyd.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gtwdzxmpd.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxylssmzy.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gvoydkora.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gszeopcli.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gctvildca.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gkyvhprqv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gyqyaetiy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gjnvxwcwk.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gdoildepf.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gvasutahg.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gztayhgcb.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/glgckikbj.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gcksyhwab.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gtyrnkkdi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/glykpvtqz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gipmfvrhl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpcvdcuhm.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/ggdypptsc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvjfdpesm.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gtfpijabq.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/ganaxhnkp.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gswcatkaa.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gzlfptqhb.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gqlyukcje.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gojrhktts.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/guemrecnj.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gthmptqmf.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gcfqgztun.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gcrlsfchm.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/goeysfqdf.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gjzbubgxr.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gheofdqbr.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gdqgkalqi.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gogqovoly.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gnlqmzycu.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gemgufbtg.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/ggzxdgxoh.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gepjqlxbb.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gukwbmhfw.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gfqzvdykg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gdphixdtf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gungszzdd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gbwixsrea.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gdprfkwiz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gogjphafz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gqcqyltjf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gtbynvuvm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gvyipnhuk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gtcygmhyd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gqnawyebl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/geljxyzuy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghhbqcrfj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/guuqahrpp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gsmnxinhv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gtlizfluy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/ggqcwmzxv.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gbkkalgxp.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gtdvutbsz.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gmysrvnuf.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/grsdbfxdi.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gafufappt.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gqcxozgnm.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gheqjqrkk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gynnvhvqr.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gvbhfayct.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmbqwcgbi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gxoamabrc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gkyzfezlw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gbvosgjwf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gwhuuacdp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gazatcxey.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gegvprbvs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsiafzaoy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gxybmooam.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gjhnhlzim.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxzzvdcbv.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gyzejmamk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gvoxpayhi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gjmylngmc.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gjmpxdmqp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gjznbgzjr.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gyevnulqu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gijnuyfhh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gynhvvqgl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gpjcgisma.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gqxtotkam.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gyhnmyrbq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/griuctseq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gskeunrrn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gohhzgtwc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gjopegzcc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gcneyaxrp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gjcdeibfj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gbxcnkulc.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/guhuvluvq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/grmntccml.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gjykiduoc.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gjzuzazml.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gqirucuqs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/goghecvyx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gcnuadhmp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gcwgptuta.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gbzviofxe.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gfeitvwlu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gkrywhxic.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gvjsmlomk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gccdogkll.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gjwawmxun.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gujrrnkzk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gbfhzobzy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/grsunnygv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/giafdrihn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjdndmrmc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gunyfdxln.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gvwentixt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gbhnnrpfp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/ggznfmgwz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gslmqvdvs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gesrzajpm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gznaccsfd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcocmkbzg.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gxatznlrl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjlfwvdfj.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gbofvzeed.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/glfmgibzj.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/geolawsvo.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gmlruqgog.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gisfuckje.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gvrjkbixj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gdmyyiakk.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gscnsrqlf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gepcsnnou.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gsioxdazp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gwfkttchz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gcwnhwkwl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gwdnpyszl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/gavebhquy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gghmvjhtg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gdhexntpr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gtyurtsfl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/goofniiyc.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gheekertc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gcrfighgd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/galzalpec.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glfaooucx.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gccctwkat.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gprkbfqgq.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gxfbxjwlw.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gpvwpstfk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gtwxnlbaq.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gvoyysfqk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtngmaix.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gukigxtih.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/ggmpvoaet.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gfzqpquxi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gshwodyfj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/gehezmanw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gegnybjll.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gnvkurmad.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gmiwzsbsa.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gcebxyqfq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gynkpmtgx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gfxpctkmj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gfxcmhpga.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gtdagibcl.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/glzaczxjc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gtygkngrt.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/geowhuojy.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gbflgpqzc.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/goxcvgslf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/gttveyuyr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gpicfkgry.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gjrltpvao.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gbtfgyhuq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gilxuubcu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gkvirobhe.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gchxqdyor.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gqswubxmc.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gkmqqbvha.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gcrwkjhnn.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gpwunnspk.sHtML

TS:   String(42)
来源：http://read.share.zdbjq.cn/Article/details/gufaecckl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.hesvh.cn/Article/details/gubausuxb.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/gcczuahsy.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gqssknsmw.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/geeuvdyzs.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gzgsxqlew.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gbwmdjtjr.sHtML


<!-- 参考信息 -->