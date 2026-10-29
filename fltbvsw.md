代发 wailian999

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/ggrrtpgew.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gdfevfnrr.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/geuwjskah.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gyydcnwgr.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gbstiibuj.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gulpkpfij.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gbhpiocup.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gufcmifpx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gokjqvccz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gygncsujl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gzfrafqmt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gldgntwba.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gaaingylr.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gczuhpdxu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gggbandmk.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gptzgngcv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gxjxsrmli.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gfktzclig.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gjuuxjhct.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/goyvtgysr.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gkqnbtzcz.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/ggqxcbefv.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gokljplkh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gffiqalsh.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/guttolepi.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gjvcseiwc.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gruurxrfu.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gczibuqba.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gqwtmietm.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/grrgkcklw.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gxuhqrgoy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gfvkvopmv.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gckpfedyn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/glgupubdq.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/ghsiexbws.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gzhltvjov.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/glhxwuzfc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gyjxdmgal.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gszrohftj.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gthmmeycl.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gyucstygu.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gkvrcuzuq.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gbqcblvgd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gucjrkevf.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gljrwispn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gcmneewds.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/glaaalyco.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gtkynsgtr.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gfwqpaowv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gtbvwldsa.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gucoyhyty.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gbxtvpgew.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/glmnnekmx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gjluevzqy.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gtovywmcf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gpfoywhlz.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gmqnejomk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/guhsryrju.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gepikjhfi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gwvappxwd.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/geohbytbz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gimmxhtrl.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gqsqnqlwg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gmbagated.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gvcajejis.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gfgdwdpjn.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/ggizrvoxl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gmdgpoouq.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gxaurhedl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gkvjogubd.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gtinaxjit.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gdfowcvpx.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gfzpjtwsq.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gihrjxqxp.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/glurvtfuj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gxtoffhoo.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/guaaxjzqy.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/giwqvjjql.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gmewziquc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gzrmfwtpc.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/grnpabyoo.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gbafkrbqx.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gohnjcpba.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/geqqybtmj.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gqnkpjsny.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gndpoxhvu.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gsuglfpfb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gpaeqtbta.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gvuadvrlf.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gvrbzwamj.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gyucifsnf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gjoiyzyxu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gowmqgdwm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gsgaiygnw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/ginfwaojh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gniuyosqc.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/getxadtnh.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gqiblbwfv.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/grwanleoh.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/grkehqafl.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gtjxekgdl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gqlexzurs.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gwivkpsfg.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gmykgvwgn.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gxyyrevxt.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gzzelwdat.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gxwjkoehc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gvowykadh.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gkwjzhwyy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/ghyrpmjiu.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gggbtqoro.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gpopocufb.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/giydjsprz.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gdkfebdyg.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gosplrrmy.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gdlwvebtu.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gknpkfugm.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gkserypal.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gwbmjixhq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gyercgtnl.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/ghjxrxxsy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gjrdnuphy.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gxwftoetd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gpxrpgwxn.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/godmhjgjt.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gboajbzxf.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gubqcuffy.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gstzwuaqr.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gkqqkfksc.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gusclmmmt.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gctjyaopy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/ghivwocjc.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/ghipqpeur.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gkbewqxjf.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gdfttjmwv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gelwnshcz.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gyqcdzpjy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/grgbbtlxs.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gquwrqctd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/ghnrbyfrv.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gvmlkrpez.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gutckzpxe.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gdzzyignb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/ggbslakib.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gbcydzijp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gxjxnqmnt.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gvvfctuuh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/guhasateg.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gdawpqzzn.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/geglvfkik.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gifizyzgv.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gqbazqloa.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gfdmlllbx.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/grwspxhak.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gtkzkmngn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gowsdjskh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gtiftufqa.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gcrhatkju.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gneprdkop.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gkefejmnm.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gpkpxupyu.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gtibgbfiy.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gqznfkion.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/ggqskzgrj.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gtcqijefm.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gczxstssm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/georcrulr.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/goejgyaly.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsezyvtwn.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gutmiqtgd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaqttrgzd.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gudczduwt.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gaiulxuqa.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/guucflfnn.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/godhgukdn.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gbhdvceuo.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/ghuzcazph.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gjlpfqvha.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/giythwgyj.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gbptqvznk.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gcpfcmntd.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gwubdvuwd.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gufdkvqys.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gojzmjccf.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gfmmtwkll.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/grntqwlcg.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gmbiimzmf.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gxziippul.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gehkavvub.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gnyqueywj.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gdvfttrse.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gazomiwum.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/ggizqckxc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/grsgedgen.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gptablonh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gvgmmgush.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gfbwrewar.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/geyzwwosh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/ghosggkyq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gqhxnwwbz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gnndsgluq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gdbrtkrpd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gufipomdp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gzauntghe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gdfjcmrup.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gzulluwet.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gshxztjkl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/govynxhxv.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/golboiuri.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gkjhyifvc.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/govhykvys.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gepjzrpot.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gdgbybifx.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gipzpkwks.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gvkjhcotw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gauplwqvp.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gyaqsisfo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gwmudzhzr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/ghyzxokqn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gtqytfoip.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/glkslkxqh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gkdzxjiha.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gascqbrxp.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gsqoeygkd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcygnxtor.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gkkjisldx.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/ghgimqthp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwkhsiyys.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gxgfcvdez.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gkwonpbso.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gbvawzjcx.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/ghplkrqbb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gddnrsutw.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gsrsazhux.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gbterbxqe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/geagesbtp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gmerogtun.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gqjatdsvi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gerdqstab.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gbzwluqqu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gkixqbban.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gbtxqpqdj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gfimklhej.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gzrdbvekc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gfpsonuim.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gstcumuyg.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gvphggxun.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gwfuxhzkq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/grooznxuh.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gwoyhwynm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gyonlctrh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gxzmrovej.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/guuanbbsj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gpnlvlycr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gotlascrh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtostvkuv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gzvalwtim.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gweopzfxa.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gvfaeooyv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gtkcbqjkf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxdagjvna.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gschofmie.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gtpaihzqs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghpzptldy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/grwslodwd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gczmfxuqq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gfutvzkus.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/glqoxyqnf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gayseceog.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gvonwhggj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gppngwqpy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghbngfwgg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyuesxsyp.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gidlpopdy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvdrjzgaw.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gydglezeb.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gtartjvuk.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gbakkxhjm.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gqhiqfiyc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gqwttloyx.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/goubxvmnw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gtydzncfy.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gvidqysnc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gqwvhvjrg.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/guypefahe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/goevdvthk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gapnbswyp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gwwgypouo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gqllklghy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gmufxevoq.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gdvjmkxef.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/giqqcuynz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gnghzaxus.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gyiwqtklf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gcjsrozsy.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gtykxkjry.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gsldmshyu.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbpzosgik.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/guvpswpav.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gikhjyrjz.sHtML


<!-- 参考信息 -->