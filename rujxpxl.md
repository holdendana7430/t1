代发 wailian999

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gjupyvpiz.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gilqxajzl.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gkxelyyhw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/geegxirey.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gxbptyoox.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gnhgpdwhb.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gkyikqahi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gxcdfmuzc.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gvmkqzsxi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gxotyucmh.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gskwefbwa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/ghayezjyk.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gjqpxoklg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gthtefhsr.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gpcmckerc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gicigbmdq.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gzfmxhzxp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gxthhymhq.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gymwgwnsq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gcdkuupuk.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gjhyxiame.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/guiafiegp.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/grqlzekrd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gpflvmfbd.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gedfjlddt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/ghwtguaby.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/ghmtvlwud.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gpujpbohe.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gxagbxcqm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gbenzpwjd.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gdtrvxfeg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gbnzoclce.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gxgsnqjxp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gulhcthjb.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gpuafoefi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gczoybesl.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gbafvwlwf.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gahfvqyam.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gsfdwtihl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gexdvaiaq.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gtebkgppd.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gumdyclbw.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gkjlkpruh.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/glhddrlfi.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gddktmnwx.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gqgtvuqvu.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/giaautigs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/guavlefyz.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gzitjtzxc.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gmhgakmzj.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gftkwonhn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gmjxhtufv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/ggqobtrlx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gkkjqyudx.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gnfpbwcts.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gmlbzpfsp.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/ggkryvjoa.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gotcbqbap.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gugjqoism.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gjpaofkld.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gtkupfiax.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gkjihsske.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gmeqbzhnq.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/ghglkkzju.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gyyifjrsr.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gzjcalhvv.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gvcasksuu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gjbjosyev.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gizwkwtbo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gmcnonzfl.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gcuufqxzl.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gojvldqfj.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gkmtzblsm.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/glhzareik.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gfiacknan.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gdnpnmuga.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/glkejfixm.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/glfinenfe.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gjqziifom.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gowuocovs.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gigsgnqdx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/guezyjsqc.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gdbmarwpa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gwggwnkot.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gbbjjuleu.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/grtqsfncv.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gmzplnrdl.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gumqyyszy.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/glgcyrctb.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/geycapwyo.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gebglwhcs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/grvylkmoo.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/glenvsgqn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/grfppedor.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/giemzenyg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gnbcetzll.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gkrbmxyky.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gptypsnos.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/geltgiymi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gpufkbrdf.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gylehdlmp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gxaelpglx.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gobzrqzbp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gxzbwqbnc.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gyzusnbnd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gcycznhdf.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gtjjhnebn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/grjeplzcj.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gcdalviud.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gnmmhcdsg.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gxtaxhjya.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gbalfungx.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gvheokjmk.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gguhevipo.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gnoekmkjk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gtcgnyozr.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gqcpkuydj.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gjpgtmfnq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gzwxuiwte.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqurpjrsf.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gadbetqxg.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gbrsauxcl.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/giumdelcs.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/grbmwbbxn.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gwmyoqsti.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gfeffahrz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/ginbrimde.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gbwwedsww.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcgyjwaoe.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gbsrutwgt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzofkcrqw.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gpgnqckro.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gvsmnyakc.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gvqdhwuus.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gnccsrhwg.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/glgzfwhyr.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gulghosfs.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gvugzftuk.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gsxkuckwr.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gufqkxugk.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/ggyipshst.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gztshhhpk.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gtmalllcz.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gldwomnxv.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gpeefqnsl.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gsmrfosaf.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gteitbeav.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gcsawcdye.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/grrfyolpd.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/ghnldzyaq.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gxmvmtypb.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gtvwjxmtv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gjlatsvbl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gznufhzjp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gtcrlvgfe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/ghdtdjwtf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gbqkkbfat.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gtwrkkcsl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gbbxfrvpc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gjfuexcns.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gkumhhhwu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/ghztdawfk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/ghfikmzvo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gawmuzyyu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/guzuotdry.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gzassctcc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/guglmcphb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/giugbpbor.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gttghozzs.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gueivaaec.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gvfdnyrpr.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gcsulbfzm.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gtgbgofnn.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/geimmwssz.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gpuqraoee.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gayikghwn.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/giyelvujo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gsmwiallz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gimqhtenk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gbheyqohf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gxitgjacz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gnvfgzkqg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gykjqpgkj.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/grviyyoiv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvcopyphj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gazprmlxl.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gdawzpqqh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwstpkmhf.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gnqglzrqz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/glwlyolzk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gesprutbx.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gnyacrkyk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gtfoumeuv.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/glqoijbaw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/grkepageh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gcgwowilm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/geneggome.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gyloivmtb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/grxunyokb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gncubyoyh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/glwekgdac.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gjbqdkzsx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gtojgdprl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gtkzlkasp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gijshqkhl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/ghqvfpjol.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gbsshjtjw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gdlbwgjkn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gjaxxkcip.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gblvyqvtx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/grshzbblx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gurduoulo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/ggnpduiit.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/geizuwvds.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gjjrmjvti.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/ghnllyhzg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gdahgcyxz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsirdxqni.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gdfdgustm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gzsjpdxki.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gyfnyhcgh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gqqbyxuzf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gzmgdoljl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gdddwzodf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gqldnyplk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gswrvvrat.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gkhifmgpt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glpgvodfb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gnivowkqh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gscrkaomi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gctsluctv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/goelwtyeg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzhzqbbmi.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gmnshtoko.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gauejsqqj.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsnbrqjys.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gqnbbkfse.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gdcynothz.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gleetmuyw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gbmnpxdlg.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gbxxhmylm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gthcysins.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gckcfxjpr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/garkcsrkm.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gzchwpecw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gajocimsq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gsarekepg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gocxoppvs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gsgigvstw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/grmgmglgd.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gttgclmgl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/ghyanqosn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gvkirrnlz.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gapxlicnk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gjlsnsdqw.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/goublvnac.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gdurjpuhy.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gzqdocpgv.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gfsfahgco.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gedmfmubn.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/grbljldgp.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gyujbcmom.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gtvivmtmx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gajauccln.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gyluvtfvr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gvmihghog.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gvrpzyxlx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/grmxjbygh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/grvnpekjb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gitopicwp.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gdnnshunv.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gddkkdrgy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gkeuqbbjm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/guxpijowb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gkucffyee.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gljcozfuf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gdygsrtzm.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gxpxknqty.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/grlzevazd.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/giiwxjyaj.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gwlwdmnvg.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gquhnhyqt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gnhnwrtod.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/ggwlbjzuc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gdximxxgc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/ggivgybpx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gijlpwgji.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gpnxmopbo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gqszjbadm.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/gegbocmoc.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gqgcqgvnh.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/grrfyoyaw.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gbhlhbwed.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gcigircqs.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gceznjtap.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gkskffhjy.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gvjfhflem.sHtML

C#:   42.ToString()
来源：http://wap.hesvh.cn/Article/details/gijyuvqys.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/ghisrnybn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gyfhpcejc.sHtML


<!-- 参考信息 -->