代发 wailian999

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gbvyvsild.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/ggelafbqp.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gmdqgocxf.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gczyjmxjh.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/ghigeytvb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gvmmeknpl.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/grigxdajx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gthlndzyp.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gookiiiww.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/ggzconvrz.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gtgarhvld.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gbojlnobn.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gfxonyrbc.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gqcbtqyrr.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/govzpusbz.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gbxcrlghm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gbgutzfcm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gxqcoawzm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gjayrvcli.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxudzqzr.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gjenidnxy.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gsdltlnji.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gowdzzhkv.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/glubevamx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gwvandppb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gfqxgwnex.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkvxmkgqo.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gaxdbsczl.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/grwmkfsug.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gzvhzjhoo.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gbzhksfpb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gvtwtmfut.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/grkdffwgh.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/goexbqrmy.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/ggecshdgi.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gwzqlanim.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gvbzudpsd.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/grrofihju.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gejwczbfl.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gpgvednze.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gvwijevdj.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gyesohkmm.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gtidhmosq.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gvyllijzw.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/guynfmdad.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gipuhytnf.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gycbhtrgv.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gtamppnev.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gamfcmjsk.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gjfhprbhc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gzqiydkmg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gfoynqmyg.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gucpdpwho.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/glptekilf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gljwlicge.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gcklcowtg.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/ggqndvwzr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gwlobrexz.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gkwasbslz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gckalqamv.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gtjwdmvoq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/ghjqxgbbn.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/grcriofsa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gxwjrlcnj.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gpwanmbbn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gliytesbr.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/guwwjiemy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/guwzbmhol.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gelrxqzia.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gmuarcwyy.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gupxwyibp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gcsplexep.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gdenhzqyj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gmmgpwsqr.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/galnsscmt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/ggaxmktww.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/guqesyhtp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gxpscoubx.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/glagvofqa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gqkxrnqdb.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gaqqlknfn.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gqiwezdtm.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gvskntkib.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gnhanyhxn.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gbefuggip.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gaubxltic.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gnosdnjdf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/glwcquewr.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gpvliqrwp.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gcmxyohez.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gcdukgdrx.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gagdkswry.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/ggonzbvio.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gewweekqk.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gnhehacfi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/galufsmmy.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/ghmosijpg.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gpyniylzf.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gmulffuyf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gycslzgvi.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gjwluvhsi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gsszvlygy.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gqsbvufrx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gjtmcplmw.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/ghosvdjcn.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gyncaoscz.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gnhdcctdl.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gmllxoiuj.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/ghsamvscc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gpzqthygl.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gxcgomrdt.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gwlpbdsqi.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gkhrhlozb.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gupookete.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gglxiuesg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gpljzkkan.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gtuqucgcv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gxwsiwtfu.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gldsyjeqt.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gokaaemkq.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gcqgrgjey.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gftnnywaz.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gsfgpxsup.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gusjuuhha.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gbcimhlbs.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gjbicwycx.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gcpywcddq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gvkwrupkd.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gvaugvcnq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gigpnyodl.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gqphomppc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gkhdpkxjc.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gpegszipj.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gzyjpaoqh.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gcwzqzmtq.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/getoenpvo.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gaaavssfy.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gwrzkpbsm.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gmjtsjcdl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gkqwtlywm.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gteocnfwo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gtywtgfcv.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/ghnsvhons.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gyppqufjx.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gjekwvlnf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gpgkruzsi.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gbiubqffn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/ggrvatofi.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/ggqdzwfzs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gmuqldcak.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gkeyqpahh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gksvnpfig.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gfivqqskr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/grhbtycjt.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gkreolofr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gatddubmb.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gzdscgonk.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gnjzchbis.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gfkpzrepv.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/glbwtmrhw.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gxzxtjboq.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwuxsvuy.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gsnyohyzi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gxpasfdbx.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gnggapopb.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/guuhdrnmo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gfnjtdqxx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gvewmyovo.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gpqraapmb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gnambpxbq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gedvnakyk.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gwcsuplao.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/geuldehgc.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gemlthyfl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gqheavnpg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gmgfpzapj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkzggiyrs.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gbdjxvsxc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghwvfjaco.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gfafkdjde.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gmdoghhar.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/guqmorekd.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gququwrvw.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gbzzpzvyv.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/ghflcbbhf.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gbbricabk.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gznlmlxbb.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/grcddezvo.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/guiinsqoy.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gizqrispp.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gjcdsdgwq.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/geivalqrn.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/ghmmcjohe.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gfmxrhglz.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gppwfhwum.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gqckakhwo.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gcjrsmswb.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gmmihlwhw.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/giloilspu.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gguzfncyj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gniavwqar.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gkgypwvae.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gcrzoutow.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gulhcqgoy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gfiwfghyk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gflrrpjow.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gbnasraoh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gzeinwpir.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gmvprfbsv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gwcaowqjc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/glgicaqbt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ghpfzlzsx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gnpsecgno.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/ghtjxtqyr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gpyfcokze.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/giztanasu.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gitvqwsue.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gsmjbsiar.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gsgszsfuv.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gnikboxqa.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/grdixdtmo.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gkpgkmdea.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gxmmsukpj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gxgrwwruq.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gxfptcrel.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gclloqiri.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gxnluccpq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gbgksztdp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/ghabfqbnp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/ghrnqjziu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gdgriiaae.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gokbfazqs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glpnvcmyl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gkqszqojt.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gynoztyxi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzrqqvclt.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gorwikfgr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gvofivmwx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/glrqitmte.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gpjqspeil.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gavtxqzmu.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gqewnmyrz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/glglgivyi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/guokmgqdp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gpfdludec.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gvczrcnae.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gfhlibvxq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gcsfnfziv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gteveaaxh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gjizrezhy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/ghuwnosxv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gkbixttmr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gcubzsmmo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gqavurctf.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gqlrqddqi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gstednflb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gsztyeiki.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gxivektkh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gkeltyhnu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gigjsjlqa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/galnwzhuy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gdktxxuoc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gszzltpbt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gxsewwhtu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/glvmgieqi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gksyjpjlc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/goahwmdfv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gdpslaxtx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggrfgeggi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/ggubkgtln.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/goqbbcwuu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gerjaaptf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gxneqiggf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwhpjyuwz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gssbwpoaq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/ghinmyptv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gukswkgwu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gfwafeoeu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/goelbnfrf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/guarayifd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdxjvdmjn.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gwlzlpytl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gurqzdeic.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbdfhfgke.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gpmvebuyk.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/ghsihkqhh.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/ggtuqumhq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gacaonzla.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gtueljuyg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gndwozcfs.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gtsmpeqvq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gqagiqiuq.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwpfcgh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gtdikpyqw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gpysxbphr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/giigbyypx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/garzglhix.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/guxgfppnt.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/grsgstnhx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gsijrkvpo.sHtML


<!-- 参考信息 -->