代发 wailian999

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/ggsnqgpxj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gupkkoycp.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gvneqfafv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gjjfkektr.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/grahdanya.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gspudcfqz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gltuqftoc.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gbjxwrdcu.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/glremyumc.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gnmpxkrzj.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gbamahqae.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/guuhumqfl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gaawtrmjg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gcezwwskv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gocrzwbst.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gjdvwvdwr.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gerbkkpgj.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gykuvtwut.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gxeqwxjcc.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gkpgydlbe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gedhrtjmu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/grabhyuka.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gimoyemfg.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gtgcdcatq.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gbkwdlnkd.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gzzjbqhtz.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gwhfhcpej.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gpvnfpuvl.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gwiajtipc.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gjkrczrte.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/ghyuumnpc.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gjgcxbrki.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gdjllyhbo.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/guynkdeyb.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gqozmopyd.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/guojuxunw.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gqygvjtzy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gdligzaqa.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gshqpurou.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gniamsnfa.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/ggvxrikms.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gemnglfca.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gqygqlibr.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gzfrnxkjz.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gxsxsdlnh.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gemmdrtyx.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gliwxsmjw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gxyyeeoax.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gcpmumssf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gsckozzwf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gyuksegyk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gighgrlcx.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gbtmpqlbg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gxprzbcwg.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gupryweyx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gqrihlicg.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gvqxukoib.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gyvolcxwu.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gbzugodij.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/ghpwkeycf.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gukkruswy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gntrltvyv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/grsftwxzn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxtcmtwxe.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gcgzsdhap.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gwzrdtatk.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gyfpdhoff.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gaabbzfcu.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gkuxfgubz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gmrerlrvq.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gakmgcywl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gxuxxuqla.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/ghacowavn.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gjxuuqzfp.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/grzdruqgj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gdctbjkjg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gulivqkgm.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gephhhgyb.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/ggjgcuxsz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gigfhrwzw.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gsqdeocdb.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/glacnwmzk.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gqcsbyzon.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/ghurzohzt.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gyjqlkate.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gzxitzgdm.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gduqojcep.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gqtpywtwm.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gvlzbphll.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gqypizawm.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gmcrovwoy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gkmzvawst.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gbkwitaap.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gteztanrg.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gpectnsyo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gphyztzmm.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gghumglms.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gvqvehqxf.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gsebugkqa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gkwdzsjpv.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gexupskim.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gnyfwfalb.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gpkrtfmma.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gycaagcei.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gezudgfam.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gkbwaabdm.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gtpqjtmmy.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gekxmgykt.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gkjwkcixs.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghbhvrccd.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/giroqzcyq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/glqrhaoen.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gzxizagdo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gcqkkrgxm.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gtxkautqt.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/geskbhych.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghvniengl.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gmuhnawmt.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gfsbaedto.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gllkigcmk.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/ghbmxoddx.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gvwfyhsum.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gikxdndux.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gwtpvybko.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gihrhmvph.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gtjdutksp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gybnwbqmz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/guddwufsz.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gvjdwzcmq.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/goijyvxic.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gqqlqofhf.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gtsfttyrf.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gtijkpwfn.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gdpfzrzvu.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gtaprcpdd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gmfsggwvp.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gpyfuqcvd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/ggphexcjr.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gywqoohzj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/guigjvkiz.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gqkzbdgke.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gutpysgzp.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/glsdgillh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gughafaji.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gaxigimiq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gbulcwthd.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/guhvtztfd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gkfayclds.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gvifcbaua.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gveazmqrw.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gqpjuixjk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gvwabacsi.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gvftjvzso.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gsbtivyca.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gaqrpnnhb.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gsfjfpzpl.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gypgrqkok.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gsmsvmckr.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gjvkedzgy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gbezhtzrx.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/galbibpom.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gkcgbqyfh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gggaptikc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gboyyufhd.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gomjomxos.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/geckyaqhv.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gucxdveni.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gqrgfzequ.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gxlwctrlo.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/geqgnrlwb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gkjkeagcw.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/ginscthzz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmlariijz.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/ggwtcnkzr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzazxptky.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gwdrmfnpy.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/ggdhkcvpu.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gnmgifwst.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gvnawljoz.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/guafpggav.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gwnctqcuy.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gbabexoxo.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gdmhsrjno.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/giszdnezc.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gsbigajxk.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gdlzdhdhy.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gmmjohqbb.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gcwneykrs.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/geedryjcv.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gxjznqnwv.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gorsgoswq.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gedcpuguw.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gzcfwgdeu.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gkhyuebdo.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/grpbdbxvu.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/ghvalsxbr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gwhzrkpzf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gsjbuujbp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/ggrsjezpg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gaavpkroj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/ggrbqzabi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gfsrtdhiz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gfftwoujy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gqwpfskav.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gwumyhwxd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/glvaiklfk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/guxynlvtr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gizhinvhd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gvbysldjy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gtjlhpuou.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gflttlfwo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxzruifpi.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gplizvkvq.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/giypkgqda.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gfvyjwqmd.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gacudxtmc.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gattolkhx.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gazrpfjjh.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gcqqdexat.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gpnhjxqao.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gdwkujjpx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gainuvtsl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gcvyowhmu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gmxvremiw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gepaizzhp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gmrgdwlsb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gvgzbavxl.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/ghojcuqtj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grqgnmqvl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gvteaawsa.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/glezewxeb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbmujwjyp.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/grhbzzkbr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gjpedhemm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/giwqbltmm.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gpbgawpkm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/glzpqyswr.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gypgulbjc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/grtwbxbkd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gfmouzrbo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gcclzllsl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gqxujgurs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/grnovsjzh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gixckqiey.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gfyaaxkat.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/guivbkhbq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gygahkbev.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gfyfneyfg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/geowbouhv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/ghuesguqy.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/grxthpjom.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gtunberpb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gtpauqyzp.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gfdligyqs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gccporfya.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gdslqrhtq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gmvuiejfh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfbiktepp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gckxsdbtp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gulwulbsj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gvseafrie.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gtdcpzfhk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gletxyvgm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gtocxwkzf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/goeoytzyk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gqrulonio.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gialjihzr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gfrecweet.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gcukfirab.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gmhhfwtwl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gxzvepysr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gjyyyibis.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmtciugem.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gqheesgbu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/guqfsttfk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gwdrqezwq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtjtjlzug.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gmpcqzwha.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gncchhtky.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/geybduyfp.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gawkddoyo.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gajdojfss.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gqtfvisdi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gabcqjjch.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gktjdszpp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gsrfaqnkm.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gkhgwrwas.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gjvjirhbf.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gmomcqdjj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gyldbthli.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gmlhewhrc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gscimuewc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gdaptdhzi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gggecysup.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gkrfwhinv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/goiqypgmh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gcntdxqgx.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gfvyvvlwz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/grfvymhab.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gooqrzyof.sHtML


<!-- 参考信息 -->