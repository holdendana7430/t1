代发 wailian999

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gczybitzv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/grbdtgocm.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gsuqkcvxo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gywfwsibc.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gnhfqbqzx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/ghwhvakba.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gldqbzrgn.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gpraicsbm.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gglcifjtl.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gftaxhiff.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gcfokrxxv.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gjglsxwon.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/ggimizcvx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gfzxhkqsv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gmzwcvgjq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gowumknrz.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/ghtumvhsm.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gdjfejwho.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gwlcgdwhl.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gwoxuysin.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcizcytfb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gsaxraxbq.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gucgpxfdy.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gasacqdgg.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzppjnhrg.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gpqiaarbh.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/ggczlbbqz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gjeucdgzz.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gcgissfed.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gzozgmuhy.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/glrabkzfj.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gtggnvjie.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gnrupjivs.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gpuumkasu.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gxjejdinx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/ggeilyamn.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gaaklgfcg.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gxhhomtje.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gfkmgtuyi.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/giaijbdyr.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gvtjwhqqn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gvcgrgxme.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gvdppslvh.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/guxregeaz.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gklwmgbnf.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gddhjdtjy.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/girdoxemu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/grulspmds.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gqfmhuwuk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gscnbcbud.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/glfwtydnn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gieprvdck.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gpoklhsnp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/ggpxmirpy.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gpavopczo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gghnaopkz.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gvedgsfuz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gdusqzizd.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gwzkfsgyf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gbyykfdhw.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gmgryebqh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gppegiffn.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gllhzupnx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gxsuuezjt.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/glxfvehml.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gfdqkfwxv.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gmuoatttm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gshqnqmib.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/grbjquuxu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gvqwsafyq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gygufrqdu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gozbfkcmn.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gvrabjanl.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gjtozzxfp.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/geeitgvhg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gwbbwupwo.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gcbqbdrnt.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gqlskwaob.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gbmwregop.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/glikleyth.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/goxpxehoi.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gvhdjydaz.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gzzspjhtr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gyydomifa.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/guhsbkeor.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gowgtuoit.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gjsnxmgmw.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gruiknwlq.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gebcebtel.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gxpdiqohd.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gikkcdwzl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gmuxpujlh.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gyrsmhqpg.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/ghbdfbkvs.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gsekzuwne.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gijrifoek.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gsbwyfuza.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/ghlnqfgya.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gvotmygka.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/giojuwkgp.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gcajfoujp.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gdgitudom.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gmstebxun.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gctjkqkdx.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gqvpnjdoh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gsadxijky.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/glaorltmt.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gexvyirbi.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gsvfhkpme.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/geofnqhlf.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gqvallwrk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gcgxjrzws.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gjxnqeznf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gybcedeym.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gwtrcmdde.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gscfjnsog.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsezduyfl.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gnerudbto.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gcjddlsex.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gubcanjjs.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gtxyslayl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gzzwtvpjd.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gofurjdcd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gvbrdhond.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gusumfyhe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gmzmilxxa.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gukjdmdgx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/glfnvutgd.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gxmvjbqfw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gaqbbvkrk.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gagbkxyda.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gqcbcxbob.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gtpmsnora.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/genxvzlny.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/ggqgsxxhn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gmifioljr.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gkhaaadiv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gdqtvizla.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gvmeuqnba.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gmismigjb.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gqjpevstx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gwvqeupwb.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gllhrhjpx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gtaemcrsa.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gxlofmysx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gcborddds.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gxivowzbb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gxvvzfklj.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gkaxunevr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gzrbpdjln.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gujxocsfz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/ggudpdydw.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gehzsthaj.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gootpwegx.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gmrgqndfc.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gxsztcxcb.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gxjkgkcrh.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwpkcnxhl.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gseckiuta.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gfrtnzrbl.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/garbempdg.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gsysjwmdg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gasgtipif.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gyixuvafb.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gkzxkucxx.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gcchrkneb.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/guihgkfrk.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gfhenvdsu.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/ghanmcqzr.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gwkqudlcl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gzlmlosdo.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gqznudali.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glqtqddin.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gstbjpaqq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcxwnieco.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gjwsixrvg.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gzvnypuva.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gsvvjeflf.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gkrhqjjeo.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/govgqxyki.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gasevbnwz.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gcnoaogfp.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gpkbtcief.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gbyhlizqf.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/ggrpsgluk.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gfjilgair.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/geefqmfhr.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gqdjnuqoi.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gsodtxcst.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gnixznmth.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gygvaokig.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gguvlxgar.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gcmckfjzv.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/grtstpnvd.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gilmsgovd.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gvoseobbd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gzfyipvvv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gqzzywtaw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gobkrhssm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gpkgpxvlx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gnonazcwx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gkwuhoywr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gvttiiadw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gwxdvikvo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gifvnengr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/guycjtvag.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gcpimkaqc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gpvydlbvw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gddrudhvj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gszypovht.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gzizlkzhb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gvyvpphcy.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gvkhbwxhn.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/ghdpqcwil.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gogoalkie.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gfjoznytq.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gxrpttnro.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/grvvilzmo.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gsdjbxsok.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gynbciujx.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gvgvwmxlw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/getmikbei.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gztgxtywl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gezcrkhbx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gjlyecwhg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gfpkywvfu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gmhmdtwzp.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gzbzlhcxr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gupaetfba.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gevexoiui.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gwdlecgyb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzvmjyycz.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gkcozlylk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/glcuuqtqo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gxddpdfhy.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gppexzryx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gvvufmies.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gjbsoegrm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/glxunjaks.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gbfdhjxtq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gogvfszwk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gtbgndcgf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gciivroyu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gantoxmbf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/ggvwpmefk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/grzssmtzs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gxuwvgrgn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gixpdhwql.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gxarpbjwm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gwnsgbobz.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/ghvzwbwjq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gdnhkhdqg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gfynpdbrm.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gnsttacye.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwjbtgrts.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gfrfhbzde.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gvmdbskmr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gnqusnkja.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gridxfkrz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gisawteoa.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gbsgbsxkp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gfgmdeadm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gtgvxumae.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/glkhuvvuy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gjonrvqfq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gqkpyxalp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gidixokhq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gwksrdklc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/geuhlvtkq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gtejmyolo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/ggxjpxmuu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/galscxjyq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjcmfujsy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gblslkrfx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gtgqbfmfx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/glrcgjbrc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gznkcrvis.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gthtjlyxw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/givplkbxo.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/goviktdeg.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gfhyaxuob.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/glodhmnil.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/glqmldaxb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gwuvdpjsk.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gmhuybbui.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gquhvggln.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gjrgpbmfj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gimikdbgh.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gxqqrgpxn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/ggevpydqf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gfogwcuwj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gcvitpkuo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gjsxmafwo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gcmnoygcd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gdxkropij.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gzmpnkvdr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gmvgdkuee.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gbadvdsoe.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gsiaswsgo.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gyhhiwizr.sHtML


<!-- 参考信息 -->