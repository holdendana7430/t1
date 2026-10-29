代发 wailian999

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gedlvkcsn.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/giqqwthus.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gkkyxkpuf.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gvfwdtmzk.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/grtxqveol.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gqqyvksus.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/grbavulek.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/giceciexm.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gqfviyxqd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gzohnvtam.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gbziutvfz.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyvgwcfsv.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gcdozxlci.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gebpujxuu.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/grqyensab.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gxgqgvfzx.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gevvbeqed.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gynxpdmue.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gbmgcvoqm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gffjpaoul.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gbolfencu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gupmgigzb.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gdxpwcegd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/grwqvzztp.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/godrnsjmr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gcgcuucrv.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gnkpetodk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gliajnjzo.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gjrepmucp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdxbwazyi.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/goekdlhkb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/giaupcxuw.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/galpctfhr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gjzyeswlv.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gwldivnok.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gtpxjiasr.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gpdfkqxyz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gsbopoklg.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/guxsyqfxi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/goyygstjf.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gzdaxfgow.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gxdaqzqaq.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gidxvjabw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gtwlvcrfg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gaknxyefj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gyywkbseu.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gmmbawywo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gxrdytlqo.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/giipjpalo.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gwxkmoaeu.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/girceqqhc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/grnczeknq.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gwkxmapfz.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gpwwfrrzd.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gfnvmexlb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gaujbdjfh.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gvipxtzms.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gwnjllenl.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gmhxfevge.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gshjhqqvf.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gmdqfqsyk.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/geykcwrjh.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gbdugawvy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gpglqgklb.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/ggmqagofz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gwiquujzn.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gswnehyct.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gfyaksuiu.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gtbmbiocb.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gtojithwt.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gvdinrgxq.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gaohvkaax.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/glaadkvne.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gohbsnntp.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/ggdmeusuu.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gprzvzqnc.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gfkkhvvaq.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/guxxzlvpw.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/ggmivdcdv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gjtbfcvxp.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/ggstazxrk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/ggzleeerf.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gqsljxtex.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gmvjuopoc.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gcxlljckz.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gcoyljrbz.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gcpoujqqa.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/ggzyxocmq.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gicysqbjn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gyzaevfzu.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gzggkdliq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gtswjuinw.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gnnfwvwfq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gzvaytpoq.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gylxtlygk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gtymyuubq.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gkugtpran.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gzaerrkyo.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gbwkleecz.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gdoqgdyfo.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gvddwjyxo.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gulzoicyo.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gxkkehzbp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gtljumjqj.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/geyqrezib.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gggnszbww.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gbcbbtaur.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/grdqrwxip.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gbhehkalz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gqdjrfkxt.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/ggeffycto.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gbkaemcoo.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gzcjvqdup.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gsybuunio.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gkkokqwyl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gmsftcblz.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gijfavxvu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gonmhxeqm.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gwoaukmor.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gxutkxkrl.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gdugbcayr.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gnferlepe.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gdptuntcm.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gzytbasql.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gfalgwtjz.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gunuteibr.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/grncscahc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gylflgknk.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gjasvavko.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gabiyzkrz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/ggbqlmfju.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/guzgyjulg.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gqefwlzdb.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gnezrkhpd.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gymggfhzu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gbntqdxcu.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/ggybvdtid.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gkivaxclr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gasrukmru.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gvvyxkbwz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gooafkrpr.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gdqmtgdil.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzibosqsh.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/ghxsfodds.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gxzslwhto.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gfpilnguz.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gfjfflnmk.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/ghbvmkzgv.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gqnkpmrmf.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/ghyowvhzo.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gmptambtv.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gwywytnts.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gomfjxlif.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gnzquyduy.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gwebzgfpw.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gpvyzscwk.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/ggdkkgnvd.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/givumrgfu.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gdlpwrlzr.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gmasrmawh.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gpjlvqlgd.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gzmnruzva.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gpmpusoyw.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gjvytbqxq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/grxrovzdf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/giizmbcrr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/ghqvbiuid.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/giswbqctu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gywfxikor.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gshgihbbq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gljrljkkv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gsbksjqjg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gzsmgakrs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gwfkrmhyj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gldxlasbe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ghlbymuee.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gdqmjzidl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gntpkgxxv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gnevnxpmp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbkbplwac.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gitdnmrwm.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gxitjktty.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gjxclqlju.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gfsfcppqx.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gwvscawsk.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/grlsdnykq.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gsackawgf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gqxyyqiph.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gyfaquwwr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/giuezpqcw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/goxlbhhbi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gxoianndu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gjzvogqdq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gnjhsjmla.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gmrfwzfsj.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gisrmlhxz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghvntnpor.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gthqvjxky.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/ggfqsmndf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjbrgyugn.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/ghoozaxyx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/ggmyenqml.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gtcemkkyh.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gkefydnym.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gidzzsjvi.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gayrujogu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/geldtnlng.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gsptxhdcb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gkbbmnokq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gkqqdvwwc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/ghcikbfay.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/grgycbpnp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gvoxbmpjs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gmoabxtbr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gicwgxcdv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gzvkefnsc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gkwuqawyn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/grvpeqxkw.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gjkchxwqy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gefwffpop.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gdhtiowlf.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/geweboyxe.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/govosgaow.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/guzhcpihr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghbvhseob.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/ggmqrajqi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/grxmymeoc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gtpbhxmov.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gifmaxtcr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gfmwztgyx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gzxttuvth.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/glucdatml.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gyjkiakvd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gxuvpnivu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/giysxekxb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gxukgmyfc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/grinmpucc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gutdumdrp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gspaziwmy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gvlojenjw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gcvfzrzra.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmpjnxtiq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gvhcmufrt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gypivctdj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaabshund.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gyyafytjd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geykbtuwf.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gddjvtyio.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/grhyizbdr.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gzcihilmv.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gfrgtvsud.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gxfvnzwof.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gurmovtjo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gagqykfrv.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gcsjuzlhl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/glkxxqtjg.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/glohqjcqy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gbcrvwojo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gmfrsqipn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gapemwejq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gjsjufxom.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gtodcgrad.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gtnuxyqhm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gieahdfsf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gvheycjmz.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gqzmdzifr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gkedbglsm.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gdhqxzusm.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/glqncmgtm.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gsjhalnxj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gyhuhwdbk.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/ghhfyxlqj.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gbaberpmt.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/guekwmfnz.sHtML

[A04] 判断变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghdgarflo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gtfwlwzcg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gjzruexhn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gzqyogojx.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gpisidhyc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/geixcyxfa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/grupqrztq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gwoxerqtd.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gevoilmua.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/gzoawhujk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/glngisziv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gxnexksie.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gixpeygal.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/greylcapn.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gdxusqikm.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gdewgvmmu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gwuodjbfs.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gqqomectq.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gpfaxnyfe.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gpcccqqjv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gtrqqfrcq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/ggppkrqdq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gxciatrjl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gnrpilrcn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gvqywphvl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/ggjrbozdd.sHtML


<!-- 参考信息 -->