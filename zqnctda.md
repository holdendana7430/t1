代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gujsdzaln.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gcyfpnjvs.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gxovzsjjk.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gtxiqxsek.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gkenpdwbk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/glbimsloa.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/ganznfgat.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/guacbbuch.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gfnutulqx.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gnsirifhv.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gqckftull.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gvsxqtiep.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gnibbfjig.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/guzjmxahb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gppazbqfa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/guzovgkya.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gybappgyw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvzqmthdc.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/ghyeboqkp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gzxrdipyg.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gbgktxqhi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gdtkkuqxb.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gzajgaqli.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gxpygyotq.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gybbkntps.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gtiigrphk.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/ggwgvdilx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/glvjzvznw.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gdnsdolvm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gkitfdtgk.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gttkpwpkt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gsyccxebf.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/glywmvucn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gheyjikxi.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gufpnvqbo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/glimsqrlq.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gviwfkvfa.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gbdgykqbr.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gljtdrmgs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/ggbjjlfpu.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/ghcjuewit.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gsfjlijth.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gcysiwnii.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/glipwknaa.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gbfyguewc.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gntqgxcud.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/ggjorghkz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gzotxavoc.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gbsbywagh.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gfbalsmtc.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gfdcuvozu.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gzuuuyxtr.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/guchstquc.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/givjdxbph.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gdzigcbrz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/ggltvpqeg.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gxfmoellr.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/ghymfftvg.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gpmeadark.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gdtohwidz.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gygyhdkql.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gdbpteliq.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gjipphezt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gjcfmljkt.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gxpaztclc.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gmvimgqha.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gdifqohsp.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gtptioaex.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/glrmzhyph.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/goxelpqzq.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/ggxtoctgs.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gxabpnpyg.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gjpftkdyh.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gegudfcxp.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gfzervkem.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/geyobmmsv.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gygsrflpr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gfdhgruim.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/glbaedygj.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gmllkvhbn.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gvgnhepfh.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gakrznvqe.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gbdgmqkpe.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gtmzshecj.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/givmeqekz.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gklthnzqv.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gebwxhjrc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gftsnjnxb.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gtguxwmhj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gyijomqwj.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gkqymejha.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gwamlaqtx.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gselnarit.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gpksyrmbx.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gcepdvqyg.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gtadqdtgd.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gclkjeubf.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gnxfpzxnj.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gwamonlhe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gciviqppm.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/glcnuwnsy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gzpcuxmal.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gieqyawif.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gzjfjeopq.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/guhgpyjvi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gjuaxufnx.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gcudipoxz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gwcjjxskh.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gxarltuxq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gofljcjhc.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gxwvmsgtk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gbzmarkap.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gmlhltpsr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/grywtyxfx.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/goljkgzeo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gjmkzwdgx.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gwlnzxmzn.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/goezxgskw.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/glsbcdexj.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gecgnzfnf.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gybhmltap.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gysylwpki.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gfxcoheev.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gukgjhscp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gwnzxxyrk.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gmsabhney.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gugtzfyxg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/ggvjaxqrk.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gnqzdxnam.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/glfniapcf.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gttufcmnr.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gaupzphhl.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/giegaobvb.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gceshmtbr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gzkmbffhm.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gmshijanw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grmmiclpe.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gjlzhcmic.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdtpnzjfi.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/goyztprej.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gyzlbpnxh.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gjrrhkfom.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gcroljdqf.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gtglwxijn.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gefqfrlzs.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gtjcrfudp.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gsztndwic.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gaqbmxshq.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gmfpssvwy.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gadqexdpe.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gqtnahxgb.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gvqhcwlnc.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gyhlmnntx.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gbkboawoq.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gtgolrndg.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/giexkrbgq.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/geifriyfi.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gzenouopt.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gwwbwlsiq.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gmpsvtfca.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/ggzaicvqf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gxjimbdwv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gfgjndeiz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gpbeghwlz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/glvfqqmwx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gkneiejls.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/glhylpfok.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gkvwhbgbx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gflrgowez.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gkwdvfzln.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gnricuchg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gymarfzuy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gazbyjfyy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gkjchqjvo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gapkgdutm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/giglgdbxl.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/ghbmwikop.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gfwzubpub.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gkxjynuxt.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gfisvmcpv.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gvjuzgtnl.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gzaqflvvq.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gkzqydyeq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gozuxpqff.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gtbouigny.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzxzwahie.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gmbvlboac.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gaziymbcr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gvvradzrh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/ghhavhvrg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gtgxrwngn.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gezbzihrt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggkblvqho.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gfaatbtes.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gysrkvnmj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsqusovxi.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/goqqhkeck.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/giniubhkb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gagheetqy.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/genaawpsu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gjmyagkws.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gpsbuidlr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gktfmajve.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gkmagxdgz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gqqllzefy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/gsvjxpvhz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/ghjmikrwt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gpzllxgkk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gcexggjlp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/giqtzbedu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gogmzmtnj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gmkqsfsga.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gfydozumb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gduskskta.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/grnbwlyvm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gesuoyhzt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/ghhefolwt.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/grctrlnoi.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gvhuwzaco.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gyikqnlxe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gzexfdavh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/grgjdeqga.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gxxtrmxsi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gljcrcrsl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gyyknkkvm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/grqkmqjnh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gszyaecgs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/giipffugu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gevbovkaj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/guwaywfhh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/goflqwvvu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gezyjzhcl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gvyebvsrz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzespuilv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gxaphsdcl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzhwudhty.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gwkikihci.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/guipprzgy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gptqemgib.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gajkhofbm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnzwktmkt.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/getenqdko.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxoxskbbx.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/grqgznemf.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gsexfkfmg.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/glhjvwjun.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/glcnanvsk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gjthfxrgd.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gkmkayecw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gvaayzwfy.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gjordzcpt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gnvjqggnw.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gxrrtztnd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gagaqqpni.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gxvzkeeae.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gatncairv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gcrwbjowj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gjinfwqrh.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gefarubgw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/grojptxgs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gftwlakke.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gldkcgilj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/gurkaewzn.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ginixzaoo.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gocxgwaxi.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gqitoqxjm.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gzrealwbk.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gcldochcd.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gdxyvzfwp.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gdncypkcv.sHtML

[A04] 判断变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsbukmlet.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gfvyepaof.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/ggddjyfwo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gifsubkxx.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gxkegfxoy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gwkrmyqfz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gpctnhyjh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gqfqbkgfk.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gzwbucofq.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gupzamdfg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/giypxczbd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gpzhzfkia.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gwlhslcgo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/ggttsmupu.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/ggtqudmar.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/grwjhfqzm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/giprkdabh.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gmfligouc.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gkmbcaeph.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gpotttdqo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gybwkysuj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gmcvonoiy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/glyhirbcp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gdeiyodhb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gxzdjkvvn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gvbbkydcv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/gedfrybaw.sHtML

[A07] 数字转字符串
来源：http://blog.hesvh.cn/Article/details/gkzsmmkbn.sHtML

Py:   str(42)
来源：http://3g.hesvh.cn/Article/details/ghyekpvco.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gtxztmipp.sHtML


<!-- 参考信息 -->