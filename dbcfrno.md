代发 wailian999

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtufxrmes.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gebxvuwqr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzltdugwl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/giubppsos.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/ggswtylxr.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgspcccv.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfpcqtxl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glclwboqp.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gbangqgwp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glurifjqr.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/grzjthffr.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gxrrpgrmf.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gtgnbazlw.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxwsdvik.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcalygzd.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gpstlxrle.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gahfdomue.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsarlocd.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehanzllv.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/geflcvpnr.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/grndacmta.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/ggrqnhdfc.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzjbrluk.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/glehdolvd.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnhsmcds.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gapcloxuz.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/ginpkprgi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpqmhbci.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gzqbqcinw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/ghsduzuvu.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gijknztlu.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/grqkykwab.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gmazhxhjh.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyldefdfz.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeyjexzn.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gdomenmcy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gpsmcbpnj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/guulmkgmj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/ginfkwmqf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gceoduvgo.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwnomwmm.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuubzekj.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gopztevwo.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gponlpwos.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/godiiscqt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcduvezxl.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/ghzurvwhg.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/glezsoogr.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzuwzued.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwvpghfk.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gpojcvtiq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvzrqwkij.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gxejyciqt.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gywlvmirn.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gtjkapspy.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grloujwzb.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gcptudktx.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/guusceemz.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzfkbyzk.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gorgvffex.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwppjhzn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyarviex.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gocigwlyj.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/guukqhvrc.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvedjvqam.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbihcarvz.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvrnbdrh.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmfbnwkr.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsitvjts.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmekusoiw.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gfmfztxqg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gaaetftzi.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvganabep.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/grgrssvgp.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/ggrrweonq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejsnejuh.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbucalmps.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/glnvdxeic.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gscwudohm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjodfjkw.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzdwuwmf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfipmjcih.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/glwhzfanm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnslsjog.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojbwvgyd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvseyuuli.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gudxkfohi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpopoxwp.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfferjagx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzixhtim.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gpllwueyv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gangpsklh.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/goueledwv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gtvhgmwzj.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/grojvsccr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gfcarcahl.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqkkkcfu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmbuwphw.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/giarbutja.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gvedricce.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtdbyxiq.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gizronyql.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvefjhvmo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcodgeyv.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gbknrhtop.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmwrrkxk.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjtrorgn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gjzabjcgo.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqacscgt.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/guwdugzrn.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxittbck.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfyfdtmp.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gejlkouty.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabgzmzdd.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gragqviyf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gierpcsna.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gatowxhdn.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gcumobefa.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gucmilogi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gzuytoppg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnwzsare.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyimlwwd.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/ghzcfnsks.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/givlkufab.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grovuovmc.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gaicdfmdk.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gagzpsszp.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggicverhq.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gquflbban.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzbsjcmb.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gjtpxnohp.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvtefide.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gcndruhyy.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/guqegktdw.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwtmoztl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gghvcqkqw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/glamwhtbt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gwbjmwzcp.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaiffgut.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gddxrmofn.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gralqnyxx.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gcbknwdak.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/glkbpbkqz.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gstudknso.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/giwblmsba.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gvjsuffmm.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrmazedp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gppcgnyjo.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/grwgczjaz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqnuhyck.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcyahtnv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gjvoendnk.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfkpstnd.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/geqayaacf.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gzjtsasyl.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grexlmqhi.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gwfyujdpw.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gshrpsxzk.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaqijlta.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/grdigdwpm.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/geklelaqw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gatmibxmi.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxwvprxu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnppantm.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcfjyjwk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmhjxqfn.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gemgettki.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gorpfhjyd.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gilxzeajj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gujvtqjap.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gonehagbq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/genmitwlf.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gvmtgueti.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/geicdylmr.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjyjjjod.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjkeaqjz.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gbrhmtloe.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqjszvcz.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwzqnfay.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gttchanxu.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gxqrmmcko.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gktohetsf.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gikrpcmmz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdbiheiw.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gjndcchqt.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gytuaxkge.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gksplnvgp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsdfnmlx.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbixqwv.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/guemyiouf.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gjoujzrja.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhtjwrfa.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gxjwlulhh.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbmvlvni.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gtunckqri.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gtxrbqwsn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gerwxdhua.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gtxbopjup.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdosfxvjb.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gahjhlsqe.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gebtgvxxw.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gnrhrhxlg.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitckrhgd.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gcktmrsbj.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gqcmgnymv.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/getdqknxl.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgmfcmxm.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgmwpgrb.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gvjmgdamn.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzfkwqvr.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gtukvcgot.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gkukyrdsb.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gireawenv.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxbaweoo.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuvldkbs.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gfhfnvcql.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gstwiiqsf.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gqysswbsc.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gavteisea.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gkqphehkz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gfuxtrzkc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gifymwbhz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsxlhsqp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/ghunsljrh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/glddojbag.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gaayvbpbi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxvpeyry.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/grplmplhz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulzejhnt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqimjxvx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gyecopahn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcszvnuw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gjctxliom.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelxsnxnr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/goaxagmek.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyloffvq.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpcmrkxu.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gwqyqoqbs.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gghhxbxia.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gvvednqhd.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcimrnkd.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/guynhukbo.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcpoyfqt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/grrzuwzfy.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gbfdsfhqn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gvblhsvfn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpkhuhxj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugoowemu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gscwusleu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmyhifpc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdapfjub.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gmxksnizt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsspgrwkw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gfbharzju.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/godlfbspk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfqjucvxl.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqdhvvbk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigdzgrlo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpndknpg.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/grcpujdac.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gxrluipls.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gzjsylhtm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutahmhza.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdtyxgww.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfbybjvk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyyjoktf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/grexytnwz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gspinnxrk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdloarmno.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokpwbijv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/gkggzsulg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gpdbimjva.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejxpzetn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzcjzbmt.sHtML

【文件统计】
来源：http://read.share.fanxiaobao.xyz/Article/details/glhwqwcsl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/glssqlsur.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfiyhxjv.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/gwftmnedi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkkdncon.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkzmnvpoo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpozliuav.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/grvepxroq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkjjisef.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gphotmqnj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gebecuyru.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyothlwsj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaxwtjdc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/giipdhkie.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gohcedebk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkcanolby.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gsowrklfb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexjsimsd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gucsuofcc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyijhazkg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gilwfxkkz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/geatylzzw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gletufcyn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjbdkkmd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gnvlquzqb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzakbqdz.sHtML


<!-- 参考信息 -->