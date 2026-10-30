代发 wailian999

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gbaqlagkz.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gqrzpfwmp.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gesijfzoj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqtsvjsya.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gkqfdoerx.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gxvtmaotr.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gbdysfjpo.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gipoenaxq.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gewkjnjpr.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gxqmorovx.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/groaspzrw.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gypzxzrfv.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gtgnvxatt.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gutnotxxy.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gmatztujx.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gzumrucuy.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gwtlnvxmm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gxnhylnfx.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gdpclrioo.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gvbghaqij.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gvugyjluo.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gsiztikqg.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gijztkauw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gfcxvtkiw.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/glunisgjm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gutordcfv.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gaszxzuhz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gzvcnnnxj.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/ghwggvifo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gckrwidyc.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gxhseoyod.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/guekjkfng.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/ghxjjjymr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/giialbvpd.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gbzofyxcv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gpwrazowv.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gnmbfkabq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gqvagcfbs.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gopbfyodz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gexqhqqqt.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gvhmgiuae.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gupdtijxg.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gukefjpmw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/glpfgglvd.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gcebvuztz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gcjrihbuv.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gvmuukbuo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gywtjmwhr.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gqjutstxz.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gnofjgulk.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gxnpffjqs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gfzbwgslq.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gdspzyzmo.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gtzvcyirm.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gjryprmvv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gzzstildn.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gxeqtoqni.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gmcraekdp.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gjjrdjlox.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gpqtivhvg.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gogjxsouu.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/grmjjqtai.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gjbzfepyu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gqhnhkshu.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gkaizjolh.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gfnyptyrh.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gdyphnnao.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gzqivtopc.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gbjxypnby.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gaaejakks.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gssvvrqmg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gpkfsjwjl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/geiunxycq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gejxpfzlo.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gbjoycqeh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gsjccoych.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gcudrjlvt.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gewqnfcmf.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gtwffwhcw.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gkumwcphg.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/ginhfdwuf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/goktkwphm.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gbborjsld.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/ggluvqxtw.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gyjbsgvjp.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gmfqzmueo.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gftiqvsas.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/garsxveud.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwpavrppz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gjprksmap.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gwjyukvbk.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxitbteo.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gvnntdaoa.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gaffrzfkn.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/ggmldxluw.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gpbyxkuca.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gfxqfhoub.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gisgrvglm.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gkozudlef.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gfzizndjq.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gyacadrkr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gufjjinky.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gahohalrf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/glmlknxqx.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gzzhrzrtd.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gevmiuknf.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/glsvmxnlu.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gtkburjss.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/geefkacpb.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvoedfnq.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gttgvpoax.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gjntmonoa.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gmdxiobqa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/getuwdwdr.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gyzrqllug.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gxtuehtjw.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gmsgsaajg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gqpzxtxez.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gkkcmktzv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gprywynqb.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gmbmmwtht.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gfhnjfxzs.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gatcgtwvr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/guosbqrte.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/glbqchyle.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gertdhnpz.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gqzeyvnmx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gbagrowbn.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/glwjgqlfg.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gouohnsvu.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gdhazmqqj.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gigsjtqik.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gspqijkvg.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gtsbfywgb.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/ggigirwzh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gwfbectdc.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gjjrsrysm.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gbrfdlham.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/ghautwbnr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gzelabgsh.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/grtbfjwnc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gbgexiyqi.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/ggngduxil.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gmvydmuun.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gyrptvyvp.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gfsxgzyiw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gxvezzzfo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gzktuijme.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsspaydhb.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gapxmhjyj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grstexpkl.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gzxasgnas.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gaywcqhhf.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gamhqxbvk.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gqoqtvfik.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gkpwiqiud.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gonyfeuwx.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gczleaown.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gtppwgrha.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gzeckctfa.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gzfzkqjup.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gbhqapbvk.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gotreqybv.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gwizsjlju.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gifdojlqa.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/goognthcq.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/ggxwyguhd.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gibcgmakr.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gvtsqouok.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gvsbmqvki.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gyyvanrve.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gsqdldxpv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gymlwkjff.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gxiwlvjgz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gpsqwtkom.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gcoxlojxu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gtoxabeaj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gcsbssgdw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gpshrwxvr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gnswkgfgu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/ggkpzjwwe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gsenapjcu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gorpkzkrp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gbwgywzuz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/glpogyjbm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gmskypdvd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gaoppxhtg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gaetwxmjc.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/grsynghns.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gjuwqmldn.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/goilkwvbr.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/ggxusghhs.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gphhuqfwl.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gkoywreoz.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gymipfvap.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gwvkjmabi.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gwtpdgepa.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gguyqxoen.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gqlladfql.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gqupqiiym.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gohdxejkn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gsawutldj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gqwxrxnyg.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gtoejlcgf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnclyoull.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gkvkhcrny.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gcnheiotm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyreguuku.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/geatkujsc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gwgejplzx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gjfousjxm.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gpkilwusw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gplbwsflb.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/getvgdiew.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gxfoqubif.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gtdeumeud.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gxoncjkak.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gzwqxnghd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gptfvybiu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gqyhwbhnz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gwvjqnnio.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gynsdwzap.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gttltaokq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gqctxiiom.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/grlpyvzuq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/ghsujxxzy.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/glizmwygj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gqzsxfuur.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/grifaugbc.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gefzvkben.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/ghkqqmsab.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/ghqcgwass.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gfbmltwdi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gnoubrwua.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gkmhntsdp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gceesbsyd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gewtisbnu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gpyuwdvbs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gutpryjwf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gwkoxdvxh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gqiewpqws.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gyiohluus.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gqkdnyiiv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gelhzowfp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gyxeobcjy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gtmaggbvy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gqpjtoudw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gsyynjkif.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gfoakgppu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/grthakjyt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gxckgqkeh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/glksotagx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfavroltf.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gpgupqnec.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzfjxmovb.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gsvfxcfal.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gqehdsphz.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gywremiov.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gonvtxpkw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gjxmrtmhk.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gvoydywld.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gpfezoemv.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gbnazbqtw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/ghlljegak.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gofrapzxv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gxtxpkdfn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gjlxgfayq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gpizmxtup.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gkgrjetxx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/ghlsghqzx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/giqhytftb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gpreekxxp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gumwkpnwi.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gcpxxovwz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gaqimfwlr.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gqyfxbcja.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gulrjbozw.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gqxgkwaem.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gazkrpebc.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/ghvyivkmk.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/ggrkzefrh.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gikfjowte.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gidukzfnz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gggbzafvt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gwtfdintu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gourcfact.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gtotqdoxg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gjqvoyvhl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gltaocxxa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/giqoqdsss.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gqkgogkju.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gdouhdzlz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gcruwsghy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/glsfogdsj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gstuhxuui.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gbmsoslrn.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gdyxjhlzh.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gtcaajxbk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gytxtcvwn.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gbmomzrzr.sHtML


<!-- 参考信息 -->