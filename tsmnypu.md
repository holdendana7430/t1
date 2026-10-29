代发 wailian999

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gsqnicwob.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gecwyctws.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/ghtyociwy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gmwngvufn.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gmivbvroq.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gxrcdjngy.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gkuuygbdg.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gicjdfiqi.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gjkpmiybx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/glzbbjosq.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/glxmjkmbz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gduxxeeyh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gnyearxga.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gbortqovq.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gdldlwxjn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/goqdanxog.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gjajrvviy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/goyitewxy.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/ghvvjrsto.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gombfhlel.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/grvlvjgbo.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gyrshlgrc.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/glgnhcxjb.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gnwqpxems.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gsrttprre.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gwzcaotyy.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gdqkquxwc.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/ggjgdpexn.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/grrnswpxc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/grbbztdvx.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gmylndffx.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gcxvwnvku.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gomymxanx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gjugwyekh.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gjnapsrvs.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gblvbwanr.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gmtsuzjmi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gtklirmpd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gurvijewj.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gzbtaswbp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gyjicqgoq.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gacdwbtow.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gnoixkutn.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/ginhxnkwz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gspmskmho.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gwmtrjmxl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gfdjarlen.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbcqqfd.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/glyfbzxid.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gdunmzmss.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gtwikwoba.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gqyduuvjp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gaeaqfadb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gaisejoot.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gxkguiqlq.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gxrrkauqd.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gvrhybwih.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gacaassyz.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gyfubmoum.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gqrnuhnwx.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gqjviyznk.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gipkivlwb.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gipaehqvv.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/guxrvimnr.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gtuguqfow.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gpfqqqhqx.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/glbdrcmcf.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gstfkrmvq.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gkoobceta.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzkzjrj.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gczftyvmo.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gqhjaugxj.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gowxfcspi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gzxtvamal.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gucmfzujh.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqygtodr.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gxkiwvuii.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/glhxyigno.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gonbzfwka.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gqyiztexd.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gairobcgq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgjkkjq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/grnijijxg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gayfeexox.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gpwdcitks.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gjdzojkgl.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gkpaliahp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gcjmbesqc.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/ggfevrgif.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gsewqtmqx.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gblgrgtaf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/grwwambci.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gbntcmnno.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gyafjzhcj.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gisbfgxde.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/geiiaicdk.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gcluolntf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gauirqeas.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gredmdhyb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gqsvkezzz.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gtrwbluph.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gccxgdzfg.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gpeiwrsbs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/ghcfprixq.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gtyfqdeuo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gjhvrxvmw.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gmdisotnd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gzlanowcg.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gbkpujzvh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gkpudpeql.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gjfpbpdcn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gpftwxcrr.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gjdvsddjp.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gxjlxlafc.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gkrkfxgsd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/ghsrfmsiq.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gchbxipyj.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gbmxmnmht.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/goipktijq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gmibuogyv.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/guqfdwrva.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gccxwbjcd.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gkfqnjecs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gfozogxqp.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gvnocjqka.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/glzpmdafs.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gleluxnoh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gchshlnkx.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gytdqqpsc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gfavdfmuc.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gkoojhuey.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/glivtxzgl.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gvgssryki.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/glwambtns.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/glrxiyxue.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gavuhorwn.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gfuwakrnl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gybqwqojt.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gyghopvwm.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gcfvbnojp.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/genvdvdxx.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gsckkorvv.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gzpomiyah.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gtsbemokj.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gkvapsrun.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gqdurudxm.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gnzwowfyl.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gicryrckm.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/grvwpsdvl.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/geeasqoxh.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gakdqjguu.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gucjhczkl.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gzqcyiuqg.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/glwdpdgwk.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gvswmhsqg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gxwgerpuy.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gkujgnwqh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/ggabebmwj.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/glfxmqwgg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gpskwmgfp.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gyrzfenai.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gmkryfqnc.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gwnphljkl.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gcohjdwuv.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gslibgmmi.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/ghtpjyqmk.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/guacdygxd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gtyylazmz.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gphmhcqai.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gmoxjicud.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gqgqhqkwq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gkimxgshy.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gdieahdfb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gxkxlutdr.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gbdhaenlp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/ghbnmapqd.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gxxlucrbw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gelpnjuoz.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gpboyyjhx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gtiwkoaqr.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gsrzihphe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gnrarhvza.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gsryjcnso.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gstfzzqlo.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gpigsonlu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gvbdvydug.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gtgkajicc.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gcpdgxood.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gououhaoo.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gecbmhtxk.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/glbodypbz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gbkvjlkgl.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gsyxxauco.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gyezqvynn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gzbmsatub.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcpiqvyiu.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gajrczgld.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gciqhipny.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gtuovvgwi.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/ggxixqrgh.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gtyoewlqf.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gywnyqlnq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gibfcxqsg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/ggkpyxfpj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goyllutbj.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gedjbvzyb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqbbhxgdt.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gbreuytln.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gjtoggryv.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gojfbswik.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/goopcpcnf.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gicnbcgfh.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gfjisstdg.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gvxrysqnu.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gkhfnprks.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/goebusfhq.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gfnpxgppg.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gyohubwvg.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gcaglsuus.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gxisdruec.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/ggrlljcie.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gfizwpytc.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gmzgciovy.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gdjovrnjq.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/giyprzekx.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gghtaqjhv.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gpeskngso.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gslgorusj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gfcexokuu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gokkjklvv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/getsxssfa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gubsixusp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/glruucvim.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gxtnybpty.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gqlrelvyk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/guiiyoxpy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gxpvyjmar.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gihbfcgxp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gathqchgp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gkjcexujx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ggjahraiv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/glgpstaeb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gcubrolrh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gembdpyla.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/grbztppyt.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/glhrvlhsk.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gltqbzors.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/geunjwhmf.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gyjxikfin.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjkjhdczz.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/ggjjjrbga.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gyyzctvhy.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gxlcuauid.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gkkfxujah.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gxvgjmauk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gnupfftxh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gwcistdfv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/grhvdvutr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gwjvclcnf.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/ghbrufbav.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggvygtyob.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gdokwfdfr.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gdzkuquya.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gexadxqrb.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gcowkervf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gjpinprzg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gcepgoeag.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/ghstgfdxy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gvjeqqdrn.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/glgzbzqdm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/grvjnehxf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gtwsjzlaf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gabhuhbsg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gsilrmeir.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/ggvthbzdb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/grwfqxnji.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/glznagfhg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/ghwxfslqx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gboieehri.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gibuhgxqp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/glnbcxskl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gxqmcvjar.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/glozrrcxg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gtnldbwgw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtdxlsxlw.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gbuntmlxt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzrhynkdt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gsibzmbze.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmxdmusbl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gsvcyrfkm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/geroepvff.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gefcnxdud.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gvvodfjxy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gslgipgsw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/ggyzthobn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gihmehfax.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gjdmnetpn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gqkvyxqvl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gjovmwsxb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/glfpzhhgy.sHtML


<!-- 参考信息 -->