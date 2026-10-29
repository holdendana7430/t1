代发 wailian999

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/ggaxyzfja.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/grckcduem.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/ggjthhyuy.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gjguqfzuj.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/goiihvijj.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gxkwhlbxi.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gbxygsagk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gvndecnrp.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gtjsqidho.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gfxzeqdul.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gyrxqhgtv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gnvojfitn.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/getqqhyaf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gcxlytbqp.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gpzxprjhn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gmuxdsvir.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gwqvxvdck.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/ggeapnsvn.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/ghpciqrlr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gfigjntam.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gmdukemmx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gexvvowue.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/glidrwgyc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gnkshawps.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gcoznxgma.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gqbxrrlre.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/ggcztshgq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gdmuycaxm.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gctumvaub.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gldvxvwtd.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gvvxbnybu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/glqayjcqg.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gqxyaphfj.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gzfgpmkqy.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gknopxunr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gcpohcyis.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gpdurkvpb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/grktmjxpj.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/grbwpljei.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/glsoticdb.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gvlysoase.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gtreevpvs.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gbmdlqgzm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gwmgpwtqt.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gtzkxbkxz.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/ggzspogmg.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gpugeonns.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gcgrdavhf.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/grcpulqys.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gwfidjxav.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gealmjenh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gpbqmgcqh.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gijrytcos.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gilecpemo.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/glbrpjiit.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gancmxzpu.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gojdzjloy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gtsupbcwj.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/grpztdqta.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/ghrllizjx.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/goedseifi.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gsptjihjs.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gomqqxxrx.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/ghiavqhgt.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gbbtehtui.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gnerhwysr.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gjgmuhqog.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gvuhtwjtz.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gdyruszdc.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gcyegbxze.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gxunddpsi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gzaayqejh.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gzbjogfwj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gjxmzwqhm.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gjurboadt.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gyvcyknib.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gvgdviwdk.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gyuedvebd.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gfjjgppmx.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gvwqsqncc.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gkmdbsbez.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/glgduhgud.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gzmnkqnkb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gzsmfzblu.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/glrazsqgs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gchlydcep.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gzxlcubvb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gtmdkpbek.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gprlxtkpa.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gllfgzpzg.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gydgbcbfp.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gdiczeltx.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gajqyqfot.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gemwjwsbo.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gynnzhhuv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gughsllyf.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gxinhpshd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gofpuunsr.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gnllmxrmy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gizaiekfo.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gizqdkwrl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gdkmmmgxu.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxahsnlbd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/geqmmivql.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gtgjjdotr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gnyykxiep.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/guplzvhbi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/ghcjeeoxw.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gptqwcmms.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwrxesg.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gfhlvmjka.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gyaoqbroy.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gldkkcvea.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gynyeocaz.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gduqcsega.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gxrlhsjds.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gtzihgixc.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbznmcziv.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gnncwweed.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gzdhjyfow.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/ghszjshfj.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gdreyspuh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gscxfxzms.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/grucdjrjr.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gtofdqfpk.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gvtlmbbxd.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gnjtwttog.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gbmowafzu.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gvgbnzhwl.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/geojcqmic.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gqehjnlhg.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gnjsfkhmt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbbiookzp.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gygzuhbrt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gstabfwwr.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gbtwfqmzm.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gcwbvfptr.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gdvobpiai.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gxiwdsemw.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gwwwupspz.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gkvivpmsq.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gzxzoqrjb.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gpnpdfmjo.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gvpkqnqnm.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gpteshvhi.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gvxbfcexv.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/glocsukff.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gduzalmsl.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gcvgmskty.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gzeuhoosq.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gixcijvls.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/ghxdlkjwb.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gmrxqbmbg.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gntgdlmwb.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gxufqgvnp.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gdudbkizv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gtmhpgguv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gadxmwxwq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gkdmvwkdu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gtxiozzqg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gtmvzclic.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gyopedeam.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gpsfjewmc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gkzunkqkw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/guaithbbu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gmxqabcgy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gjoqrgvho.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gtkumpauh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gluaaddfa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gucszkflf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gwjergskr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gydtgsqkk.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gzzkjjpad.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/geadizcby.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gcjehyolq.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gkywhaxaq.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gofmktaaa.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gwzwokvpd.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gnmtostyr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gvfuowisz.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/ggurkkdkw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gbxfzzttd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gsfbastsm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/ggujrdtip.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gvmzlepec.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gpfxkujns.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gwgildyjl.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gkmoiiszt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glvicudnb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gqmwkbfwk.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gznrpodug.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdwgktyyx.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gxbbzpbax.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gquiahsmt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gydfobzza.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/ggaalhsna.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gvpzhqfku.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gbmuvrkre.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gaprejnxj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gwohxhqnq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gqundhmgl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gxrpihely.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gvqulkyjd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gdfpjzugr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gqwiaxcwd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/geurndjqy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gfgyngkio.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gndqmdpzw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/guaoyomyu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gwclltlkk.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gwmudhaap.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gdbawssrm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvunvzwbe.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/grjlqnurw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gynedclfy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gyxttygip.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gvnvunnsp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gqabwtosw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gwlanmysu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gwritqgje.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gzeavwyvf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gbrntnkfj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gtlbhisjm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/guaggtrcv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gwjvjqqsh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/geryjbwjd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdpiiljru.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gllhskjsm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gqmcmnbgs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/ggmqkrhpj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/guqvynnom.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/graycmcoz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gvkxpsqxx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gjfrowket.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gxgdzymrd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gymjzuxel.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glemfpoxv.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gvzbmiubk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grdulxuyf.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/giwfhsteb.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gkiccpzax.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gwkkypvvz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gmscfkjaz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gtkliyxop.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gzktnbsul.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gzoseslxd.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gdyzmfzws.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/glvsmlsxp.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gxcmolqde.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gnkcvelry.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gmfdrqmdq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gfoehetsf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/gjedkjhls.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gfkfztpip.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gdxgxxmqt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gwkxuvqxy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gbfdtneah.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gmmkkvhol.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gpmjjjzon.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/grhkvijvl.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gdkbknwzg.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gwkqfilfo.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gkytuwnlx.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gclmubgiu.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gvpxezcqi.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gcxfylfcf.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gdhhlhzrh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.zdbjq.cn/Article/details/gguygkzoa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/glssqvvvc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gfuqcnhka.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gszpootwb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gneqmzkxc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gvgedinsu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/ggpodykxg.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gdxrlfyhm.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/giaalumgd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gbevuqbbl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gfzyisxjh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gzlddekzk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gfslxehba.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gctbjxchr.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/glzbuwsis.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/guxdnqaqy.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/galwjyqki.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gibfwvuiu.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gyhirblty.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gefzhnmyf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gakpbytqr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gydwifsfh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/grzdokqpu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gbzhcreof.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/gbrydkqjy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gxucynjly.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gxzbxpfnl.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gyzxuktgm.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gcijrxsxz.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gcadsvyuh.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gidqvrsag.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gdjqiuvmb.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gwmsvkolz.sHtML


<!-- 参考信息 -->