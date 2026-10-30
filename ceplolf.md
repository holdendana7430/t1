代发 wailian999

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/genkurqyf.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gvbaivbrl.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/ggfvpnppl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/ghahsijxc.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gqqxcreji.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gjgizckjy.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gtoacchgf.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gezhdralc.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gjdquxple.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gogvhmnvg.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gyuxdkaan.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gqmvtjevg.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gkdrsydvg.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gylxytdvu.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gbuosukfp.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gjtkvguse.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/guuqmvofd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gbdoisxbc.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/guipfsgov.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gnkhgipdj.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gqludjkll.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gcixztlkd.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gldbxlqpg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gafgiyopq.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gtbffoffd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gissuawdd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gyfymbepk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gqacduswg.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/geqewonjf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gmotyfyha.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/ghvqtjwtu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gmzvqbthb.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gvdcujhub.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gukbwzxrz.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gpufjdqjz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gkxxrreha.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gfqfwvdif.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gnvygvpij.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gylrgmsos.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gtgaxhqdy.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/ghnwovbwq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gugnqbrlz.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gutuweibi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gdpsvtykr.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gnqufkqqk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gnnqsiuiz.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/ggsxmrdod.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gsuwjwulw.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gguvplcao.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gxltghwpp.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gsfdrswlr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gofkofgjt.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gqciiqxmw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gszqthsbo.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gbpbybjid.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gfqqfndta.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gisyvqrfq.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gkixeszeg.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/ghmzbkrmn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/ghilstfok.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/glqljysdi.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gilzooflh.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gpxsajwls.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/ghzdpanmy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gwqpajeeq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gpyyyquiu.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/ggllpawev.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gxufnrauk.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/guwmxysqw.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gsvgpkqxb.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/guacbbpby.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gbadkoitt.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gipgjleta.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gnpvfyanx.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gevbpandw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/givlvwcmu.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gvgugmnou.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/grettygyh.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gugdfiqkm.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gsiljnyxu.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gxsinysyc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gkkqydmkc.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/goqkgsohz.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gksahhifx.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gizspzptz.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gobhzqdkr.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gskyxybph.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gloxhjebb.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gknmmimbg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gjnvxxhai.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gqtxgvknd.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gnfxwiddr.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gnqwkhprm.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/geogzlrqi.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/giyarrxei.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gioszyurt.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gwbpsjeuj.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/ghxthelql.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/geqdbnzzh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gcdusgvtb.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/grovgueec.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gkbjsqjre.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gfjruxxmt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/ggvicmskg.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/glzatiins.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gndvxndif.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gdgqugbil.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gyllfvvbe.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gxpjnujnk.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gtxkrkald.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gwdkepmod.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gcyzysold.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gcefsgmav.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gayebrejd.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/ghdvddfzy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gnzookzsm.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gnjrfzrkz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/geokdjteq.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gyhcyzpch.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gqzyqdpxr.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gnnjrtbkk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gkqanyfsj.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/ggigcizni.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/glymbkkpy.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/grvcjaijw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gfymzgwfc.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gyxzihtjj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gimgehgfe.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gouxzpcwv.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gobmafzlc.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/grvqvdgpf.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gbdkchxar.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gqdvjgcyu.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gerrrfbkk.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/ggbkjstiq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/ghmfdjarf.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gdtzcjhct.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gioyfbmfb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gmjzarqal.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gktskeeut.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gdbhwhdot.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gputlince.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gijgbtzib.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/grpuufdje.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gpvpvntxw.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gpyaykjxi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gcxtzfwew.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/ghitksexj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvguiycff.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gvxskvvoo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkprzaylg.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gqzfyiule.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gzakxbeps.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gmuqratlh.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gufnyhlph.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gotmxdsck.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gmryncfvk.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gzrxydaig.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gagvemkxt.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gdhqfymxk.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gvipnvpwj.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/ggtvwuerx.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/geswhlrqo.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gjepqzlke.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/guplhecse.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gjlgidkzs.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gzobrdvrq.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gavjgffhv.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gpkuirjjs.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gqcnyozel.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gnitzmuti.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gbmqpcqym.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/geybzwijh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/ggaqzwtbz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gedjjvqif.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gojwssddr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/giawgsjtr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gkfekafsg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gtyjgcbvz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gsdyurhpy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gthsmnubu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/glnfmndyo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gsybebrvx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gezbzwmvs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gmiauecsg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gtrfezjrl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gxevkssdr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gjhwiwjln.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gmvvhvdiv.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gxgeydtra.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gwmndwdxg.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gnrwhjube.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/glrcybbwk.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gjxwghwnb.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gukvlwfby.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gcstqzjym.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gsfqmzrwx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gurhesrie.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gtlwlirwc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/ghkkmnemf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gffgwdhdm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gmibgirif.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gmcfuqkbl.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gqsbotanj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdimymuca.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gzpszkqdk.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/geqdyljwy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghokexwsw.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gydprnjcn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/ggmnufapb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gxnzxuqjx.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/ggmwwxger.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gocqfkilt.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gpvlvqrkf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gvgttsybh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gfhbinbbc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gjzplfiaf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gaaiczzrv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gkvcmcjel.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gxqdqptaj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gyfyvihux.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/gftdlpiux.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gccuonvdg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gfoeypiqf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gvutgbskn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gnhwyhvnz.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gflydlvhx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gfnbdmonl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gmsfujssb.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gxenqeypj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gpfqgwlcf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/glchyuawy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gqwgyjyke.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gxjuvuyly.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/giqyietwp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gshcawsci.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghqxdsybi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnmdlpmsc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gtfagmpkz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsscnizvj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gklazurhu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gvkygcsfz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gnzmhprkv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gwqwgjgih.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gmlnxvyxr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/glubvmrrj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gevgxogaf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gyircpime.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/ghkdbvija.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gaivzvdpk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gxkkmqqfl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gexywrfkc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkbocrasf.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gjhilpxgf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvetukqqi.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gnqopdskq.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gztpxthqy.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/grfezvmth.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gdpbyvhdk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gvnvmurct.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gxlbmuobg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gfcmtbdfo.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gcykubvsd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gezfpbkhs.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/guglbgfcp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gzkyxgwag.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gkswgucwa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/glsaqmxjv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/goabcslgo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gqzxieyhk.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gnmdmrwvg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/givzztpdz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gqtvoqijj.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gpqohihtz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gryjmbdco.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gmjnkejxo.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gmftfcevq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gofehgggv.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/guislrgrq.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/goxxvxmgi.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gxkdhpgrn.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmlcsnrvx.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gyofxtavr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gxmwwsjzu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gbnlpysgn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gvicneiax.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gdpfmkosz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gmnjrcjbb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gdvljgotb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gbebxkgxe.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gdntzqsjb.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gcjntzmds.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gejbediqi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gnvisbxpa.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbuijbztm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gqeldfarf.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gtbmkxion.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gnwgmagkj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gfhxepsmy.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gocqxnukl.sHtML


<!-- 参考信息 -->