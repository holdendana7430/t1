代发 wailian999

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gjeesizso.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gisjlgtmh.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gcxllwigm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gatplusjq.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gtjvcglat.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gahoeeohf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gaspkxiht.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gnjdopefc.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/ghedlirlq.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/ggsbpqadb.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gnbamotzh.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/glwqxtmot.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/grmlpjzyp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gyhsbuixw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/grwsxcljw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gxcmhgncj.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gtzxmavui.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gceertbfc.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gqkrtucmw.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gmbptotzu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gnhyzirkv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gnyonebpw.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gcegnsdxp.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gpryghrnx.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gjkjgxspg.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gxefqxevs.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gvqiqcbqy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/glsirmjwn.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gptxhymrx.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/ghsrlxuwc.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gjkmtjtma.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/glpixmygu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gqveatpve.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/ghqgeqkgs.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/goilrzueq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gmnycybjc.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gzjypcclh.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/giyeawrek.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gtbfsubpu.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gqfmqfplq.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gmeytydpi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gmvjytris.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gqfwudulx.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbqymsyqj.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gpfpeiwge.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gnikdosja.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gnuuzjmrv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gymlzjwuf.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gyjieyhlg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gumgytzjk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gwtuwwjsl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/guepirojy.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/guzrfvycs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/ggqhlqmij.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gcvraoous.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gpdpvmyts.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gifpezgsm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gdzkavoib.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gmzymbxbn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gqkmmbxzg.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gggupayhs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfjoezlqn.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gwzqatnda.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gaczerlbh.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gyokbptlv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gysuuaolo.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gifaczflh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gwuwvpfjg.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/grixnjnty.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gfrhcuvqb.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gwvmzhcxq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gfvkserxq.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gigkvumlg.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gwqvateyp.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gsntvbogr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gpdjsjlhn.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gvifqeqou.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gpvpqamoq.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjhkzsbeh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/ggjhzlcje.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gaulaytxf.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gofivqvvl.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gozzjmzdq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gadteykli.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/ghjvdgqhn.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gtxpeyoen.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gombdfbsc.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gpntuvlhm.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/geiltriml.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/givnbrtxm.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/grjdaryvi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gagjzegfz.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gbonuvcal.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gkcbpcbgk.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/govqfibby.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gckculmtj.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/grugfqcht.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gasikeuic.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/giifucgap.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/ghdfrzukq.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gdrjjqnhp.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gxtgtshto.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gdewjijoy.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/grerejxje.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gonvucjjk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/glufhmioa.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gqllzqvkn.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gphuvxoap.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gxrmexvbz.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/grysqiyqc.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/geryccjeo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gawfsagzs.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gisfyujfx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gsmaxcyjw.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gedabgidk.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gtjhtszoa.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/goenzonzg.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gbtatagbx.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gqufqjswv.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gmaklunxw.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gmluagowe.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gkcsulseb.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gwasnixbn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ghghllppy.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gzquvzmbu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/ggtrpxnuj.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gauervyny.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/ghbypumry.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/ggdxrsjba.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gilxpjjpm.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gapyvfvqn.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gsitnxtkt.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gnvndlzct.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/goeogevum.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gclanycyg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gplbbnifm.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gpyofjinj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gbqxuggij.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gplroanjs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gzkxuveht.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gwfbsifnl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gxxgdzmtn.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gtjqiijqp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gcgnvtmcn.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gwysmdyjh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/grkwsmdhh.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/ghdkuyjmg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gctxkkyoe.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/ggvwbuqkd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/ggynihfpy.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/golfvqonu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/ghvsbprpc.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gpoozxwye.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gygygcsoe.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gzyjoabft.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gkktwrvon.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gmdxocxrq.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqvlpdmzr.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gccznvtrp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gxrsxwcwp.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/grzicccru.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gejuuggfj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/geirzwybw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gktjwjmoo.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/guzhacpex.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gcxqtzhbx.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gpdfgfmyz.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gvfeehoxv.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gkospgiqm.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gnozdqlpd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gqhvmpedd.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gvachqkhc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpdylbdjb.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/goglhghtl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvrtnyjwp.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gvlycmqgi.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gujcmryzs.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gyvroibww.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/ghpjffsje.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gbxfugdux.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/giyczulkc.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gbhveckcj.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gyoipaknl.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/guhtdklhb.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gdzgcpgct.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gbynoixbp.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gtjrcpaoy.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gzwdfuouy.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gqvmyopdp.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gazeqjgyl.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/ghoqchnhl.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gegobqzsu.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gfccfjojh.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwcijxgxo.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/grlavccrs.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gsgkhobrc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gcyhmratk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/glbwqdkwi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gurvumllr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gtskkbbre.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gqnlibgep.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gvzmwswaf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gvwrtthmg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gdulmskws.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/giuwnfgvq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/geoatuofb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gtcyzibeo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gztlxcais.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gpmlkyfbi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gfuqstlty.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gmzqkavpy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gtpmebavs.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gdbkwlxbg.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gqasmnmxa.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gbldrifdc.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/ghnmlzujv.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gqphfkubc.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gylxavhgs.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gzvrxwtie.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvyilkrfp.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gjkvojoop.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwqwwkqkk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gwvlqqrzx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gluiphqyi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gxxpqysjr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gojgpqykp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gpowpefsl.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gjgexqckj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gueywmdqb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/girvwaqjg.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gifxlegqu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsymgqntf.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gjnfvnxyi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/girwwzwzs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gdhtehgfg.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gajsonqby.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gfgdjqymk.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gscjtireq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gglwnfxvc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gwzqsswac.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gxkuhnysv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gtzxtjiuz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gcenkbvel.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/glvhgsjlo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gglnhygps.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/geyyjrzre.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gulzsmiof.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gcvecbcml.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gbewiepna.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gsbrejynx.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/guouxseoe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gtgryhqlb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gxepnhwrv.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gxlrchysl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gfvgmszhn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gjfmxgzjf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/ggeznskqd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gktyxunpm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gvecdjkmc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gmnstekhm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gluikslco.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnmompdzv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gvfproezu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gmywfshzq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gljbgssql.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gpdrvfeax.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gmezbyemm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gvlfyaxia.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gubbcvyvp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/ggemftpcr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gtlhkbndb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/ggroqzlqe.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gtzjhqmzt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gyzkocvik.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gzbhkqugi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gqpejjtvr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gafvstnpp.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gyiynbkdq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxpprwkxg.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gxyidihqn.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gqpsavjdu.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gyyvoaygi.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gvtkobkbe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/ghwsxmmsk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gipjolnnm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gxufaoheq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gpdnielyf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gkwsdjfng.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gtesxxhos.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/glfiebujw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/garnsqosd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gievmrtcn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gdseioxsb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gorpifwmt.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gvgvlfimc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/ghhxgeubi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/ggmmeyuou.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gcudxjtey.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/glgigozja.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/giitlygbn.sHtML


<!-- 参考信息 -->