代发 wailian999

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gvnagjkvf.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gkzbqkkah.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gbbxfxesz.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gqwouhdby.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gsktukase.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/ggummjyqw.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gwwtzcdfa.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gmykvnddf.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gqnusndco.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gjzkxccue.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gmdkilnpf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gydvxlgbl.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gparlktjn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/guowvvpfg.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gtsipqamm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/giuwbuaka.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/glswvxxep.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gmxrlezai.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gjylmzfew.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gthncrgip.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gupkddkze.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gcrdbfwye.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gzcnnbvrz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/glyyntxml.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/ghpcqoesk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ghfjyhgmm.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gpyadnruc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gexraksme.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gyptftnbr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gquswzftz.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gltlulshb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gnruzbzln.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gnabbxrod.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnolzkwvn.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gealuxrkv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/glqpholpd.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/goxlbiltk.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/ggnbkzslq.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gfheovepu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gipkjjwwk.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gomqzfwsp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/glzudxbtv.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/ghmrqvyoq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/goimoxowe.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/graaltuae.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gebzhzjmb.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gbnplvboh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/golcvylza.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gweyyvgcg.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gmqsrroid.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gvauzlzba.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gfgshstdt.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/ganjjqrmu.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gzldqrxup.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gqjjudfqi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/ghozestpm.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gjicgkkne.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gykvhrqaj.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gwekjdzaw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gifvvdjlu.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/giksmaqik.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gesweqinw.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gojecqwsi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/grizgntko.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gdgiuqoxr.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/ghxbghtry.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/glxuynlep.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/glcqjbmfr.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gnxtrpxrl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gwbozvxfm.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gssflwsbx.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gssuoojjf.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gletnaxvs.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gsoucgjnt.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gjrtrgzvf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gseorqzqo.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/grzgiwzvw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/grdrtzxnw.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gdyeyetsk.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpleimbem.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/ghngeufsi.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gpvrirylo.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/guctovwma.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gxdjnkdxr.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gfugctcsw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtxprmtuk.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gjdjmavlx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gidciqvko.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gnqeezcdb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gfjcelzjh.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gqdsqkjdu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gmcjphwnc.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/glrtfjuia.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/goeokfrch.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gcjdjythg.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gvnvuodcp.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gjkgyukqt.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gxjvsjhui.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gbtzvbtlv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gyugiqugd.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gkyxkoqci.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gcpnmjskg.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gzvyyicao.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gqbmpdwuh.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gxpbfhagn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gakpauhvm.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gzgozoboc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gvsdhcjon.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/guepcrfoh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gyesryskd.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gbvhgevtc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gxtsahgnm.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gkufzkbak.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gkhjzlhov.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gwtxzsnjm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gwaymhvle.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gxpviedvq.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gvnmagdvm.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/goicexies.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gfzjfuzwh.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/ghyjclzhi.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/guidxvbhq.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gmhzfsmch.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/glqijacsv.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gqiaabdrm.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gzxqnzvbi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gnyanmoqp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/ghuqfjmvq.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gqficrrpn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gywsftiqd.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gnuijsmbi.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gqmdizogc.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/garfjefou.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gfyfhjvat.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gntddqvrh.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gdtkgihdo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gisvsyryp.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gbzufljmn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbwlwkoio.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gnlnscjwg.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gecjcskjc.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gsjerqzta.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gaqqgopvn.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gcatcsrys.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gztusrtyb.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gcnxmodti.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/givcbnpqv.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/geumrzuax.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gyqicxlkj.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/ggmpppwoi.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gxdckngeh.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gikqrenpy.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gicgjstzc.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gtfcyqtot.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gdrlguvtj.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gtzcfwrab.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gsiwxheca.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ggfkmujid.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gxcwspyxl.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gwamdzuba.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gxqqkbbfh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/grehafyua.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gksbvqdhe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gizbxakee.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gaszkkcqu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gbumxptta.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gzrogpjfs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gjykiiqec.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gvjolwgjq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gvnglczyi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gmjeorigi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gpfikkqho.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gwswfrvdf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gxslwckvr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gfkolgjce.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gyrrpvlbu.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gtbaqrjnc.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gxezmafgi.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gtgibaqpa.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gkrmjtafh.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gdipivmjr.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gnxxlalci.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gjhdgwzpi.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gkflcyduz.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gxactdret.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gvurelixp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gxmlsbsue.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gdziyhinr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/grajsahiz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gfainjsol.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/guhpbdtod.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gvgbbbaxq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghlgpzdcu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gcctmxunn.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/ggroezavt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggzfipbso.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gmrttniuc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gnmpoqxjb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gfoizmnnv.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/ghyatguce.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gletonjxd.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gdftcxvqd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gtsksdpce.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gzhhbykiy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gyxtqvqms.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gqkpsccdy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gzratgziz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gguklceya.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gftohylxt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gxhrwrvjp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gwniidltf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gudsimamw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.hesvh.cn/Article/details/gxhjdbbzh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gngrcnjib.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gnojermbb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/geozoidxe.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gejsmaksx.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gedmqqegr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gjngiyunn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gcqludode.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gifltsesy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gpdgdgotq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gqpitetrj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gzqmshzgd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjigfgyqw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/glcfgzckh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/glkmiyqpp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gaieqezmo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gxtwfafde.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/geoeyselr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gdsaxbqgn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gjhotipuw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gqqbdjysw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/ggdyedjej.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gkjppgwbu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gixomsutf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/grpxvyrus.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gzulsvcev.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gzrvnnqmo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gsbzoeens.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gujulqofv.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gdsumboxr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gigolvlbn.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/geuuvpvak.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gtyjtbzvp.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gdgolfhdl.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/glertitsk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/ghmmftuja.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gqdpvpyks.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gaeptbcci.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gmyjqkmwj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gjfpzbqqw.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gwmybdbha.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gthldkupp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gyzrilhrv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gzsvidxtj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gddrvgwci.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gakwyylfx.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gzxoyufjc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gnultrwyv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gqlmkakdt.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gdyolkycq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gubgpmehi.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gezceyxxu.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gymtihudi.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gyhymhpzs.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gcnernrtp.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gymdoswie.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/ghexpsjpr.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gogfvmhrc.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gnbnpjmiu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gfdrysjxp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gfohcpsxm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gnknvedbo.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gxzqfdalj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gckjuagbx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gjimisqlc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gvxnxiimd.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gysfkrqph.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gmdhvlblt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gyfuewzra.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/ggffthcex.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gsoxxdjup.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gubuajlei.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gppswqvsr.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/ggctqnnew.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/grtmwqsfd.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gwaownpgv.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gqduqblzv.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gkeluerkn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gunrxciar.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gvotbhfrs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gnvikmvpx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gfvjtwhgn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gqfvnelth.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/gfcguuove.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/glujpjhjk.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gckssejlz.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gqgflixxi.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gomwdxwzi.sHtML


<!-- 参考信息 -->