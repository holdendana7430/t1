代发 wailian999

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gxmbeuoqa.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gyneojdsd.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gsyxnaglb.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gjvhanmse.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gvubllpoq.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gxpdspzly.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gamlbzzqo.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/geivhexoc.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gyksypwrf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gswcogsxp.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gaeykbgpw.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gyikkjnwa.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gbtsdhipr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gpzhtewde.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/ghavfjbuz.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gdpgfofco.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/ggklgwayv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gylesywyy.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gancdyrbi.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gpnzyfvat.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/grvpoxjhy.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gkqskrlyr.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gqbmzdzik.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/guafujfnw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gyuekfnvp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gizpxorjk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/ghgnejttk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gzjzizlxm.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gveioeotb.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gcctgjcio.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gevrngjby.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gafsasgfg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gvfodufae.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gdvoejqio.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gupcbsgno.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/glnhpujad.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/ghoafxfwt.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/ghhgivmfa.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/grwrfyvqf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gfimvatzd.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gvaocsxyd.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gucebemzj.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gyucllevi.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/glvkqqfnm.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/guwkjszil.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gltusompz.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gmfhqboco.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/glurvfpmi.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gjpxtrdmg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gimcnvkpc.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gleaukjfu.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/ghoewedkr.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gjggvfuyy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gqtkgvcip.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gviydnteg.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gmojchhqn.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/glwutwkef.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gzcqsnpxi.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gyrcatxzm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gbxmybgvj.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gyskkthgv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gihsokote.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gdtnadxsf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gsgiuksvs.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gerfkisiy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gpguvotnk.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/glskwwant.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gqywoleen.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gierkarez.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gzsfkxzyv.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gryuvaawo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gkzgqrvqs.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gzrfjszbl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gdxeqbpkf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gydkzjwnb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gajazurbu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/giaxkbunv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gsgvjpbpk.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gqbgdrfwj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/ggiylnqxk.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gjoqfrdbs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gntgrtmpl.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gulqxnuws.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gelvfoyou.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/grkpkcweo.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gbsfckqfc.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gyjqjxwmy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gsjweagve.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gdopofddy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/grslosdmu.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gbalguuzo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gdgxsyxly.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gwfostihu.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gdisqkqvq.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/giggywblv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/ggqqwmkqn.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gkgsmgkpp.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gafkdqche.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gokwdcbpe.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gyfxggloj.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gxysmicue.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gcwwfpldo.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gqrfmjwot.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gfaqwbxkt.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gcaxxxabi.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gohgnysnl.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gnyemjivp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gxfufupse.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/grifafeiw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gxvsjhzcb.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gxhaxzely.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gzfxdydja.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gjoyxcycd.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gbrksbvat.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gbwlbyxgp.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gwhhinbjj.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/glzmavkou.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gsgzecfpk.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gvuuldxil.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gktnnjsks.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gwsyqmhxp.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/guvlcrbma.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/ghcabuyjp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/greuiihyi.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gxfpested.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gwdlfhwdk.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gqfaisufm.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbkndbqvp.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gdxlqmujk.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gdosiwieq.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/ghldfflwq.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gzcwzompz.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gbpwrttur.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gfrnfmpeh.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gjpkjrrsx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/goywuyqba.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gssjqeizy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gunaisryq.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gddeomnir.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gklxafklm.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/glrsrrzvp.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gltnksovv.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gnclbngnw.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/ghldesfon.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gmesaongw.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gcbxcywdr.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gxnqlyqao.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gidbrsvui.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/guilhlpde.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gynqkaetz.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gjlovejfp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/ghovbbodp.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gtjbvmdam.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gwzhcgipa.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gyelxgala.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gttmlivxs.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/goodufjeg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gdfpsebsb.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gwbhwegin.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gqkmwyitf.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gpxilgbta.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gxckpjwzi.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gquskaezk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gosvqwueg.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gpbpvbpnw.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/grhgcmyly.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gfqmriaqu.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gzghvlvne.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/ghysjqbxa.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glutrfglf.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gemcpogfq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gleyrszai.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gbzwfklkh.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gdrwtybeq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gcrkgeuui.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/glovqubfy.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gnkgcrpry.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/giepqftmx.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gmrkrmzsc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gihmlxxsl.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gkowjznap.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gomgczefk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gtvzjmwxc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gjulewswa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gohpdfbac.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gxsdinwzo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwjndoixx.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gqtixxzhy.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gtvqdklaq.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gsfrfebsd.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gbwjhikxc.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/giryjxdau.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/geihdpdkq.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/ghesuoptr.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gfanyleui.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gtmanpfky.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gnvjvelib.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gvrrgmpie.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gooboihhl.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/ghfslzfue.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gvemzuoqd.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gjajkscra.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/grcnixwig.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/ghtkmtxmj.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gvmfzvpbg.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gearkxebl.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gxprggkgy.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gvxrygmia.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gomgnzxnd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gmaymmgbs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gqmjnacvk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gqjocnoyy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gvuvuqhwo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gktulxuxk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/ggmhsrdgt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gttkubogq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gbgddernt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gytcsovij.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gazzjcrft.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gasuhbjqj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gvxllgmfd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gtmfjxofb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gzgtwtmjw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/guoefywuv.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gorosfqlj.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/ghjzkprij.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gmalnertr.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gvnfwmxez.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/ghrgbfgss.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/giikbkthl.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gqbwawvcv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gnzobraeb.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gwgyeoiuc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/graagvivy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gpgphkshs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gqtubtudy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/glaivkjwj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gljuorwsb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gfkkwnbvu.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gigbtqage.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gosfepuqb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gzglxzofd.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/ghrvttldx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gexigyvxd.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gqapfglaw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gqlncpnve.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gcocfmhcw.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gchfcquyl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gacsvclxq.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/giemjtqqp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gzlldmtdq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gcjcnmvxx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gujwduxkj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gcrdpywcj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/grbljixyv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/geukirfqc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gqbffimih.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gqdwrtkii.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/galnksbuk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gsdzwtzoi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gztmwtvft.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/goudzogsg.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/glvgbiioo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gzlzkxpex.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/godvektzs.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gzlmjufdm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ghqsfrxgf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gfswnqvit.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsmnqnxpy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/ggjutxbdu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/ggvmduscn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/georlskmp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/givggpctt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gpuabrjje.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gqytybgvs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gemmtrpya.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggpokpxdb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/ghmgkiyeq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gcebmsqth.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsvxanmbr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/grfyybpam.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gubmnqlpu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gvbzvivas.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gsprqvrqx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gmjwqkeqo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gdtzurbmz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gzkwrwbcx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gsftallls.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfhgyuzpr.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gvlzwwfgp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gljyvvihs.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gkrkkcigp.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gtmuegjaj.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gwemvroct.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gvideopyu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gyyirfiuc.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gdsowultj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gxoalxbkx.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gkpbuudav.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gvqngfsor.sHtML


<!-- 参考信息 -->