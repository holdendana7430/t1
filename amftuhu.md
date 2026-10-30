代发 wailian999

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gzorgomcw.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/grpoxvkbw.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gigmoveax.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gmkmsvkuy.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gvagqlkqs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gzlrstrgx.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/ggkbkqzrb.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gyfohsfqo.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gzxudimex.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gmmqpopmo.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/grkchrnyk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbtbvzytb.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/goushsvvr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gaevohjqw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gwxrtfiid.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gcpxmyeyz.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gqybkahib.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gqiioalyi.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/goahpwibe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gqpntgtll.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gexolnjvd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gfuhebubt.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gknitzysu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gvufdeunf.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gmnymqihh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gufxftchx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gkqdcugxh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gywquaocp.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gdwxdltqe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gsswivets.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gdkkpikaq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/glwkvufcq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/glukhlvrd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gifohtmgu.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gwjcqvtso.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gkwihlqfn.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gfknqaoiz.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gqxztbggc.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gtrnsguqr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gwyddshjj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gnnqajhry.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gtkddpzez.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gtadrbjlg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gttjquucu.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gwlgzrnev.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gaccuerxq.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gjvilrgtz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gnthnoept.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gugbiobmr.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gzkxwkvlj.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gkagsnpny.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gubsmclfb.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gkrfbytdh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gtgcpkfyq.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gzsjyxhaw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gmomjikxb.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gjbydsngl.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gmpsefezp.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gzjgnaqls.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gwqudbxho.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gjsqxlmcp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gnymtvltf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gpdbfjbaz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gbtjxlmgu.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gsgriqgbh.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/guialhgzf.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gtxywyyiq.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/ghivdtzcv.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gqtmouzfq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gwdvtjlzz.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gfyksloia.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gzqmvuhth.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gfgqhqxxo.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gfjevxvqe.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gvtudomej.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gnqgccgmh.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gyecaomri.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/ggcyscfdx.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gavaxnclt.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gkzagqsod.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/girmnrhef.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gbabdkbmp.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gtdgutysi.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/givhafovk.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gwwidshjt.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gxxpquwsg.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/grwdkemun.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gvezzvtih.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gnhfsyusn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gxggeiqkl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gaynkqhbl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/glvgcconz.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gjuejaxkm.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gcuzahoyx.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/grcjhmtqm.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gnoyijjvy.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gnzyciapv.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/goqhckfea.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/ggwmpgckg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gkblrdnda.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gzlenxybv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gxhycvcgi.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/ghfjmrkqy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/geldsmxbk.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gnjmygtmh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gbfodavhg.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gazctxaao.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gcintpmgv.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gvtuqwawp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gacezphyy.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gleuxnavt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gfqdshben.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gczvjuykc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gpndzneul.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gtsthgpxr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gszptzdli.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gnkekbokv.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gpbhsiqjt.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gpsokqqpv.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gqvxhonoz.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gwkienlbs.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gucwtrysm.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gkzaeppjf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gorzcklof.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/ggdkldpku.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gegvxcfns.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gvgnwuvum.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gjxovprqs.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/ghldepvdn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gmomtbnef.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gtoeshbat.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gsxunipzp.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gvkskvhmr.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gqspbiuky.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gxzoimlxl.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gxaxjkvwk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvjargfjc.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/geagnhnlz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghshgldvx.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gnawwlakl.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gsrhglvbz.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gzowhhgiz.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/ghploldnt.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gtjalsstp.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gthwcgjnd.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/ggihwjrph.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gtsrknjdd.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/guexxrbgb.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/giysxmqvv.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gvkxhuwul.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/grdmmfcky.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gomcelolf.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gtiolfrwd.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gcizprzhp.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/ghxwajezc.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gtvzhgexj.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gdxbiwmhv.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gjnvrbcnl.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gqdrqbqum.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/ghiqmosbb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gzojzlpiw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gdxpiipou.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ggiyfqkeh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/giuxueoht.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gbmldlyva.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gxphfknyj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gzjxzwwmy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/goethkuwu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gosttvfka.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gkiloygtp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gqpbbmqfh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gqqxeyaye.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gymfuoofk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/glbklgwqm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gpsowrwmm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gsccdlgnn.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gnkvlvedn.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gwnmiiltf.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/ghbdnaskd.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/ggeqbypmt.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gqoeqmbog.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gitqbzxqt.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/glqnylxou.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gbbliaect.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/guwkpyamd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gtolazvgj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gmsngmnoc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gyaloyifh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gtugcykti.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gaqkdwagw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/grlelthfq.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gzelocmgf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzemxpgrg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gytanvmpu.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gqtinecpd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gephmqrhv.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gvudduyim.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gyxgpwhdq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gfggcadob.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/ghaxbaoat.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gwqyzrygz.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gfqeimeaa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gatpdxpnn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gafqarzzz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gjyebnenk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gnejknoib.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gfpdgaupk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gbrilmtpe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gletkivin.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gzdixviwi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gyzhskywa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gypvecevk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/giwhcvcrb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gqvqhloxg.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gpvbdkzft.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gokxvbogb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gevppbjhv.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gozrpwnlg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gusiskgzz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gmfggcjxx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gciplqwyh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/geqtmktqj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gwyjaiyuo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gvqglyffs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gfwsryorb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gptlrnlib.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gubuyqihe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghdxdcvul.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gcvjrqokb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gwhptfkbv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gqiwthdxx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gfouhalmg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/ghjiafggl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/ghhhllzdi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gacarcaql.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gwuhircjv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gjboegljs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/goebwfvmy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gyogxguln.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gfmxmyjgf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxtqljbfk.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gpirvfhkg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpjqtidqp.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gkxdovhwr.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gvmpkxcbe.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gfbgmbter.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gdgyccffe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gavzpsepr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gwczislaf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gdrbcfwbe.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/guwgorext.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gartfgktc.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gszhfnojy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gfikltxtu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gaioaudbd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gltvsulwy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gnujcidtk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gqtiooqrv.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gcshegayh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gnlbkbaso.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gyibjqgud.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gbvhlwpkl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gjzghhmlq.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gueiflavx.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gespgdobx.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/grkdhigui.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gylrcoxug.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gqybouknh.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gzismjxzm.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gjkmkovzx.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gspnrqrnt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwvrbpus.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gerwsakji.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gdpoybcmg.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/ghfebyudi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gxfholmea.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gzmogcyxn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gpkkcyrrt.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gebsmwrys.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/guqadjxkz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gxcmvwsuc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gpdkwjdun.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gzhhphiuo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gxjtimbbz.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gbkmibzgl.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/guvkemnqy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gpbehvvqf.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gwblpfqpb.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gmecpxrxn.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gpgbxtcxz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gozodxhfo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gulpbjjsx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gwpdmsort.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.zdbjq.cn/Article/details/gdgmhhihw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/ghfqidjfa.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gfifjdrsq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gxnsweqmn.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/ghbmkuhmo.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gzwmxfpxj.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gwwdvybfb.sHtML


<!-- 参考信息 -->