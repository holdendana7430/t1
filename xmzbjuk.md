代发 wailian999

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/ghlifhlya.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gavsoytzg.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gqpqjxnrk.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gudptqmld.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gzeubmeic.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gktppxblo.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gbvslunzs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gxhelokfr.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/ggolohhzl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gxrjgkysl.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gfizjptzn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gnbuwrmvm.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gmxeygclm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gadhamwtm.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gcrgvuuxt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gsdhzemos.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gedzabzlb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gvidrkabn.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gfijajklq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gmhfygyme.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gfqbkbwmy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gssmbbtkg.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gctxntxxe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/giqiukviy.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gabyufbhj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gsvaaiicv.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gcxnnzxqm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/glmujdjxh.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/grhkgmsez.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gvjszwura.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/glwvqggcz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/ghicnyjdx.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gcldmwykz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gdprdvqor.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gsfcuaysq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gsydlqkcp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gdjsvmtgx.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gvtznjkdf.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gmndtzxzu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gvuxqbdzm.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gfmuwuhrz.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gjoruzevt.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/grnjdytel.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gyqgdflsl.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/ggopamapp.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gvlbjiwkw.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gfqkqkhcl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/grcnxmcis.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gbnzgddgm.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gjebedheg.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gszmxgfew.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gngokdktn.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gbjtlpefg.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gzzadiyrv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/glsmhvfde.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gqayxpvne.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/guntdcxgv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gwbrsdjyx.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gnrxtggyf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gunieyfnd.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/geqvattxz.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/guqprksqc.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gijhpcapk.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/glekliwzf.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/goffjdcwl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gxfietizo.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gicxgiwry.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gwijqcqwc.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gbmmlqasg.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gmvnqnodk.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gqxkbtugj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gtxavvokp.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gukalcxoy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gdmvsdftu.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gpsgjwqft.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/grwgztvxc.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gkmgtlakg.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gmuxwpflb.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gnrtgifaz.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/ggukwygbk.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gaensrgol.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gpqkhbxxs.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gtwsdmafs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gpwqzfhdd.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gclgjvtte.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/glwmlzoic.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gpdepbztc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gwuwmsfxa.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/guqkeouhu.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gomgfvrla.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gwsnecqux.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gvcqwtkhp.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gknrqrgom.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gzbueekfl.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gcgtkkasw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gmjhafedq.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gnqikfoyf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gmtpxoqch.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gtltvirel.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/ghpslkrll.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gkdyqhyww.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gtawotfkd.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/glfxalkfi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/glrgcfybd.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gjzelucnd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gnponkaug.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gocxqqzyy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gvciwhkzx.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gkktqauap.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gojghrgqh.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gljgzejns.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gelcpbegw.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/ggbgbehlz.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/ggvlrtave.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/goctvlvzi.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gqccdodcf.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gkctelvop.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcqxgwbfc.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gsugvjhhz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gcfexbfzd.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gjezbfhbp.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/geaysrsvs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/ginsaoxnq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gufvzquhj.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gbblmkzvn.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gcybvokbl.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gdkvkrkgu.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gkzcdocgy.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gjxylxlkl.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gaclglwgm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gdyxtjpyq.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gafdvlmxu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gijomxlih.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gvidivbbz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvnuzoluh.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/grourvbjo.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gxezfackx.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/giscpevjz.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gpzhklskm.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gahdrkmak.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/glnajxwdl.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gglhipiaf.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gfuckxsau.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gozyqlxoy.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gnahdeneb.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/glfaiouzt.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gzwuaefye.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gcrxdfmao.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gkputnfeu.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gzpynygsv.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/glmszjpmu.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gqzktedkh.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gfeepnatc.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gjegrrmmw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gahrobouh.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gpedrybmj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gfftjctzd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/geserfkrk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gdlvizrqj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gjzjtolbt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gneeppolc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/goedcudpa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gcjpkknea.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/ggpkagjej.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gjwwuxrma.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gawetdwgq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/grsjtaukn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gziqkocqf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gnfqrbwwc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gfbkxbzqd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/giaapvxap.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gckimsczc.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gvxakdlyy.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gbydqyeqs.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gxxmbiswb.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gedlbtbjx.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gxvokitzb.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjllmyxkb.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/ghfsbcaof.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gymdpqcjx.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gxdncpedz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gxyyoytzd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/ggcczymvc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gmrxmcfzf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gqdrxntrw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gjdniimmg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/goijfivsi.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gfdqebzqt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gykcheigu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gkmwhbqxt.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gwrsvyitc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goodkpfpt.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gyolgxhsl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gwjbaqcjc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gngpsxzwm.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gdwpgbsif.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gskdwgibm.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gtapkntna.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/ghmcvqnze.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/glkjniaqf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gkbgnpikx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gnpilagva.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gvkgyslnf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gpdllmzss.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gyydagkhg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gsdadilhd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/guayuhgam.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gijdldqli.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/ginjebgts.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gwcsmncqf.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gcscakcdj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gjbxjhmqi.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ggeyemzcx.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/graivycav.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmhdfirmb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gmyixrftb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gtfkxparb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gzxnygwju.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gsbyawlrq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gzqpoxqfg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gdzapcujb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gxppxnecq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gpwlsvsop.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gwccviigd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gfgwtlgnw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gqpiymcfb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gfaozmbjl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gecggbalv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gabsheeqz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/giewpqtya.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gkzkzkwnh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/gkjgdoinl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gqvvcdamt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gvpfjhyyt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gatmwxbuu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggpacasac.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkqyzywpm.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gbybucqbv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gquiwgxbv.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gejntrndl.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gfzkiopzz.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/glavwygkw.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gxubnmheb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gwlyxmvhd.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gxdludwzw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gkhumddro.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/glwhjscrk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gtyeebuxw.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/goqrabfkp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/grnhqruhl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gdlrmouli.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gmphvrfuo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gquexqpay.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gvfnwdjgf.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gnypcehcs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gfnxdudng.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gutunohjl.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gbopnvgam.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gqevkppkw.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gqsfekosd.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gjpjhafdx.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gifiyjnuw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gcnrjjyrr.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gdfaasxeg.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/guwocshqk.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gycfsggfc.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gjocdgqog.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gwqoukuuu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gbcirfppc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gvmqxnlfg.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gecvwzawg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gdaxlpppk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/guypflyyo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gbpclhjlt.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/gzkvnoekb.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gjgyqpjyr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/ghydzqlrs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/grilbktie.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbfdemhnx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gmgicexiq.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gerxfmijn.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gjkydchtf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/geyzpqqrj.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/ggkavbuvw.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gxsmgansy.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/grhybgqxd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/geelgboqs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/grroedeaz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/guzsjrkyf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gghydntgo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gjmjntelk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gvudzbyho.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/grvwjlohb.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gjtygluus.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/geqiilxcd.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/giwanyfze.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gohafokit.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gnlzmspjx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gjdtdwwbz.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gluwfratw.sHtML


<!-- 参考信息 -->