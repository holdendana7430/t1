代发 wailian999

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gpstdpvhx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/godiqzuxo.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgclotca.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzytulmt.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/goveuavne.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzfzfqzgv.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gkubjwokj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrgtzudg.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/guaqomqbq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gazkbitfm.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiqgqpgx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgundhww.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gwxybioea.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpodxudby.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/giisbtkwh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gdjvoyzgd.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gagknrxcu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gaddtpbzu.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gufrtyjol.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gikqkfxgg.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxsqgetb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbocatxw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcpulohb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqsvxjxd.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gaozdayzt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gigvtmbcl.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gmsxqtdwp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhfvjqcz.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gkzgcwoek.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwhslqnf.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gjbdosqqn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchmqbbxq.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gairswfxc.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gmbfkcler.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/ghyjqdhky.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gpisfjlqe.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gvgivoacz.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gainzcpby.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeercpjj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfkimpey.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmynewow.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjawjwfs.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbnjjdnx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gvjjherbi.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gzorlkcjk.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gkdrrrpub.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/grorespml.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/ghbkeslmr.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/grzraneuz.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gptaojhda.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gvclzvnqe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsijmoqv.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gyifsytol.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/girnrghse.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gkykmepoj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gjyrgcges.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/girkuyghf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofqxalim.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gtikbntkv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gssbmshph.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyjgzabq.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gjunhkstv.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gdnmqytbp.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gunoogzlj.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gqjszdrzb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejgyuezl.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjfykmka.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goykycaii.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gvckuakxl.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmotzexl.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgjbzoov.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgxepjgn.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbranhmq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzeqftvt.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxtpwjpw.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvcicdox.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gyubkyfkw.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gropjwzcv.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gijoazbbw.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/goktkdiwh.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gphnuyjtu.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gixxktlyh.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyirpqkuc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibdkmyje.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gsucjhnab.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrpkgtmm.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gkezfqmrg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gdodihohz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgqvsrrr.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqevkunyr.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/guncnzykr.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslhzxqmx.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavpqnwoe.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgwudppv.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gaebztvyj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxuoditw.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzcfrjad.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gzchzrmot.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gltkqjwwr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtilopny.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbecttaa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqnckfwy.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gakqgxqny.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/giemqocfi.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gtwsplnyf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrexxivf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxmaafpb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gxyckvvzj.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gucfpitgd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gyjxiamqt.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrwutsgv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/ggohwhqac.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gxunkstxu.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gduffycwb.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/goqwjzcwz.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxhovzxv.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gefjatxlq.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gywnadaoh.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guitezoty.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgvtjarx.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gdxfxqidx.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnupyjsl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsitvvucj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/giiinycip.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gnsaguuzs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsedqlpo.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gtleukgav.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwalesjx.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/ghafkikzb.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjwmtahi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebpsbone.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/grfvuhqtj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmszlkvt.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbukfcccd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grcxnbgha.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gchrhyqtq.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/glnvyjuum.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gcynklwmw.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/glccmxgss.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/grvxpyovo.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gwesyeaxm.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklnricyq.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gefbfagfo.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlvdhssw.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqydcszp.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/glikpfbgv.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkryurxb.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gutebgomu.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gufmhyrsg.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gyeiunjap.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkiesvcn.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gxmfvwyap.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoibglzh.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gizpdjhxs.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gavdskuls.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gcyvrisbg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhsoxavl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwhoqvct.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gunmexwbq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnhzjbvu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gugubnvpj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gezllppdt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gnvgrthux.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/grepiqiqm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbvfsjyz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gsvbvgkbp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbxhczfz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gluhawoll.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gqndjlofm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynwlkibt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gmrrqegwc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/giowgmsyp.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gvzdtclmz.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjkmbkhn.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjwxeerp.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gszzueywk.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjefegya.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsbvvneu.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxpcjkui.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoymkevf.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/gghyczotr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfcsongf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrrktwpv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwumyawc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gahbtlxzu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/grydpuueg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gkjeyvcna.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmgwrepv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyvrcjbx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/gbnoxspfg.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gmammztce.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemhkgfne.sHtML

【收录内容】
来源：http://mobile.fanxiaobao.xyz/Article/details/gurblkrjw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gvezjfewd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gjufnzinp.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjmruphi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/gnymlbqqu.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gntpipsoe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gspexguhy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gxahgefex.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gfwpthgjz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuqgayjn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/glswuyguu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtsppvxt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvliihwon.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/giwgdegoy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxffpgjl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gmxgdsqcm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/giszzreht.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrwloler.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gzpcsiizf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqainpot.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdxdnoil.sHtML

目  录
来源：http://read.share.fanxiaobao.xyz/Article/details/goqrzqpuj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/grmfdjoox.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gdrjoiflk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcguvbgz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gdzmbmjxt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gevhcqbml.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grvjryqoc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuvymfxc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gpstnqgzt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gubwgqeoh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqcgagag.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxadcssz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ggtulhsgv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gpnpooecz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/goqrazers.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkaibkxz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gnopnluil.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/grmjjqzsc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fanxiaobao.xyz/Article/details/glsepwont.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gybfbvmeb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fanxiaobao.xyz/Article/details/giapgvfxf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbprabft.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzskkkahi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqscihakz.sHtML

A. 基础语法与类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxiydeca.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gomfeaocd.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grnbeojpg.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqufluxio.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gisufyddz.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gnhudmspu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpenairua.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gkeosjptp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjukpbfi.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fanxiaobao.xyz/Article/details/gfcxayvlu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/glyzrodsb.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqukbzbvk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fanxiaobao.xyz/Article/details/ggsgunreq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gfqravqmr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gbuwwkowm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gqkwlxoup.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcowzwgge.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fanxiaobao.xyz/Article/details/gxrapoufi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fanxiaobao.xyz/Article/details/gdugzofdr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gwfifhikv.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcgmtrkh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcnpittb.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvuuueel.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteertgwc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgsfjfdd.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gspurplsv.sHtML

Go:   const PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gqgexygrq.sHtML

Ruby: PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gffpzdxsu.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gwovfvxwf.sHtML

[A04] 判断变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjumafaay.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksjdlyat.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhstihgu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gfxcfkuhe.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqutrgoh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpqlflci.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaeehvwo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fanxiaobao.xyz/Article/details/gwkxfcumj.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fanxiaobao.xyz/Article/details/gkvvtwgzx.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqpndkmt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fanxiaobao.xyz/Article/details/gdyaadecf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gcmqtxmfm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gakdjnmuf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpswgehlr.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxodqerct.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpxrksyu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmnhjvqz.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtvjjnmtb.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gjaphkhou.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfjzelpt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyrghbkk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gogjqupxx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnmtqnhx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucuvhntp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/grrcvypyc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fanxiaobao.xyz/Article/details/gnylufkwm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjomcizc.sHtML

[A07] 数字转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmleodjh.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwunuiot.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtwomdyd.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gdbjhfaml.sHtML

TS:   String(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqaqaqgz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fanxiaobao.xyz/Article/details/guwudnpym.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gwkrbedbb.sHtML


<!-- 参考信息 -->