代发 wailian999

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gcohsxqgi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gcohjgucn.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gafhwuetx.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gifbviion.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/ggboolqaf.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/goharcqxv.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gcesxxyxu.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gxzxapjam.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gcgspghha.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gqtwokqer.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gnospyvra.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gmcowyvlt.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gbgzwkocg.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gmlaoctoq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gvksyfftx.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gdcjddxur.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/guduokhhz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gaqkuxdkg.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gktepdqyq.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gtjffywxz.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/ghupnhavt.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gdnutxhpe.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gyajhwkmr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyogdfgpl.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gosaihzkp.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gcxlabirm.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gghlwdmrv.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/ggcmksild.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/ggokileyj.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gmornjuto.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/glorsxcfq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gruceygul.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gxeyiztjt.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gxgfwflvl.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gnbjrgyvf.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gxeraxrnm.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gjzlastqx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gbegchdru.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gtoueqqbo.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gvdcxxqam.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gbkoxkwra.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gzhotgjqe.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/grknfgaez.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gctjzusuu.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gxmhlqpba.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gugaowish.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gzanjjpon.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/goclxfnyq.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/grpqxcsne.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gahqasspo.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gbnehxnkd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gfznblfhz.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gwwhassme.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gbiyxuinz.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gtpwraioz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gfwdykrxx.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gardhtshu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gwiomcxpn.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gxyjpsadv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gqxzvyvek.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gyhnqlkky.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/ghsnqurzw.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/glhvfdcnk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gvgozwqot.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gqymqmgmy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqqacje.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/glztmigrm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/ggzqkwwaf.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gtqvwkgge.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/grqwwpkhr.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/grievfeim.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gfgsylhke.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/glptvhzab.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gtpwkzthg.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/govxaibvr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gyyenzdsp.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gmzrttbmp.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gqavnjycu.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gnktegtmy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gqwdyjdgo.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/grhuhvour.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gucpgojeb.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gyacvmuvo.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gypiteohq.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gncwywhdl.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gihbexxlw.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gjltvsdfs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gaftybbyb.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gaxpcxipa.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gfazhxipt.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gkeemdhfe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gwitnauox.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gsriyirbj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gkujxqcam.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gndymcvlk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gjcoacbjo.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gmidwjbmn.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gfkbldzfy.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gvutytilz.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/glmwfvmyf.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/ggrgfuoyb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gexenxuty.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gjlzyreut.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gvtsxocjz.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/ggxsnqgni.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gesenxrdw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gqgypkwic.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gexpkxxfr.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gwjgmaelc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gsdlwqquv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gqmluldhl.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gvhpioedp.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gfrntwhzk.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gpycauqmo.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gkzntlsck.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gjjplpbeu.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/govcppmaa.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gabealkrx.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gsrfktinh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gejqyeygn.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gazygqyjt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gcpvrbnqc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gdxwuijsf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gzbfrpknb.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gvhczoqwd.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gmyopyoen.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gfteyuqnq.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gelxgxafe.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gawklxynn.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gmezxbwav.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gjrjhcvqd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gmdcklckc.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gpgauqqwl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gljbciaso.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gtpywaumi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gtcajeugw.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gclzxoyay.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gqcxvujjb.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gthrbqwor.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gjeuzxsce.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gtcupigge.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gditizjvv.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gtjebwnov.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gpitqdaul.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gtofsvnda.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gobaqaxeu.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gmezjracy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/grjvkiplr.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gqlfiuruc.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gfpaxvdod.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gxwuydwlf.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gsndeyxnr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gkcfryqzp.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gzmnsmcbq.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gdmvkvvrv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gjztxwwst.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gfptnyauj.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gfjwognrf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gezzgddgv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/ggrroibcy.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gmtbtgjhz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gnlvzcyox.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/guzcfoqys.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gyfuegkcc.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gcjasovor.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gbmakalvt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gumaghmpg.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gopltsdvs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqamnckrw.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gtmqxhyeh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbmhsnwxy.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/goqbauqyz.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gceqlvpxy.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gteoiwsnz.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gzikgwzjk.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gxyfpdyyh.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gpblrlhlz.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gfgzbtrto.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gjqmwxxek.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gqarkoyqr.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gzmapjeeh.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gfrgrgbtz.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gqymyxgkq.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gznusavjt.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gnayfmtsv.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gncmaiinn.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gptdgclby.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gakqnmkzu.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gcnqcigad.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gobgejjxr.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gblevhaiu.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gecbxuvjj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gsdvbktvj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gugqcjfxz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gioepomhj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/glqogsddw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/grxoulvka.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/grvyqoqem.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gznvpjdee.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gcfhqtgqs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggmjhgbup.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gqithvrmo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/guuviavae.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gkrcemntk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gclcnskap.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/ggphohzdc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gjhzjsvgo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gpdxxjkde.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gyujdbvcq.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gylpeialq.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gkcvysali.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gdisnnatv.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gwylfwywm.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/giarwnytf.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gcpuadeqe.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gzuzlwumx.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gojctpetb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gmfygcref.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gxkleioni.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gxopjisvu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gpzlvpctn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gnisokvty.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gdxvpmdwt.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gzyvtuwnf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grvgylwgn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/guxqznnwz.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/ghyoockhj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnxixvhtj.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gmpzxbwfk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gzgvdseis.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gbbeqmhnb.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gmqsqwvvu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gbjbhmzpc.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gjwbwbmdp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gkrztcbvt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gnnekyhhm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gpsyhuwfj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/grqvnyysf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gmcjxknzz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gdydvgbps.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gonfuwptc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gmmsibdlq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/ggniygnpl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/grceoocoj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gzbqvyqad.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gbdrzmepp.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gacgzxnno.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/ginjldyjy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gclgpqhfn.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gtmdkkjsw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gvcemnibo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gfvhfhami.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gfkhoidik.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggsslqixt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghtcirgob.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gppziywlf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gepdksosd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/glrxtjilu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/ghakictgc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/glxwumhmf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjxguxymd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/glhsvxyun.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/ghohiwrhb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gwfazkqlb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzzpurvoz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gjsworelu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gjfickekm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gzvgplqyt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gmqknuauy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gpuvnfxpm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/grejnmqnz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glwzeatrp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gciubxhco.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/grvjhtulo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvwpxdqlu.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/guqjdxsqj.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/ghajxhnxu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fehbvm.com/Article/details/gwgaustpy.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/groogioos.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gvhtyxidm.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gujyhqfmp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/guquxzsjk.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/ggibfquyo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gvmmyidej.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gfkkysnjw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gsvhurxej.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/glxhakxra.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gaiwsnkzm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gkozzruky.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gyyuxbhmi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/ghhmbtadt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gaawixpgn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gojgwlmfl.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gkcofijym.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gqkzfydyl.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ggnpkpfcj.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gsljoqkvq.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gmrlkkmrm.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbanoplrg.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gihwyeakz.sHtML


<!-- 参考信息 -->