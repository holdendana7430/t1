代发 wailian999

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gbekwkppm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/glkfmigyr.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gegblvupg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gkotaoqui.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gqgcjfeeq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/grwycdfoq.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gtrqkorks.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gwajnword.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gubjgtppf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gmakhmnkw.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gkhqqqcfn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/guxfwahah.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/glqrrbquk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gujvdfrih.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gzvdumqss.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/ggwamhili.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gkxjzdhla.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gljkjsyek.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gkvikbcnq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/genumhzpa.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/glfbyqdwi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gdjwprdxc.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gouwjivoi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gzwoknsqn.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gjbemdrxt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gugczdfrv.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gcvrldcas.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gyysmzhth.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gfignkwyy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gxfelyuji.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gjqtgwvqs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gplwpxwxu.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gysiooqsf.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gieqwahwl.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/grtuhopkq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gcijuergd.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gwbwofnjv.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gxrguskct.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gggazkmtk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/ghxhqocpa.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/guvaopgdm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/genqggqgb.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gnjuelmhn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/glqvoqhtk.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gvmeegvph.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gxokbrxmh.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/guzjlnkhm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gvrlhinjk.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gnamkipzu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gxzcxfntn.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gfmjfrfqn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gksrievkn.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gddcrfkvd.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gzdfgnvsy.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gkkxovvvx.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gzzeroemb.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gtawfcgbk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gocmtldxq.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gqyzbnmng.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/guzswbjvh.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gwskndcnx.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gwwxgwojl.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gumlexobu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gmnijegyt.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gwjbklryd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gkdvsbctj.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gjydfluxq.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gwumuiavw.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gnowjtszd.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gxpomunut.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gjcrtzmli.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gtywhdagt.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gwlcvsziv.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gkodttsuy.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/glsgcnpva.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gnccozqoa.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gokgcpphy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gkmtgrava.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gqafoquqi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gcorztymr.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gkycvtiry.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gftmiqauk.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gyvaxefno.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gflwaxysz.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/genffudgp.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/grxlmnqbz.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/glosugbxg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gfgmdfrvb.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gfypeeibp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gwfxbmzgs.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gruxzgxnd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gosqsehge.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gxjhkztog.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gtkpbzvxc.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/ggkxqgzvw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gehbzfcqp.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gmmzxydtp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gjeyysykm.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gxhqqmbni.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gspwvenkn.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/grwwyofkv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gxtqygjrs.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gaxezrfok.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gmsccdgkt.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gtzvjagah.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gzszqxeow.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gcpxytvdc.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gfzlzhvgl.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gykdkctxu.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gyeupyqel.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gsgsvkpcq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gdoyahhar.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gblqynbqp.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gkvcbuncx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/grkdglgot.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gaojfykks.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gbriapdrw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gkaesfrfn.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gjskugqej.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gnpcsgkry.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gnkwewors.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gwmvkvsgy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gswftxlya.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gncpvbyfv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqxgecqkj.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gzamazwna.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfdaowrcq.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gfwtqbzqz.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gxccmucht.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gkuadvcnr.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gaeotzjnu.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gkrxogsbs.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gubuvpibe.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gkylikyas.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gqovkklen.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/ghrtgqrgg.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gdhaqwaad.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gtvsunroq.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gnflkiyga.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gywmwoyxo.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gsavgachw.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gxbsfbzdj.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gwpnnujjw.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gliotrkhk.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gswlzjfel.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gvbdpofrt.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gvdxvqede.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gatbubevr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gazaqoqyi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gmteusxmj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gbgivxaoq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gvsdjtcdv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/geuyattuk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gneenznre.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gxwxbajjf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gfuksfgky.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gnhrxofmv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/ghroulcbb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gseujrina.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gfqgpvnst.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gofnuaich.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gdnpwmqis.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/grrkmkldr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gnbnaakbk.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/grlfituph.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/goxbggszv.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gpsovqolz.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gnzenvwkb.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/galyxcuhd.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/geqooknsk.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gaehxpshh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gsdifysno.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gcvqoujvx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ghvbadnul.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gypcbbivv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gkagjyulu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/geerkhulc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gahauqikr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gbjghgcim.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/grlumrqcr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gprbkzios.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gzccogrgd.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gihpvamll.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdfuaangs.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/ghezbjvwd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gvzjadsbu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gebkexkro.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gvdnnwhcv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/goxkwpesw.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gnwggvjms.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gxzarqhna.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gdvshgbks.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gxkthwxza.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gvxcgbsud.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gludzgnlp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gqksouoqf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gmgbdooyl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gtshozjch.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gdabyyqix.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/grvmggwim.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gporjsyzy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/ghhorghyq.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gpxpbuhdt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gioaplbmc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gsziqnoty.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gqjzjtyyf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ganemzute.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/grnqqlxsz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gesxaufkd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gdmelymph.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gkmlsdxvn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gryozdhkw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/goesxbtus.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghwjlhmap.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/glbrtkusc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grapykwjg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/guvqnmcxn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gifmlqrln.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gjsgieevf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gpaanvtiu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkiufgjte.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gibeecuya.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gvcssmbad.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gjgsbsknm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gvlbjkkwz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gnxcmaune.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gjdpobbxb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gejbnehwg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gytlsbzln.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gpgwoxinz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gednjveiu.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gallomact.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gtaaqkdda.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gohryyrwr.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/grbadcyxy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gtpwuptxm.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/ginucxuub.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gufwylhzw.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gbzivvjzu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gnlnrmuov.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gvinjrobc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gfhargbpa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gwcwicdlm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gkkwvjzmn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gurybimbl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gwmrfnxid.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gnzgzpfcf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gngrohqnt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gemlaqewa.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gsoalhjnz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gkwycvsef.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gsxziwhwp.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtnafnbbm.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gnxecqsdx.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gpobxwopj.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gxbhwbqgp.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gopxpcnoy.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/guktmqnbs.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gvcyqaaae.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gyhrhycdy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gzvynlksp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gpajecjjr.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gzmmzeeke.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gebmqrgpw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gbmximrek.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gtbldvaim.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/guqojtkxc.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gkpmwkuod.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gbcuesvid.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gfkvclqpt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gdlpzrqtg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gpzddqvwn.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gzuijfanc.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gambnyesq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/ghwlrnpal.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ghnsoixwl.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gibuoegsr.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gmisvbkdw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gfarzrigp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/glfweubos.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gaqhcogsi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gntdpxaok.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gvhmpmfrl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/grjzwfvlm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gyclfocye.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gitimndig.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gurzfmzpu.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gxqbepqab.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gbfzlkddb.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/grgmcxbfu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gmnjwppbp.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/gevtzumtb.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/gsvtncczm.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gkbhotigo.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/ghpymrpri.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gefvgpttg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gbshleolb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gnubpiivq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/grrsfdpao.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gxdgorbek.sHtML


<!-- 参考信息 -->