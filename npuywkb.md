代发 wailian999

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gsgypttjb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gzmshevvr.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gvlmcioke.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gfhppzmbp.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/goyaoznap.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gutuveyuz.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gmemsdbar.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gomlwtcxy.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gcglfvmtp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gjqlvnvqw.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gkdribpnk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gmmayitik.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gmqxjxiza.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gdhvkpmex.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gitkwqaka.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/grmqwnxlv.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gfiibhmyf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gjtrmzoef.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/glsnkbstz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gejjzwzvb.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/ggfwjveit.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gydqiukpe.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gnajkcpqk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gpwgcyvon.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gxatvnvci.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gbsruabcs.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gratncitj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gwoksclzl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gtoehazhw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gwstkdxzf.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/grapzlpmb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gxioitxnt.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gwkqalzwq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gmhoolbso.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gpcjetzlx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gmrkolixs.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gfrlzqpdg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gbbibfgtm.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gycutobav.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gliayqlon.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gaumuzgkc.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/ganvnfwfz.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gjmpjrcef.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/ghthhcrbk.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gismpewma.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gestigvjr.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gwigphflw.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/glojykmsc.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gwwqgsojr.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gtybfflre.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gytotrvfv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gxflpcrfe.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/grztwmmoy.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gavnmcklx.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gzhxkosvp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gauvcwzfo.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gbsiqnhwx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gyuqzboto.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gtrwkdsst.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gmwduvmhs.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gfasbnebe.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gncjjnwmd.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/grsekxiqo.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/galikraog.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gkibvebzd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gsodkzved.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/grtsspbed.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gtzgacbto.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gkuumeoor.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/glmwlhxht.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/ggwpmhdcv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gctjzdzoc.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/guytlliyo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gwpcxdowh.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gezvidhrf.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gbnkzayep.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gdijojpwm.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gcoepbmxr.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gquxtrirj.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gaudkelbm.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gaamewxzp.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gcoiiztou.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gkprrhvew.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ghcjfxidm.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gfihmeele.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gkzpzkinm.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gkskrcnec.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gsvamegxd.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gchtktfbg.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gsogolhbb.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gynppolew.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gacfdsxww.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gwlatrcpn.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gwfijstpe.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gsgdpxipb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gdfqurpxk.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gbacmxnlw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gborlzgbc.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gexdisbfl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gjbbwfxxd.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gubmvdwqk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/govwimprx.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gxbpxngna.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gimtoaysm.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gmyjoseua.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gfzmapdbi.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/geheuccxa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gxjicxdwc.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gduvkepuj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gtmtihqqs.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gwpgomzid.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gmytehnkx.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gsdynwyam.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gqoedxgxq.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gadajmevd.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gsmnvzqlv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gyzepmasv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gshjspdgx.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/guomypqoi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gislqklxn.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gquwdjvyl.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/goxpohyab.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gwozqevri.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/geofrotvs.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/giirljhhd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gzowukkmf.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gjwuqeobt.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gqwdalblb.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gfcgyyfni.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gwwxqedcm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gnckaeflp.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gtvvnebyh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gseyyunbz.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gzdosmhwb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfjggksuf.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gxusgurej.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gsielfckj.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/glzawptbf.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gxckcslyf.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gqwcjllkq.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/ghaiivkob.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gfgokztpp.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gssvliflf.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gqiobjlqx.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gtnaijhhe.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/guzqfvkuw.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/glxkyzxvb.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gzjjaodbe.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gsfqcsdpz.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gkyjsuwbf.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gvzlukrtq.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gbyigzkdr.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/grkfnkofp.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gbhjiclav.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gglvocbgo.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gxyzffbde.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gwsflqgag.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/guhepwjgy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gnvbivxij.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gxktrfjcp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gcvmkjphs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gtwcmhmbf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gcmarzkhr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gjrngllvv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gycpunuky.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/ggmqqawmu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gwgjttaeo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gjhqzmfvq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ghucmjhhc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gkxvzyujj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gqjqhbdco.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gtfhqkbeo.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gmaajuyop.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gvqflysfz.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/geczczhkn.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gpjogmwci.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gtlglwnev.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gsdhpujhb.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/guttbaqbh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gvryylhdg.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gebteivvd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gtugrrqex.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gicghqqzo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gpiymxohb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gzjvtregl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gjhlhzyqq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gepqfhfrg.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gfariiwrg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxljlhshx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/garyihqtr.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gxifmstjy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gclwomcwl.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gcunszprc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/guywdpqym.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gsyjxoplq.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gzslsotyj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gvoboealx.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gnbgeoeyf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gcdgmokuy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gcofjxsql.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gdrwedtxj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gsxlyqbvo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/ggjekfjcm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/ghmlqdbgs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gpfpumphl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gvetqtnop.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gfriikgbb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gxupxbtmp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/groythwka.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gjkwiciyx.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gqpuvcnau.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gfvnjeymx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gegmfwssl.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gnljfoxed.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/goksgasvt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gwexarynn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gtmbxdowt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gxeikgdkx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/ggdauiydm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gvmtnmubf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/ghcmbmniq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gqikuzywn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gnzlfoiua.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gafukcqri.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gbfbdctuu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gshazbzxo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gafzinhrc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gxebawazr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gydxjarfz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gtbuoptpo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gknwvjjoy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gjirhtuwb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gxkqzvxri.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gdrbfcnne.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gcyeblqai.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gaxtrdnxy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gomehajsi.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gjtabfeoi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjbyubfwx.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gsqjgdpoo.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gjyncrpaz.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gjgqqzwst.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/grokmexho.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gyqsvdzye.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gngcjrmjf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gtlcolllz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gksjyebhw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/giozktsww.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gkuzocwrm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gxplugwda.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/giyxcjuuw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gflmavvmb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gzgfawfat.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gvergzaig.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gxzgzgegc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gemzprgyl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gjbvydgmo.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gblpnmfyi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gcwmgpmaz.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/goxcaipkl.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/grtxqpojv.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gufpuxrdt.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gairpyhrv.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gwedmotmc.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gjmyknyoz.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gzgxtyiuy.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gtbgbocvt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gxwulgufs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/ggsxtydof.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gvrfvcuqc.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/greybvjzp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gdokfagct.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/grbaozzms.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/glyybduik.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gdbjoksmv.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gwydcgrka.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/gdsvbkmox.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/glgcybjkg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gcagxceco.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gbeoblyux.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gsfqfjegr.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gveaawgtu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/goddcfckk.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gvfeokijq.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/givkstpob.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gazuxtlgj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gotrdidbq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gcatrnzop.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gyotmhvrg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gixkczkhh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gllvtfpny.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/ggmevqlwk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/giemkcpsy.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gfhtxzqiu.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gplttpdot.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/ggitkzzsh.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/giowderxw.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/genbqytao.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gmtpnatvc.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gafhqbbta.sHtML


<!-- 参考信息 -->