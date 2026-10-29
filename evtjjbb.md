代发 wailian999

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gatayuhnv.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gwsyghteq.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gqyrvolkl.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gygjevvwb.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gyrluujab.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gpmwixxab.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gnhlnpaxn.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gdpikrvky.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gkzxvyafa.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gmtcbflry.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gfldvarky.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gvrfdfwho.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gyidcfgpo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gdogoiavl.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gdqopnnbz.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/ghkjpdwrq.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/garivrblj.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdhnbpvnd.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gfxswgmii.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/ghyfsllwh.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/grdnbtaqs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/grrsovqju.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gqejpwipv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/glcgjbnjd.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gmcusctdr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gtepgejxz.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gegpggmsb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gccfygran.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/goeolbxkf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gwpwrdqmb.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ggckkenvj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gqfmjpcgx.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gzepkpocz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gddbofeqh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gvjahtvnx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gqzgafsvz.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gcbyunhee.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gebihpwrd.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/ghowlxgvy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gyyumtlig.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/giiaexqng.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gghchrmor.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gfajbeowu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gskdgzxdu.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gzgyruiob.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/giewttnwk.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/guylyigsv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/geaeaxfkx.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gtudghlgv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gqkwatrgo.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gddbtzrnt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gkqzfpxjz.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gifbrwleh.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gglaanoqw.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gblyhweqj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/goubsaktz.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gfknxicmg.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/grrptpvys.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gizmppwvj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gqdivdaqn.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gqrpcvjus.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gqlnrwkjn.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gsugdccwc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/geyhdyneq.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gqaduwphk.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gsuwmqbaw.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gsozupqcl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gjubwaycc.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gpdmppbhh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gkdvassbw.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gamyznjfo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gkgryllln.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gsmzdtvhh.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gjzxuibnh.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/ghdogzotd.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gorucbebz.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gpbnwepxp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gyasqapiy.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gbmtwlkjl.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gbsvbtsfv.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gdyxeowed.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gcmvlzsqp.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gymbhhkcl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ggougsexy.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gtsyjmtdb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gnyqqbdto.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gdzyodmfh.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gkkdppveo.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/grcrgsmqo.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gzmhafjua.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gcmbjcnof.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gncldckvl.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gxgwseppy.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gmidcbehe.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gddczrfge.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gzlwqwkbw.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gjvqhherk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/glcxkgovm.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gsbcsevod.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gmigbjomy.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gytwhbdif.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/goczqbqfl.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gbwndnguw.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gopniajbl.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gkdnwlznz.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gddlkugaw.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gtqjckhza.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gzerornil.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gwlaczogu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gfjfjwxyj.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gdspnldkf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gzigzotpf.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gntkwjnoj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gholoorni.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gxkjhfnpx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gjbcffmwi.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gqyqscjze.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gqzosdpyl.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gtvsgttwq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gipdbtmvr.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gbfxwkurm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gcsybwwpf.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gcrquysxu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/ghaezrigo.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gzietoztd.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gecdnyhfc.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gxcnvfgrt.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gxgsrisbd.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gixwlarrz.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gabyreipa.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gzgkdkdls.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gtvoevfql.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/glkfkhdvg.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gzxpwyvdu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/glpjwxbjl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gbdioogce.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gkjkcxogk.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gptgeohwv.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gsebkrwrt.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gbrfjjbsd.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gihlswdhm.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/glzklrxaj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gvggimxko.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gvxyoeocn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfngcxjhi.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gdwqnsqbw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggdekwjtd.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gsysloknm.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gtiwevxvh.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gdqjmdpsg.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/grfnqbeja.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gdxoqwwye.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gypdcraej.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gzzxpfqyq.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gmyjxouea.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gnsusrqfx.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gheygayyl.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gibhnsysq.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gmvafcoda.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gtgunnxpt.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gnkbsrvvw.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/goxqawjsm.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/grsnvpgex.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gyvqesmhu.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gbauyehpz.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gdyxxjlns.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gfbzjziip.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/ghncwygep.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gfmbgjupw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gikxygyia.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gubyokjzu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gfidrohxu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/ghcsrdpik.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gjoepujjq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gkitzbogv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gifourwhn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gznigkxil.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gjakdusra.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gdqsyjgrc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gbbaejuuc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gxkwgivyd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gickowapx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gjzdbkuuw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gwkrbjnok.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gecmtaxbg.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gdosvucqk.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gfafttvfh.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gytrskqpf.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gkvlohosm.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/glghtomlw.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gfzpauyne.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gxvqrercb.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gscmnlxtq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gxwiyqozi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/ghgjyfuri.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gfqbwmuzb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gquwlfgea.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gwellxsaz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gpyxbshwr.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gassskcxf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbsghokuy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gboendgkq.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gwktasxkd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnnkkedqw.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gvryklrlk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gdhigxmub.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/grwhgucdz.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gknhnfsoz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/golbomrjj.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gcplmpjvt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gpxljwlwt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/ghhoxvhrn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gwseaghim.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gwxwvbryh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gueyybodw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gjbuihoqt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gofjozsev.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gzgpmeyqz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gcsgndocc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gfuoyyqhn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gbdnahmix.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gzvoilwvi.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gyndqsfoo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gmjsziwzh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gqxdavkxw.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/ggsshnscy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gaagsppuc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gjihlzgki.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsokgrovb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gydjrdspt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gihvmkazg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/geqqixrrj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gdaakgeyi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gclzlibtb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/ghyxeiybt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzjhswvrd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/grrcewjrh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gytvfxgce.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/grqabhrmj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ggvbasvcl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxmtosiqe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/ghitzwonu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqbheaapu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/ggghmdzgl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gabzyohrf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gyawtedgx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gfesatfwv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/ggxyxhawk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gducwnfkg.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gqvbrvhfi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtcvaqtsf.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/ggivvbdye.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gufhijwph.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gzldwuubj.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gcfwfpsup.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gxlhadnge.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gejinwhul.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gqkprjvdf.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gsolntjic.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gypzylism.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gskdgdejw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/ggdpiobdf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/gmytbmluy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gagoqsuig.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/ggzxkhsrm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gmchacctz.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/ggqcdvvvv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gfkcgirbn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gutowazmu.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gptacbygf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gipfgcrcj.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/guvfgoarp.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gyvstdagc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyvvfafwk.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gndzgmeyg.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gfafvqblq.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gfobzpjfy.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gnyrexprw.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gkogpxiwp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gbjymncvu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gyepnjdym.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gzsdddwkz.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gqwxcxsby.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gcwnokdcg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gdswgqgkj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gokflofny.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/givcporfw.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gdtfpvcjo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/ghbwkiqjy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/goifpboyg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gwdhjkrjt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gefrkucuo.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gtqxbmgbd.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/ggzgpomkf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gzewknono.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gwzmoqyca.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gtqfimvdz.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gsgogtxne.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gaesnthxn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/ghalrlguv.sHtML


<!-- 参考信息 -->