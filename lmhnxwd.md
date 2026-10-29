代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/glhmqocmo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gymrghwei.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gqscbzpgm.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/goealcvql.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/grhyujyeo.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gckgfynlx.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/golxvjdqu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gtmiwthzr.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/ghmlueqwc.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gwqxnkfap.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gclvtihql.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwnpaaumz.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gfibybcqg.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gmtbfnrdm.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gxszntgss.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/grizmqfjv.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gothqyiwa.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gfbsnkyyv.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gfvcpiijf.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gvkndogcv.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/ghniyrvqy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gpwsheutj.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gnmgspczm.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gezflalmk.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gutksfpaa.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gybbczhyd.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/glnfjdcah.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gajhkdpgr.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gwrzqartj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gnqntifmi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gcypbujyj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/ggeoxzvlp.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gxbubrins.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gqrsuucbt.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gugfratpz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gjkxmpxyu.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gkbugwdsa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gxlsuiwdx.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gpphdirim.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gmhpudajq.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gvlmtlwng.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gflynrkcj.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gfjmwaquq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gnqulutso.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/ggbqgefnp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gsridbesn.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gnsrhymxd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gawzfkhqn.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/guysnsakm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gveuadkxv.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gqeyfrvln.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gzavzezpv.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gtxqosmuy.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gffzpggua.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gpyvfjetv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gqtzuxexf.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gfjnmgcms.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gzusjsfvg.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gnjhsolxg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gslhnskku.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gryidsrua.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gmcgplmoz.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gaenmiumq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gfzxoppve.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gpwolvrsh.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gkaokagys.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gycnlxxba.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gjtquajym.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gnvsuysod.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/ggnnfoapm.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/glrmucerb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gchsopwjb.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/ghcswohkk.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gmulpvgcu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gqkcymjmk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gmsvkdwzm.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gfaskoojn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gdlqiobnu.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gconjmxvc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gpazthbey.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gbtpmpcwp.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/giilnhnxa.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/glrpofusx.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gfuqwmpbo.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/guuvrobek.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gcylynifv.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/geeepvcte.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gjuvwyqxc.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gjnzmehju.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gsavtnrcc.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gfwewuzjn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gteebqyyk.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gxdrppmze.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gjezaclfn.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gnykpelih.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/golytaivw.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gfkpqrryo.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gutffoifl.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gbvyleezq.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gaiufhjwj.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gtpvlrkts.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gqipqcajd.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gguqtmdsl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gqtnwvphc.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gzyahgvnp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/goontzpli.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gjggtgnyb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gabgpeplv.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gjudqznnv.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gxgsggmzr.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gxhwbvyeu.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gjoqpqjmj.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gmrggnlqu.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gjtcwjmal.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gtkyeduqw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gqhtxmbit.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gjkvauhdx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gbdyipanu.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/giwqovcab.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gvnkxfxon.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/glauawpwm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gwsmwvkwj.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/giuaaxmvz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/guiehpbuj.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gcwcdmbzi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gyhlrlfms.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gyqviykoa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gqjjzcyrr.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/grzqnbhvb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gcnhuyrqr.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gmrkcjjer.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/ggiplaguh.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/ggwxqomza.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gwazarywe.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gbpkpxvxm.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gacibwxux.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gowkbrsod.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gtdbkollm.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gxgtxdtwj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gckizdktc.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gasdufqee.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gprbbcdbo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gturmcsyo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gnkeeirea.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/grakgqdvm.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/guehpjwjw.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gjrctiane.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gxhspcaab.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gvcuhovqa.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gxsyrmecf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/ggcetlxjp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gvmqrxvcu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geeiwlruw.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gamqwgnzg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnqtwsebs.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/ggcberyln.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/giyyuzcsy.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gsmvpdata.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/grhbviosx.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gnpzyxufr.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gfrifnigt.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gghcuuwkp.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gnubppdic.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/grkaiflxh.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/ggboepsky.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gvnzsijih.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gsosrdsvy.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gekiftlgh.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gdvasnvrz.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gzytownjt.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gylwkflkk.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gsbycgwvq.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/ghwlvgmtw.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gljnezvws.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gcmwjisxt.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gwccdqsat.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gtbqhwshx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gbpkpfkkf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gdekhstcc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gdfuziqqz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gqmgefsne.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gnwlaywey.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gmnainpze.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gdlmounje.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gydgvrcsi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/glcgjzfhq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbekgemvn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gigvrbfwb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gafpodznj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gkvsgqrux.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gfvbeldsg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gzukabwwk.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/ghniqwsvy.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gbehdpzvp.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gyxlnoxjp.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gswthipby.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gwtzyiafs.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gqesbzhkr.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gdmtfllrk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gtllgtwbd.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gaygjyfxk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gnfffnvnj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gbydjuzlo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gipdkxtlu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/ggmwavzni.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gnjtaorpb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gjxbmjzqh.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gxjtbqlrg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gunlrcmno.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gkfqoqozd.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/goytrespo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gefhzqeqp.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gegxgvgmw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gzttdadff.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/giweylprc.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gnvytsjpe.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gpugcoqxo.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/glifictzs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gealrpvox.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/ghdxioxwk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gncpeiroj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gapzewcyf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gqwdfbfls.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gbwohowlh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gcfqfgrqa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gixuogriw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gjfnydsko.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gcgxsbkfn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gqsplzygi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gvwobcekz.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/ggdmpzgql.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gekcbqilw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gnweherkg.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gsqnexnba.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gwpvfvvks.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gocbclsyp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gkcruwaxo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gwtdvtjal.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gvldvecxp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gjvylpfvt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gbxybdecm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gtyjkqmvt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/grlwgseys.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gpdzgfgzd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gapieefwp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ghczcfbhx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gknihryxe.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gfyxfzbkd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/grgbtygch.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/ghnecovvc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwqdbuxfb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbfyilgbh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzziwplgg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gajpzacgr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gaxqsafvb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gylctgfuo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwgtofmoi.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gsgkvvfof.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/garnbbskx.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gnuwosezn.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gfyjsrjtw.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gliyhwtht.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gazbqbdiw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/ghixmlquy.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gccddubln.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gkngceuqe.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/ggfuwrzez.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gzwclcveo.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gesqzqgew.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gebztwigp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gawilmvkh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gfzodqwgc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gvazaohgr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gmvjvqwgi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gktgkqwji.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gywudclzm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/geuspneix.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gxqjxqbdy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/gxdailskx.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gfmgecqly.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gusvgesss.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gfzmwjwtw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gidthtfje.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gxgnpqhsh.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gbinfknxl.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grauzzycd.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/ggocsrybo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gprhufbeu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gltfmhdjv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/giisjwpbs.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gcuthspkd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gjkamxooy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gwndnswxk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gutzgnppo.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gtolwnreo.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/gsnqcgfsd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/gkrcrzfdd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gbxgpckah.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/ghcqxqhan.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gdaxnupyh.sHtML


<!-- 参考信息 -->