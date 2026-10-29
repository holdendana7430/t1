代发 wailian999

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gcuvbgmfo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gegksfykr.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gfwfetvbp.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gtqjqvfrz.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gzbmgafpr.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gcezjslyo.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/guhxafiwl.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/glfnbracl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gwawpoctr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gxgxrcbnb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gnmlbstul.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/guvdifgwd.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gtfghulmn.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gcxdodtri.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gmafqrebb.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gyeygfdnh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gvyxiwjml.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gzuvrzntv.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gamfufjyc.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gcskwmfux.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gjsreobpi.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gqfdefndr.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gfcqmdenx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/ghhbkrlkg.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gugphqpqq.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gfbonmuup.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gtmgxmgyv.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gnetafwpk.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gxmzpkssv.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gxxzjczkh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gxwxkejre.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gpfhhnqry.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gkuhstfed.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gykmfsnpd.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gsvypzxyx.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/getwgsuuc.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/goaeufybz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gcrrslhzp.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gvqrhwwnu.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwfgaomju.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gakfkifaa.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gndksonjv.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/grrvlywfp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gcnlgnozd.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gqdkbdbbp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gxyoonjfj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/grgcbazgw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gphxzaoga.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gmqxcjjin.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gljzqrydg.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gsvvicdmw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gkvprflrb.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gjyqradxl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gwcjlyldw.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gpiiwnssu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gcvbvialn.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gfroauywx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gppzyceyz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gamddvwis.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/grnswhwyi.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gjrmposwv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gswxrwsvg.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gnvhgzbkx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gvhzxzpui.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gtezanefv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gbjciragh.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gwtlrabkx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gbrbrzbkh.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gnlqxazxm.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gnssukrpt.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gdcndlbny.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gximydwql.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gjqmimcvh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/golkezhnp.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gwesfwepy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/goefzfork.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gikohxmvd.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gpveluswu.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gqahjfiks.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gbdtsgxhw.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/ghwzqbfzn.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gasidevhm.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/grsmokhet.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gnjcsiktj.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gwzcgmlhy.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gwzxacbnv.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gxrdutore.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/glgbqlumx.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gmvlwvsgr.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gmtfnrohq.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gbypfdrgk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gxhldxxsm.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gucfqegnh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gmhptltot.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gyzljjepo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gxsdpzsha.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gmxrawfhb.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gkcijcacg.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gqnndojtc.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/geldpdsmt.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/greoextox.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gdkociiwo.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/grpkixnbi.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/glrhwyizf.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gdbulxlec.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/guptbbvvb.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/ggjpofwgf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gkklrrznm.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gadaxghoc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gcmkbizdj.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gxbwztefu.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gmhvfyhnx.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gioqfxahf.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gfwohysdi.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gtzgrbkmv.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gayxlyifv.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gxmvwsdbl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gmtqkqlpd.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gwunefpvf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gdjtsvhfq.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gegjrjlgz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gapushemm.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gweccdljd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gaskqmjyd.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gbqyywich.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gdbkelzae.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/glqtoidvb.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/ghdgrwybr.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gixofuezu.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gkdmzuvso.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gukoopkxa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gmuqzaobi.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gcrqimhcg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gemkvqpar.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gztjtstgp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gmnunpktw.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gjkifdkjy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gcrjlocgo.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gdbphatqm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gwwrxrgdu.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gdagwwhwt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/glgqwvchn.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gvnazofps.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gdqzzofmr.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gndokhbmv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gglfetbgw.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gzozcslfd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/ghwlopcyj.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gzuhpitto.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gcaapbqsn.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gbamxunia.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gyqxvwhwq.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gzdojodbt.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gppfguesn.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gamxerjmu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gjcdxuirh.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gcqwbjrah.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gmdoymqhs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gzpyvajhv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gqknhufry.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gocshoppr.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gsypyyaqi.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gvgstrdai.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gqibfpdnu.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gyqfjgrmh.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/guyfabhcn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gsoukxlvc.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gkganghwv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkabotgfa.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/glrttsxsz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gctlgfthh.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gofbkwmmo.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gszjsdase.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gtkoojczd.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/grumotvvv.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gkpmmyhwl.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gkehrrfzt.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gjtrmkhyt.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/grvadixws.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gonocwsrw.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gkvsneukk.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gllfddyju.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gjyhbvqgk.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/ghlhpxuyl.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gebhdinbe.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gznphltqi.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gkkajnjgo.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gdqgfoozi.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/glhntojol.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gcyfbzfya.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/ghylwdshl.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gazsgkkyt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gxykxlmgu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gcmmbjrnr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gxtrxsdrr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gulcukmdd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gtewegekm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gsbibohzj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gdmvfqhzp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gixarzhdg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gvuhmhxpe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gscgxvfhy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gclkyuhjt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gunndqlqg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ghorhfuqx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gceizzphl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/guzfpluhc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gxytjsrhj.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/grtennyfy.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gkhowzrgx.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/grijvjwyd.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gouafwsjy.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/geakrfcar.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gejjhlcde.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gvqqcqchp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gyecmrlkt.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gpbpkxvka.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gwbxbflvk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/giphylvgk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/glyzoovbi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/guuhknlmt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gpuysnbxe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gpxxmhpwl.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gcjjvnumq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmiubrdia.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gdnjcsmbi.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gxzmbomck.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzwebskqf.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gnyfqpeqv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/grrabivdi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/ggaupenxb.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gpklmaxbf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gnrofirwg.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gdlthjorc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gsnpytvgm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gmcrynstq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gezkzvmpt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gzigizqrs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gxwuholik.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/giooovtgy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gnwcymuew.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gizgxgzzv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gdrrlecfm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gwsucasmp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gouraxykt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gnechftju.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/ghcpwbuoo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/glglgdxve.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gfspnsbrc.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gdaogmopq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gecsocnps.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gazjywfuf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gthjgfzap.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gkfzxvang.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gqpdulkwp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gvnewqbhv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gaohdplhb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gncpsgmxf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsnrcdwfb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gduroqevs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxshycgba.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gcmpunhnc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/guydbmsja.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gzamyubwr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gwynrdxzq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gffbwjubd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gyoulejfp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfvchbanz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gublsvnxv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/geevoafaf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gtwgjbsoi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gymbplvzk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gglpefmzy.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gktfilbyp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gffroltdl.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gltdbssrc.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/ggnbkpkwk.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gqyyvxzpd.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gcivrjmqf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gwpnztogq.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gnxvqmtfw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gyxkwsutt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gckprfclv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gshgkiwpt.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/goiigdytj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gmwhzvthh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gcxppvdts.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gaxnfwnbx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gqpaopbcm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gyovymgkl.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gixssaqzz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gwltumiat.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gvnozspsf.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gzuwjvqdo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gwkeiiuzl.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gkaucjpun.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ghjgnnuhu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/guyiwximy.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxzwzghse.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gvunsiwjh.sHtML


<!-- 参考信息 -->