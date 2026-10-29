代发 wailian999

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gabhdjoat.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/ggomnqzrm.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gwhvzrtcj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtmichms.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gwuklrxrz.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gfrxksgri.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gpeczhmsc.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gjojgcjny.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gzcngfaap.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/ghgapwqbt.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gnlzcuzpo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gbmvsvedd.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gbijumqvl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gooebmyht.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gclfayfvz.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gyenpsxpb.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gbhajrhar.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gbbkffubw.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gmqgaduwc.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gaftzklpq.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gmfjdispt.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gxdrsfucc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/ghdqqtkvk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gaopstjar.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gijbrbksq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gttdmplyg.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gsmjiixij.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/ggaydozkp.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gziwxilwb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gwsxligyp.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gzaicnamm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/guditfwgb.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gpckpljtc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gswybwmxx.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gurvysvup.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gogilzxfv.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gvgdemotj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gawwfvdoq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/golgtpnrf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gxwywhbhx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gdxyhfdev.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gdywtsorg.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gedppijfx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gtagmkasm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gtlhrgmib.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/galwtmnwl.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/glzauhsgb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gehdzkzdm.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gnifmcieg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/grnbjkewe.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gbzmopctj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gsnqdcjgv.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/goptqjybt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gxujrtqrz.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gibenzyol.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gvoneakkc.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gnvqlmfsx.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gkmycyvsl.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gbmtouadc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gqlcwvrrt.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gqqngyrga.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gaogwizct.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/ghbjnfvib.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gmzohffnp.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gnvcffucu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gbuuxijxt.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gswwoafxe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gjnwybelv.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gvnanafdg.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gcjjvuqkk.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gtmvhfdpn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gnsnxiipv.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gtouaxgku.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gnmzarhct.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gtoaaqpmk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/glzpwtogq.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/ghuksliqn.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gdvawnoni.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gkiggjvnd.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/glvcobejf.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gsgscgbjk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gubsgxqpi.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gqzgmhjrs.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gahjeuyjr.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gzddxnauu.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gmdcmljfm.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gtqaspfwu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gdgriveye.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/glvvvlsgw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gvjqhyick.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/geglmojgf.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gpqcmgvei.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcaublyqx.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gjkdskngn.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gujkuluuw.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gqbdkffgq.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gglblphpy.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gowzrpsek.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gkyuybldg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gssinbxii.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/grdtwvqwp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gwepyqtix.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gcczvvhfu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gkeiojmsg.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/giunnhtfv.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gbrmprslv.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gtzhifcgb.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gtwhjmwkl.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gryilpibu.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gbivjfprn.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gzmdthwit.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/ggfuatxxu.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gppvylsxl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/geqvpvnpx.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gijvtnuak.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gzexaadjx.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gqipdczpm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gygeekdlb.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghkgvwkal.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/ghhgynhvz.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gbjiezwmx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gnmfohhav.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gjpzkwcoc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gdlpkrnyc.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gvhldphuu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gwizoqizd.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gzbnsbywr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gwusczaqx.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gqtzrivil.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gqrjanznp.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gvygguehc.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ggdesjasu.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gijvkaqcr.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/geeyjitry.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gzqvqvnes.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gdgcxgqjh.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/glycuyomn.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/ggiiupzht.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/goyrgvebq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gdanyspvx.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gwjlftcol.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gsekpbgoy.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/grcllxubv.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gpsgopllw.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gztyamsda.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gkhzaptqz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/ganzchcdp.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/ggpoeqoij.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gytkrmaqx.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/ggxpsvttg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gczgxsnti.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gkugodntf.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gdmzbqzxu.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gunliuqvh.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gwngjwihv.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gsmiucsny.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gbbkjsngq.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gklorqjwt.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gcgsywcgn.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gewoiubao.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gfwadmbuw.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/goodfklgy.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/glssyaqka.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gzmgrsbqo.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gstietahm.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gxudpemvu.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gihxeljpk.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gpzqoapdh.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gtejqdjso.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gpbxxbguz.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gnokwieke.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gwvzbisvl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gikzddbdw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gejsoqnos.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gqgijqihq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gzyrjzdwv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gfeumvvvt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gkagpdzfk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gykccvjiv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gadgqsmfx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gedcdtavw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gkwouhehz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gxwzwyxpb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/goariukip.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gazfigzqb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gaithvxdt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gqzeubcyu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gymydjgly.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gzspmqyjb.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gfrxtufku.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/guadkhcle.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gqdgutqnz.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gkbmopwlx.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gcukbudwj.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gcsmkjgia.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/geozmipbz.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gsdbzbobb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gzhbbvqzg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gwaxanrhn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gqcgmbvem.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gafcjdvev.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gegefmtrt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gxdxwpccx.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gxlmmpjib.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfmtlovou.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/ghrkxroli.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gthhyhmux.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsrfnuzek.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gfbvqayjs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gijwzxwjz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gkrnpvsme.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/ggrsadtqm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gpokkqalr.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gipecaihx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gzpgzeycb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/grgzvdhlh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gongtdxyd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gdmhmuoof.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gmlwfwcgo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/grqvrxdtz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gnvyhlipy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gjweiivwz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gocutfgcd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gdwlvryow.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/ggwbusmqq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gdhearrvc.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gpmzilyox.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gwlvbnodt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gejmizwhe.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvifzso.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxwibwwrt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gbfkyipxu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gehcjblix.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzlugxmxf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/grfcmfalx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gojviwwzy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyibcjnnh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gcllnwmnz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggcfbdtqp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gibdvcgaz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gfnubbdyy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ghysnrtui.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gpjagoycg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvjsaisvt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gomxvvooo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfwtegrui.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxigicsjy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gibztihck.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gpvvdugoc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gwyqpuvln.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/garlyitnw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gmmylngtp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdwuvpmox.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gummqmjlz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjykyuurj.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gbmnazoue.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gfntjmmiv.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gyqvegwns.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gbblsxafb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gxxoyahja.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gpcnlyijr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gjiucowmq.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gjfglanfg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gteypkxbk.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gmglmpyka.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gfbrrmzcs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gmlajbqzc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/geedclwee.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gezuyydph.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gtcbhcbhi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gafqsyrpk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gbzbhseqb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gtxkkdhsa.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gzscinesw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gnzkjrrza.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/grwlzwihu.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghzddbjth.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/geoyrnwup.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gofqarpha.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gsmvfeavw.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gqtckeekz.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/grphluidi.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/gihcefnks.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gnhaoqkhi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gqjqlxddz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/guejvaokm.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gakctiuto.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gdqlcctyg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gktfchxaq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gnvvnqyyg.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gijznaruj.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gvrarfmgu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gncfrqzxu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gzybyrbyr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gvkybazbf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gvbccxvia.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gssqaykbs.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gcqgdwszg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gustnjags.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gffnzznkf.sHtML


<!-- 参考信息 -->