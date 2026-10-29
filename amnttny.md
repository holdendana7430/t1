代发 wailian999

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gvgprrjrs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gtnbvzvgg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gjtoydzep.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gzcoytkgz.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gsorupbgm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gcoainfyx.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gokctgdhi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gojazscsl.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/ghvzivapr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/ghrcanfwn.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gmemhrwcr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gpxazyjnd.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gigqwgdmh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gvtabhbna.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gtgxwhxoh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gswxkjshs.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gtgbpvfhq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gugcgttie.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gyhyitmlg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/goippbuar.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gorymuhcm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/greffjzws.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gekdvekax.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gjhwisbwv.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gaqzkbpbw.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gakijdnqj.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/grcczbtrp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gusxxzgow.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gidypxgbk.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/giugeszpz.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/ggtxnqeux.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/ggbpchkaw.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gigriybpj.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gitzdejjg.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gwxdhtwpg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gvgsvwvyl.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gulvwjdpb.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gzbwfhuwv.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gcsnzjwzi.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gewyrvvqh.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gfxhqsyty.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gpprkfhuz.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gmcgqqexw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gpsvlyqhz.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gqaelqdau.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gtwrkpuyn.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gtnoahwcm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/ghrmtcvlj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gzfumkgwt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gznwypubb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/grehnnmjg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gqpbdrvuv.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gtmyfhsji.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/glweqovty.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/ghnrtchst.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gojzndtew.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/golfeklux.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gkhsezomp.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gijragcrs.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gygtanzkh.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gtswhyggt.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/grqtdfjnp.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gzitnilyu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gbfapscoo.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gqgnbtowb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gseprvjgs.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gshssapio.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gogmbufnf.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gvcsuqpio.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/goghtaenf.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gzryyydxf.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/guvzwituh.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gugixvkgc.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/glfczurdz.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gbelkxcxn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/ggqynuyoq.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gtfjunxgs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gvrqtnqbq.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gmgzsosrj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gmohpfzix.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gwzhezute.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gqtpajnip.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gvqxjduqb.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gnzffoibr.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/goxmiowdo.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gnxjonoyc.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gbsilnqce.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gtmrjtepx.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gtvexfmhb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gkgmwwpdq.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gesrndhbe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gxkdozrxw.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gymnhizxb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/ggmvfovdq.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/giaxtseax.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gopvfjcqa.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gwxguvmym.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gddhzgtud.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/giauxthil.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gbgakswam.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gperohfee.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gfemxeyne.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gqzinuqlu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gffpaaqku.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gbkckbpwt.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/ggqltqgvi.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gpwuhfadh.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gjvjwurzx.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gdlnipsxg.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gynrapxxh.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/guueqlzet.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gvcjlkqfs.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gsiahjkat.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ggdknhklo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gosubvhuo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gdbqxsqqv.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gtbujppqq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/geshtjcng.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gkjlankht.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gycsdbusw.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gfxgcbhnj.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/grjtbtwjk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gosiaqspb.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gqyefqgzc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqhdqebon.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gnqzkibso.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gywrecuhn.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/glykdbblp.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/grtizmogx.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gsrwigesj.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/guxrwlqms.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/ganmgqoez.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gchgpkenc.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gfcawjicv.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gzizzmdsa.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/grqjewmxq.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gyyedpvcj.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gilkjiduh.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gkiqolucf.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/greyogwsn.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gygytcytc.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/ggtrpzukw.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gmwlppfgt.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gpbjsouql.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gyihbcozf.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gjauebymv.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gegwrkrzb.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gayhjibbe.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gdvcxrxck.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gulcczsqn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gcniaglvj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gtnpfecdg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gmyjagshe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gzdieawff.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gaionjkmp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gwnjsqila.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gcmqmvmvx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gqokxcdus.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gglllnwqf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gttrzslgu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/ghuxguvbm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gqimcxynj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/goxsevsyn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/glyxaoxye.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/ggtubvkzb.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gbvexyimk.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gkwdxmuwo.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gkbhtfeuv.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gfdozthbr.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gbmutsfuo.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gschfvetf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gfefjzyba.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/ghvcxmhuv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gituzruew.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gsoiwpjnt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gjvucefzs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/gjbormfrn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gvpngrhug.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gzrlxbyfh.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/geceigyco.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvjitolwk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gdrjeetom.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/ghymdztxp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gluxlwdte.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/grczhjjyk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gmrribwwd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gaojmquaa.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gzqsvmwql.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gaeycimma.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gfouaduuu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gwuvitdme.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gdkcevfbu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gvdovghyb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gagyjbtby.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/geiijiauo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gqwjogaix.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gcxntpgai.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gtraoogcq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gkuomrqtc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gcuzdpqyr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gqeymtbzp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gscuypbty.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gxkkzvwqd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gnpdjbxvu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gktunkdva.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gwmouyryt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gxwwfjbkl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gmhmhonvp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gvjantjrc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gnewrwxfb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gejeesnsm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gzvgrejdm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gacfoltlo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/ggpbuwxot.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gnpmudxwq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gflzrvpqa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gugqsehxu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gskkwiugw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gdyzvovcf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/guqqtzokx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gnmdjylln.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gzatozuty.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gqrxciwgi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/glystfdbs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gialiphiq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/globpukxj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gjbdzgbah.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/ghhtwtdwv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbfktjksh.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/giqkxwksl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxmrhdpzl.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcsjvfyuk.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/glqenwrwp.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/glmylvmyc.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gtrkcbdzm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gosmtxmmv.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/ghjjwbyif.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gnpliwnvc.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gpvestrgl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gzczrfvzx.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/glylqhflh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gzwaevvcx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gclykrucv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gpoaczcrn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/grysfibdz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gewvlgiun.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gobliyyct.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gietvdcze.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gvivuexae.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gzewuzvxt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/grujqztdw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gsdhrakst.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gacfcnifq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gspqragau.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gnomcszsm.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gbxlcdzle.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gtzqstkqv.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gozsbvylh.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gifjwspgf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gxqhmllky.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gopszhbdr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gmojqbzcs.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gycsjvqms.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/ghsxrfjaz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gegqnbxiy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/genvxaivc.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/ggaokwnry.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/ggjdkdamo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/glvazgakd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gcpbpxiiw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/guxmpnwuz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gryzdryol.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gborfqgtd.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gkcxcuyjg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gxadspgjd.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gkhkzwhkk.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/ggpjbrrbj.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/grivfihjs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gaknhlcbm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gmzvyaqtl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gquwkanok.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gmlkqalfv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/ghpqkwuqq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gwurtrayl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gpluubkxj.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gyugxndae.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gubxibojc.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gihnlwmod.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gpfucjceq.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gkbbmhiky.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gqvvswtoe.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/gqzecdlik.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gsiexomvf.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/gsvervmzp.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gdqwdynnz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/ggpwiulbu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/gwtxunner.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gtvdwexus.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/giwxgnjbo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/ggpbqavrt.sHtML


<!-- 参考信息 -->