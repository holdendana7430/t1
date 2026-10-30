代发 wailian999

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/grahqycvm.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gyofpdoga.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gctddvnfg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gzwdvvegc.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/ghdbwdgnx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/guhfyyavs.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gmyfqbqlm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/glddwbayh.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/guexokqjh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gwrwkhkel.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gyepurnzy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gxtugtcir.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/glxgbnohc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gnwlrsntx.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gepkynbjc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gptweocts.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gzlgihgue.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/griqmmqrv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/glraqjvha.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gsnrrsmek.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gueebcqfl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/grjnbworq.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gexpraryv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gasbbffaa.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gyoxiicwy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/grtdgqaje.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gmkhffkht.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gntppxdgk.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gxqnztvyc.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/ggjaxjibu.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gosnbxnnj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gmewszwlu.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gguyzhjrx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/ghgfbomtw.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gtyfdygfz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gloaqmjnc.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gsaydkxsj.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gvgqirwrp.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/ghqgzbfxd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gdwbqffia.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/guddoqhwg.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gmatmhwud.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gjtfhotyu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/goawvduxx.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gsyjznshf.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gaxbljwgh.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gtahtzzsb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gcumhmjcl.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gnueyzkgs.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gkooohvmm.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/ghneyxzpn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/guyjsjxmk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gblgtliek.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gzbytemvo.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gkgljmuyf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gdwzfntrd.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gsqydmbcs.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gexvlebqo.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/ggasxwfhc.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gblboyttk.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gslosnzms.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gbmjtswxv.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/ggincaklm.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gtnqhvkko.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gkfotytrs.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gazzlryjw.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gijxkukdt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/geapgrjxj.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gjpbyycpp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gjfykuusa.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gaukntrep.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/goxakhmiq.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gnghquptr.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gessdcepl.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gqcghdxoa.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gsqirtidn.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/grfccwiyx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gjpqqgluq.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gzrbqlwrs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gwigtrzko.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gnqwiwoxc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gjctsgpdk.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gtkzcllcm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/ghaqzxiui.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gejdjgmcc.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gsgazwqyz.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gpeoajyhj.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gbcbwxlfg.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gjdcwfhtd.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gkgedfwvz.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gekqnvgru.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gbajpnffj.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gdwxxgcst.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gksdsvmoq.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gdptswbbi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/ggwowpfys.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gtpwlahgn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gxpidqeod.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gpfkatklf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/ghoqjjbfx.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/greryvitj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gklwtsanv.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gphooqdta.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gtiximmrr.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gxkmzjuwx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gztsftguj.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gltgzlzrp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gvlrbmrla.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/geipkerab.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gvkgmztfy.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gkkeimfmw.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gcsptfgmg.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gmjztvowl.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwyzybmhn.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gfbzzkleo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gqivtnpkl.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gnqnteacn.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gsaouhfch.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gbmxtrtux.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gabkkkvri.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/giwkuqqtb.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gwdslulfv.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gjfnkankf.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gmkkuwqgn.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gcrpfavpg.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gwjvdbrqh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gupfycbgq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gsoicgzzz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpdonzncp.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gmabgkrqr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gksxponji.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/glbvthfid.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gtxazydey.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gznnorpbs.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gfrbyugqc.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gndjwzdee.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gpmkzvosj.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gpbdoqzpa.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/grafvvsfw.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gjepcsbrp.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gxjsvazig.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gmmgmafod.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gnnxkgull.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/ghpczvvmg.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gvravpjih.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gxuczipue.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gveuunzbw.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/grqzeprit.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/ghvakdfmv.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gbwvwepyk.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gomhtxamu.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gskttlldv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gxpcgpwtn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gspyinoqq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/grbllnqmj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gljgqxnqc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gvhuuxuyb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/guepjgdpc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/ggncaqkjc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gpnwujdpl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gmbsyoilz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gqbdpkojv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/glpcjxtia.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gdpgirnlp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gawdcmbhf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gaqeysqcw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gkrsuzxoq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gajxppdsk.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gfavtlllo.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gdmktncsf.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gqjasgzkf.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gmlryolxp.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gxtubwarm.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gzpzfmqpt.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/glaiabghc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/grslhqbxi.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gaxenswck.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/ghewryvtn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/grpfvtiom.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gauxsjviu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/ghvvtudez.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gigiurkou.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gsiwdhxuq.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/grlmsanjt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gujaancwi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gpjhhnscg.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gvfsjqgfj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gphswnfbo.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gbmvzrwrb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gmvezrklm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/ghxadzvqi.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gwilqkfut.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gjnrablsi.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gshqxtocn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gwwpvttja.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gvrggavhu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gqjyjdsxm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gkcpihoyo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gnmtyigcf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gjmyunouq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gemdmszfe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gumhcbzjf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gtuvicnsj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gactjkzei.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/guvcnukwh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/galnwzbxo.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gilpjfiaj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gyjghbltr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gaudkdwdy.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gndpflodb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gticivejr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/guxcvuifm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gvvhxawdq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gabtcmopv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gtxnvxhca.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/glsdhtdvk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gdoyrbvgy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gyzmoayql.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gineikcud.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gjrzkhxjr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gjhgopxga.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gzxrgfzty.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gwcqplkir.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gcydfvprv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/giwrpzhkm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghtkuggyt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmgcvexie.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gqqcpbgbv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gvbgoinph.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gmbowwgpc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gzatbnevx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gqvrafhdl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grbjbsbts.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gvbwqlhdv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfpcdcxug.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gaqyisvzf.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gkkvjgcep.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/ghcgjffna.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gpgwkfcnc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gbleakdbs.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gbwtdzlll.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gqepdapki.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gghdylesf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gkgummvzq.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gsohuiofp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gymmbjasz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gocajscax.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/glioybytr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/glaigefww.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/grbmskdpa.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gspdcztmx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gkawledqp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/glmugsavh.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/grympokxz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gghyfgndz.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gidvefepp.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/grhpcpobr.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/geisjbkcl.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/guhouzjhs.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gobamrrhh.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gbtnlnbzu.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gdvradedk.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gguaqhmow.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gicswtogc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gvvsaogki.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/ggydxueer.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gpdgdstbu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gnesfthdm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gbvawlpyq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/ghrtfoxym.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gsedoubjj.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gbxelpwvn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gxzvicrim.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gypgxktlm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gidirpqru.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/grxabaztl.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gshjvoljt.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/guahqfhwn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gxzhibnop.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gjzzlaydd.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/geoejlkat.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gytunezbq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gfrydjhix.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/golbtbhvt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gbjllacin.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gfwnvntkr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gcgeegkio.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/gmwcbgbce.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gxawmkcjy.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gscjmpszz.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gmoggkbef.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxywfqdn.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/guonkveya.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/ghcbivxaf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/gxlmxcygg.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/gsvhvpbnn.sHtML

Ruby: 42.to_s
来源：http://baike.fehbvm.com/Article/details/gjdizzwlg.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/ggvhlqtno.sHtML

[A08] 取整与四舍五入
来源：http://baike.zdbjq.cn/Article/details/gkyoqdvlv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gpfiwwzxy.sHtML


<!-- 参考信息 -->