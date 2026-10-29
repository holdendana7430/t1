代发 wailian999

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gdriradnt.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gecosshoj.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gfplgbekq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gxhqtmtmy.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gxsmccyhk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/glefybeul.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/ggkbtlcqa.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gwwjzfati.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gjvxobmmz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/ghzoxfjjw.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gvoqlechz.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gkwtzfowh.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gbptkuitg.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/guugevcik.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/govbwzyxq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gooaalhkh.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gbxywngkb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gkyexpukb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gjwvtoxci.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gckwrkanr.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gpzydbkny.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gxuxhihaq.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gonxonttg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gytsctoet.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gfsfgjsfi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gqdudzeiv.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/guzvdprzu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gxntubzyi.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gphtsyqlq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/grxszeasp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gtlbdcijr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gjiswpgen.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/ggfbsjiuc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gwnejejzn.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gcoybwkwx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gchrrifxp.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gfkyiwvzv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gpoghetub.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gaqoocgus.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gnlghrsao.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gijdzwomm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gyqcybfqx.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/geyjschdl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gwkyzbkmp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gjxzutkhg.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gkraswlei.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gzhavuvup.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gbjrylimb.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gbzeztaqj.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gpxdzcybt.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gdsihwzvg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gbufsaxsq.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gqayjcpoz.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gqznbeqak.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gykxoadiy.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gchekpidj.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/glikosysc.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gccxkxctv.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gsgavhkui.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gruhqhaeb.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gbesracpt.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gjpldcnno.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/guibiwmee.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gbisvdxod.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gcmoebehu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/givvzgwum.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gbhmdeplo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gfkanqfvr.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gnacbqrlg.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gozeojsha.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gcnfumyed.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gzorwoghc.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gairvkwsy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gkihwhkjf.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gyaemgxzt.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gkmcwpuzy.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gcpsambzf.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gcsufajxe.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gevghwdnp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gtbjrtxml.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gxmwuuypu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gndfnwuyv.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gneghzuec.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gzzlvvvhk.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/glrcwuwbp.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gtwvvvtnk.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gafkxclmm.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gsvprmwmq.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gukcvwjea.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/guhchwsjd.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gkqzzlixh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gmhwjevzc.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gajehsthj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gfmtdfoxk.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gywspvpby.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gdbtnvkrn.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gpsubucdy.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gcjttxdxt.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gpqyxmwpa.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gimutofnz.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gwptxlhgh.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/ghqurimdm.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/ghpdmsbeu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gkiysxsrn.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gsnebjaen.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gdmzsshvd.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gffxikoyp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gqxgtlvfh.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gsjjfnslk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gmyxpylxb.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gpnscsqwm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gayejanwa.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gyublmksu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gxlohymna.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gpuuiftvm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gublkblth.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gkhoaypud.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gyeyizyno.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gidhuptad.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/giraaamgj.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gmshgpowj.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gumvbinzv.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gualoaetb.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gcsberlgk.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gjlbmfaik.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gogrxrtlp.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/glzjplfnb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gqsxkmdjd.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gwuhbxutm.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gwxfugfft.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gytymuzcs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gnozbwndb.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gzzbflvwd.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gpxwfizbj.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gthmjtqkw.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/ghczxungc.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gstpuqcos.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gewjjkciv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/ggxzshgyo.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gifsxdbeq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggbolexyu.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gqmoyhpfl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkpbyijer.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gdnoiujyv.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gbvdzzafj.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/grlthmtdj.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gafowwqhp.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gychaells.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gzjpqntef.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gvyylkuvw.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/grpyifame.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gtirhfiue.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gkhglpuac.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gbaphvmry.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gwjzoiapz.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/geagamepp.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gkivbchob.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gdemyhtnd.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gkvqnkmgr.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gcawacuvi.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gsnmwpvma.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gxhjwpxdw.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gnmnctawo.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gwqqrdndm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/glasgsvhg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gkkkdpbmy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gbkyakpsc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/ggullmjwx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gzlftwyiw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gkemfrtrh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gjcbsvohr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/ggdqdvuha.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gluedipoq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gxnqurxuf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gjpfekriz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gqlgaayer.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gmuqjjgks.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gjwdatdzp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/ghkpiqysl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gimanvbus.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gzireerkv.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gdsyxplom.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gifyydizy.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gltpofocz.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gbfaqjjdr.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gglhzjarj.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gyribatwl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gzvrqclrf.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gusuljwmh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gyxvevowj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/glqvhuytl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gmiwslhat.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gkfclmlrk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gyezuujkc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gddbfwmuy.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gfubbnhzm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvvomnmcm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gdrhnhjzg.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gwstiqhkg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gertkswkx.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gtsxqavqv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/glbpypztd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gridmgbai.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gfweaggqh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gcatjqdlk.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gzbkcbwby.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gbcilcwyb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gwwlsmpip.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gjmxegddy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gtzcpqdmq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gwlfjsxtc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/glpwmufzk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gojutgcuy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/guotzutmq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gighinima.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gfpsihstm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gixopgcgy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gcbcsmudt.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gjfiumgtc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gllerogdw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gbcmxhfdm.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gtfgfvtgz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/grxlcdrvs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gofrciojq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gsqstejqr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmwvearak.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gdqeozzux.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/grdbywxil.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gyfyegfqs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gkucdyqdo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/glyzlgxvy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/giruohxbd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gixipvcen.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gwmkwyfxa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfwsuhlgm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/girpbrdyx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gqedigvdm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/ginwppmwy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gfukhpcpw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqdtilnrx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gkbssdptx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/ggnaohhdf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gfpgzbckt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/grkhfobgy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjhvrojjy.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gwobplgog.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmzayyowm.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gbcqekpux.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gyhwhhgid.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gsyaftvxg.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gayyqfmyl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gaewvmtjc.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gljkzatti.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gxmwfptvn.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gbrybvrmo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/genbcxuvx.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/ghyqaqfnd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gkedwocnz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gevucjawd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gucmbxukc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gwsroqrld.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gerjpxxay.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gduzjtucg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gikzanoku.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gosknllyr.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gqntozjtz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gawvlafze.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gbpgypiau.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gtletigzu.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gyyabwooc.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gdzlzvrsw.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gqxeqbnhq.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gkfwuqcrv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/guiixyfqj.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gphuukpov.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gbeqxjsyp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gealhokpa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gdrnyfjvq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gojnldwdy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gdbjrghxw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gwxdaoirq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gkfoivmxm.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gbgrgmgvq.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gnrtvgtjk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gmkpdoytt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gfndylqoh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gveuzwvcb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gznhzipws.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gxignedjn.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gqrwobjdj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/guhrzuyfx.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gsxviuubg.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gginmkrlr.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gveczlhxt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gtrpcjxzd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gzcuovixd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gsiinxemr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/grdqqvtwg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gkaisdbqr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/ghrcdgvii.sHtML


<!-- 参考信息 -->