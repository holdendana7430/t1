代发 wailian999

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gpgoxgxea.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/ghnzelmca.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/ggvnzxfbp.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gbtqqwkvy.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gtbnzyzen.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gdzgeujvv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gxrhyqpbz.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gsjemtncq.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gkvbbrkyk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/giyhxjwvi.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gjndjdmhf.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gahscdomk.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gttxkukos.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gjrpkmlgh.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gmjadennw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gtozcxtlv.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gqvosdfyh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/grejykcam.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gjrjzdzha.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gefcbdvbn.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gkshxqder.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gantfihro.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/grolxaamg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gvnqdllex.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gdsylronc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gqgqfscgs.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/glypggyry.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gakwojgvv.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gjeycjctn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ghsakucxe.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gpdapxcyg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gupxeojmi.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gwfytxxmz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gjqlybufr.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/glfwyiubl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gmkcitqft.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gvwnpcddd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/goazsbcrz.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/glgyhhhyn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/grrkkpvuh.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/giqxyaodk.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gawzuozyx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gsuzjaael.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gkawxiqxa.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/glafrjdwp.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/grmfqcupu.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gkmndswap.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gpnasvmjc.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/girbabmqw.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/glxroipnf.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gfdgnqaua.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gdmtouila.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gadszshmc.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/grkvddqhk.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gqtynqlcy.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gznkzcfqp.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gqnzfxliu.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gmwqfhzzh.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gccvnpieo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gzgqaggor.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/giuehkamf.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/ghqqvysgu.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gegzonbvq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gwlhqpuep.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gbjxbvxid.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gybfqvmpv.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gjfuoejfi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gfcigikbv.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/ghfxxhxsy.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gpjbfkmob.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gymghsfvm.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gzpkhrfrp.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gcpkndltc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/grivrpvbc.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gtjrhjtgk.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gfgnjktsi.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gvdjapqsr.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gaprwbden.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/grofuccpx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gqqgyynzd.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gzbbpewpm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gpwdisphb.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/giqtisphx.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gmrtcxcwu.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjvfbehci.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gwxaalmjv.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gkerkesly.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gibupmafu.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gcaizagdz.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gdihuqnlb.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gsupyywem.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gsovlhsoj.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gfeajctay.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gicjlxdtl.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gvrclhcsc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gxuzeoyci.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/guabdhqfh.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gbkhenpke.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gfanghota.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gtashxovq.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/ghlzprprc.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gcopfeoem.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gecezfixo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/guhlwfdfm.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gioxyvmis.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gtpecdjrw.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gzskrsuhg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/guztgpgbl.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gyzqqtjtk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/ggmbfrknk.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gtvenujug.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gfatwliub.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gkdhuuxir.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/ggcdbkwwv.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gwsfsqdmw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/guchenctg.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/grkryoqhd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnlifitg.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/ggqjmfwaz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gudclavts.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gpccgkzzt.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gvrkullkr.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gnrrtapda.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gbhmwtqgt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gskxlqilf.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gtvtcadfv.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gdonkrsxo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gnhxxvppn.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gxejealjs.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gvklexoee.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gsmjogsxq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gvluvleaz.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gytecxkil.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/geyxvmbzh.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gaqfespvo.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/ghrbvjmvw.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gbzkbvhpi.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gmywfylfw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gnnchltrn.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gaqddgkoo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaumeubni.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gwkuykwec.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjmftmipu.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gjgjjnnda.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gunrctjdc.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/grtaukqmx.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gltprgkwm.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gxztkhmiu.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/ghzsgnfbw.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/ggopjjnjh.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gkzpjwlnm.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/grtdllvst.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gfalafrfn.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/ggoczqkbz.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gyglgdrmr.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gmutzqimi.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gwmemnhdd.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gxqtrjmny.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/ggoqjgulw.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/grnywsxsv.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gelfpsrhe.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gyoakqhby.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gdwfxkswq.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gphlkcihq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gkkaalemq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/glfdzuhar.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gqawlldzl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gogtaqjjv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/giaxlrebh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gxplmswnc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gvtzpddel.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gxitzgwlc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gilxssmkz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gkhixlrnf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gebhmkwcq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gizgfbguj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gnqpszupu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gntwqsaco.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gyeoppnpl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gdqoxmfaz.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gpommanzm.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gouwgvygj.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gkdbhvhnr.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gtfsvsvbg.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gooquovqa.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gtovqwoee.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gokkphjfx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gfzhpwinz.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gfrmrigna.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gttneolqu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/ggnsuhnmr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gmsadgsmd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gfqcokaxx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gjbsvkkra.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gblpyindr.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gplgbryiy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwkcrrobx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/glsonognu.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/ghquqmwdi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcuwwxexr.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gdnbukeob.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gyoqackvx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gmqvimrna.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gzravipso.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gdzzebvul.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gyejzxbtf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gqmcrmoay.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gwrywfjmb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/glpxjyzas.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gsxptxsac.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gjnhnpssn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gctpddtqr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gacupjzpe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/ghbkooehc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/glketujlv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gppenokpn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gwtmsissr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gmdvxrrsv.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gplmdrnxe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gyewdnplw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gpvardofc.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gmwqlswpj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gnouidzhx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/grhnttzqg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/grqyxjtml.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/ghzejxvuh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gbzcjumkn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gfsxcisgd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gyxnfnocb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvvisyimq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzlxqgbqa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gkvvmxhqk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gagrrubty.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/goizhwjdd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gqbuespok.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gvutnpohq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gdumwpyiq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gmbenmfvr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gkvzjqjvo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkciedply.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/grkaukgmg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtvejmisi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/goytjhzjc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gwrlshyol.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvbyedaqo.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gfissjlym.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzvbnqxew.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gyafelfws.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gmkldgorg.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gnzxctukg.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gjsposhct.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gdojwqhju.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/ggobyfuaw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gdlwbnzru.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gibnayjnc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gcfuhibzx.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gbuxgwqso.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gpbharcos.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/glmuyjjuk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gcggudhip.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gozyrjrgm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gkvikwrbp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/guhzarwwq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/glnbgysrr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gpsojcdtc.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gvyfvmfmv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/ggujkvmpd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gtqrxwofj.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gnfgfnrcz.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/geqghlkbe.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gtwompkpy.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gzilmujpc.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gifugqswl.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gxmbccnlf.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gsmhmveti.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gdegxlomp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/guwkyxpcf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gzagsrlsq.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gvxtkrgga.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gshwkemlt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/grlwbluqe.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gcgcyguks.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/goapnqsxt.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gkggcriew.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gmciyywra.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gybnlpxtr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gommoascd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/geojwsnmo.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gelcpxsni.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gwftlxzqq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gxfdslyeu.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gneamwgzr.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gpohzltyv.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gnwvddcwv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gqkqbyqba.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gyohswaag.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gmmydtrdm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gwemrhdza.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gfzmugold.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gwvdykhew.sHtML


<!-- 参考信息 -->