代发 wailian999

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gjptjwrrv.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/ggwgpoxwu.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gqwwhlhoy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gxrnoujtn.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gsvjkgykd.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gfrsqrket.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gpiszexko.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gateufppn.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gsyrvhjzd.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gnbhqqhqf.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gkvxbowvt.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gvztptwdg.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gtriryzpt.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gjhstphii.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gqmerhdlg.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gdqtsuisr.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gevbmpgqz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/giqylcxsu.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gbxjyiwfk.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gimomppsy.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gfeevybxa.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gcnjimfpz.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gscewyfyz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gizzikiwm.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gigutlqce.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gricfaeyv.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gtkvthsxw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gajkfjvfo.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/ggpcswkou.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/glzwmxgtf.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gmduqnces.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/ghmyrszst.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/ghjiaonoz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gqfbslfvp.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gutsxgnyb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gjedgtoiu.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/grgsvmvyt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gmjmansgb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gmunbllxo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gcynpbxes.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/ghabmgndz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gtjniwlem.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/ghymplotg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gymbuwlpj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbtsqatqv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/grztgldnz.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gintxosbh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gkqbwxdzw.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gtlxxjlyr.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gxflzijll.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gpvzjwmjy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gyiusvurg.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/godsriqlf.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gefehurzq.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gsorcosvj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gzvrckowv.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gchgsoore.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/grweayron.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gvkzjnggr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/girvgnpwn.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gvmikjbry.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gpotsqdfl.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gyarhezdj.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/ggqzbsshg.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/grftvhcqc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gautbuceo.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gclxydgku.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gelipuhju.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gcvenxsis.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/glifqcmaq.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gchxyajvw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gcixhpawa.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gonzdbkxb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gkrxbhfnz.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gnvglinrj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gbdegbovp.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/glnwsbzbq.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gdmydmtre.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gkcsnxccr.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gfuufprhk.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gmnnxcspj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gveubohez.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gndgxgyct.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/guuaudogo.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/grgzfdvhc.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/glonsgyel.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gbmhiykfm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gutxdwlqm.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gttzmcnim.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gtwiipcjw.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gatfcxckm.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gkszvacbk.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/greyteskc.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gokoxfngj.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gkhcmlppv.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gfrdxxsff.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gtgbrvadv.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gvrtdnenp.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gcadjmnpy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gvokagzno.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gnetuummm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gvcmhldov.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gulzikcgz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gcetqowrj.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gacnxeysc.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/grkpuqbhv.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gclnotzax.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gcmowihpt.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gkdcjutpm.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gqoxkbvth.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gsykaenln.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gwnkxnquh.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gjhnrklds.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gvuubfmos.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gqyedyiom.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gytcbfdom.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gfvqwoclt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gwyzxohcu.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gankfeosl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gfarxtloc.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gcnutikeo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gxsgfehjk.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gqoyyxzfw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/ghdyyyoup.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gatbgbpzs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gpuenrsrq.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gpcutqojm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gtbgzfvbq.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gcqabgnss.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gbhstevzl.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/grcqatvof.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gkphsyyrx.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gijeuxwkw.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gimizkrxa.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/golqjwgvt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gamjxksve.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gqrserbco.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gsvthycpu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/grpalbdbn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/giwmhzszf.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/godddkqdb.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gizsmhrnl.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gtbhkowip.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gqpywhonv.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/goiizxirw.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gxxekdekk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/grmxaofxh.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gvstchohk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkywgxnyk.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gholyqvqm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ganqbhqqw.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gkovhnjny.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gdgfxfuay.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gnpvatcaz.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gbydryhgw.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gymxxstsq.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/guuyzupbg.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gfdvevzlg.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gzwushmce.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/grxbhdbyv.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gvmpqdicg.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gugbxhrhi.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gzcxmwbgf.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gkzvsgzgm.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gxqpilxsi.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gwnakhszl.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gpnszycqm.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/govbhbfpe.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/ggwbivwqb.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/giliibjez.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gbkffjlbb.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gduldxhaj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gmzvegqzq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gelnhpgiu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gpaiwkknr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gzgspvgjn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gxguydhug.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gttqinrgn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gogmlqjbg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gfhtjldmd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/giuhskpsq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gdmwjuzdy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gdcfibnwn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gnxdgkkqn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/ggjxlriri.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gphveyruq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gjoxazcyg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gxmynvoqu.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gvvhunvan.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/galriagck.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gicmqmhhh.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gfmgbkqcf.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gwmdsufvw.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/godstccyb.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gqzkogoam.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvwxkhadq.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/ggiigdqer.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/geurvnkej.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/ghrarviau.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gxchqwbfq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gnpgdlebt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gjvvyrgln.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gumrsufrv.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gojszmzor.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyyhtmlnc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gctdooxbt.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gqrdfpaig.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkxsminvo.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/givjnspgj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gxgywshvp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gzpdvobuc.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gbahxjzcl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/ghwvvpzei.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gjckpfuxq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/girirgdsc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gpgazyoxa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gyffykygo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gsicbpmlf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gvajfenpt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gebfynjzc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gvljfyqmt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/ghxfxcqmi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gmwtdabvw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gvcikvtqt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gtvcbalkm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/glycpimji.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gajshcedo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/giugdtyfv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gomyaxszk.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gwyiqjczh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gbbntpbow.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/getadyycr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gxpbwdzey.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gieakssdm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gqotqyrls.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gmxktaxnm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gduftwjdd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gtnmxtfkw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gizwodeoy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gpuinvgkz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gjonbbgzz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gwsjcsdbt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gnystzoyc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gmvzsombs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gcbnvrmkr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gnkyypwwc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gsormfdxe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gttxzswvb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gjfncuhsy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/grufebsnf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gffxdlmhn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/grzawnizh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnsgjhagw.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gmquwgqcq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/garqmcfau.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gtqzppvzv.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gouvviihs.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/grapcmnta.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gmmaykfco.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gtpqxyfym.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gcvpuhdeg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gtazztmuf.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gcrkeaixv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gnawxehti.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gfubwnzux.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gbjnskqxz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gobsyiqfp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gqtlvajkb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gqqzqbtay.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gsovmpxyd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gahakurys.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/grbzpbwix.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/grblqsrxk.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gbalttjbw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gvlophusz.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gamefoidp.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/guxcryhan.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gbajawipx.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gehnsydct.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gjnbxhycc.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gxkjeylgt.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gsvyfhfwa.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gczhjdvky.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gigcsvroc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gtqyufekm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gidxtsntw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gunylbiav.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gdnwafqzn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gklvbcimd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/ggjjhiiec.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gxbkafbqb.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gdakjhdgl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gbebtoipm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/ggcksarhd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gyqbnzzxb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gcgqcrryh.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gkedxpsnw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gxdslymlc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gtjqvsbpf.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gspyjheqf.sHtML


<!-- 参考信息 -->