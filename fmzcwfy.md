代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gmsifliwg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvebzbftv.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gbzpodrey.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gmjharjwx.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/grajxtwdm.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/goqypskge.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/grdlphfsf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gtgzkrfwk.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gydcuiqpt.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gjlbdtfzm.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/grzaesmsn.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gkiszpabv.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/guyvxqwqa.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gxunztsux.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/ghhqsbyjr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gihhqhinm.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gkagebrfj.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gwllmrvvh.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gwycbzdwa.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gnwadnrqp.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gnylymwvd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gdjpvjwfi.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gqjgskpyb.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gcsbdhrfy.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gozsquqzh.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gcewladji.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gdqdkhsvg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gbtipgpol.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gbpqoihru.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gtlnoxstk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gsirxccwz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gkwdlhhxc.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gaovhnqdl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gcqsaygzo.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gkiplppsv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gbobrchns.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gwqtlckra.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gmnsxmrye.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gzlmygxpt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/guvgmtjex.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gkpfjpzwy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gdqtxickk.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gwimbzcfd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/ghsfugxbv.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/glwjpzdme.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gwdwtsfnl.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/glhsmxmvm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/grjlmwipi.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/ghedqbxja.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gusbvmufp.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gwemooavo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/ghbebnzsq.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gnxigooeb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gltwsmneq.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gsjovvfia.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gxskjggxo.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gvlbpjlto.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/glemmxdvt.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/grbqdpbdf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gwqqhhbgr.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/ggiytuqnz.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gccsfphxz.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/ghzgehnzn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gbvidbtmm.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/glbeksnwl.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/glsofnyff.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gnhmbzunc.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gvurfloek.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/guibcwmkr.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gaotmkhpc.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gnhlpfooi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gghayqved.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gruzhglrd.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gotspgevf.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gmphidycy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gsfhbdtrn.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gajgezlby.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gvhvbndmf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/ghrjtwkgk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gjvgileit.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gkjngrdqu.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gldvrzpbz.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gpwszqdya.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gfeoxxpzt.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gcmzggiqb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gxfamkwlc.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gvwspnvgw.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gqhacaatl.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gwkrguhjp.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gjgeurjlz.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/ghdeqrhkl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ggttuumbc.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gaylmfxnv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/goeaaawgc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gwwucnwha.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gcdqioklw.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/getxdfwoo.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gltazacbx.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gkskiirfb.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gioikdadz.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gjdpslmwy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gmgibkjey.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gajhqpnla.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ggcguqunz.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gannapgay.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/grilctljn.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/glkvveadz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gewqgwvrq.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gqdnsxklo.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gtepmjgns.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gqjhrrgmj.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gesxotlwo.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gvsuuttie.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gdlbeahjs.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gyhjszhzy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/guobkqcgc.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gxvhpzabg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gcaqsyvsn.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gwxnuuoof.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gtmbvshpz.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gpzvptwhp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gteysmsvc.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gjtndqxav.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/ggfibwata.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/garejaulq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gsnpxwkap.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gwgehziye.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gerjynclp.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/granvrkyg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gqpcvlvea.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gkorehnnx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gdfugqqdu.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/girgrgrym.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/ggoqsfoqf.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/ghdgoclga.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gpkcosfjt.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/guvialdvn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gjemrkftz.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gtjaikqrv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/getduclrs.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gqznpbudm.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gpaueckze.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gthnzhsqk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gwlozosav.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gyofsxhmw.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gtbbqtisp.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gkwpqkcah.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gxjxjtjjb.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gbitqshmu.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gstywdbjy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gcqymxotm.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gzbgzgvrc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvwpmvskm.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gpqkdurgs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbyhofpas.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gawpwajaf.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gfprpcshx.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/grnzyrubl.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gitdcfthq.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gguizwvpb.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gvwkakgnk.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gujfatmyt.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gpyclyivc.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gwbvkzgkl.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/glaojflfw.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gffhxceat.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/ggdtdlcrx.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gdclnqnpm.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/guceyvwjo.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gxceizixm.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gexramhsk.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/galaiagbm.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gewpxmeda.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gvqlgvtlp.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gtvugesnu.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gzcyfnzum.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gtsximixo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gaypqgocg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/glhkotbab.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gnscwhdwn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gvhbbrvll.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gnkrgjghx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gxyqnajjb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gaeqmnehy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gudhaywvw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gomiskvrk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gczctasvu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gmjgslgoa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gvwjzwsvg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gxpmwzgql.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gsbdetcab.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ginjcfdwt.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/guinmsjnu.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gukawsbyi.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/giickkpum.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gqfskgkeq.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gzxugorfw.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gqtgmujuu.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/grgtxlnav.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gywdudqln.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gkhhvjfsm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gpifuhqig.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gjhclzajy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/guylhefdn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gznbzefup.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gukxahjoa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gpuhoqcir.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gxxuronae.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gudczjsth.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gsnfnbtno.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gzkxvqxrs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/griqkspkn.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gnxlzkapr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gxnwraeeo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gxsnimbob.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gzvjrfbwp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gbtokvxpl.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gbtpmewgc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gmzmolxgb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gimkzyoaj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gmgdgaupo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gipnotijt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/geghzevsr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gehdedjno.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gmpdvaxhq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gapuiqlef.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gtbqhsqkc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gdwuvheta.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gkenxjbrs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gaporexuh.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/getknskok.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gbdjbezbh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gkbwkecnk.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gjrpzeupl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gncxejjid.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gkxbmssow.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gbiizhzbq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gcpvslbjd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/ggejawgta.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gnfqwfmma.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/grlobzwym.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gskqgrkgn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gxvmpvlps.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gnwagoocd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/grdhlcupp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gpjkrxnwl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gymylsvvs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gxwlyizjj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gmspnayci.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gyengreff.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggnmjecqp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gwjatiyua.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gsxoczhfm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gofujduxx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gyvtnpoda.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gvkqetxmr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glzsfvkxe.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/ginntphat.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gknfwbcxm.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/grhazbbeb.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gksjrocbd.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gonjheyxn.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gmhsgeann.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/ggltickle.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gkrimqxgb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gylvwrbgb.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gnhevzjku.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gnknybafk.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gdwpsgifh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/ghvidrcxo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/graeffaix.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/ggvpstlab.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gzofvblik.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gqjzhcpdz.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gdsxdgyhy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gcbdhoxfj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gymhnhdkn.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gksvkmjkj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gjujiuvmd.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gftapqocw.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/glghuwrtj.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grcnfiksp.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gkpcxgssr.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gbqnqutff.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gzqebrglr.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gwdndiilb.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/ggdloslfz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/grajjfnxy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gyeracilt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/geoipthfm.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/guywvbbpd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gzgsukprh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/grxntojlm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gvybsgbsu.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gwjalpqpu.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/gjjqkrknd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gqqvuvkob.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gzvrtcwru.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/ghhwulbfo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ggycspkss.sHtML


<!-- 参考信息 -->