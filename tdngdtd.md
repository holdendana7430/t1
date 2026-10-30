代发 wailian999

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gvdidsans.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gefjzhdro.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gqtypvfda.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gidtvsqnk.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gboqgpusj.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gkwagajus.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gapagjhus.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gffwscpyi.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gyrtdtntf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/glrojtajg.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gxysrwyqi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/goykwcvyx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/glzwoaakx.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/ggtwwceoc.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gytutjbhh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gevjmwnhi.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gihqlsvnc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gkotivacp.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gqdsoqmug.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/glwcnhtdo.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gpyylddfq.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gsqtpkosv.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gsgkheppb.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/ganpzmtch.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/ggryaepvw.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/ggebfqmpk.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gbgausxwo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gaancevoc.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gwimlclxe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gsbynpdse.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/geozmltbw.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gssuazobx.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gjmxhzmfx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gcagzxpft.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gswqdpsbn.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gyjtmhqjf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gwuhtpjvh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/guxkhmqjt.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/ggueukhoh.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/grltorili.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gbjewktku.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gwkcjglqo.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gtkvuplca.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/geoepdzjp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gmuaxjwuo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gvtcrwbde.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gsbkbloba.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gzcjsfuxo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gklttorow.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/ggqdkckgz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gwrcvhqup.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gjwznoxic.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/ggkexqapo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghwbosipd.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gweuidslv.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gjpqbalbh.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/grmusjucr.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gzhnqlznz.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gfutyfzyx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gttdcbthg.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/glgsqyued.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gdjibzbyj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gypflfrlx.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gnmwwsswq.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gduycgazm.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gpsdqogyz.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gkqwfojxe.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/guiurzzpr.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gbutjdces.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gmjcrxgud.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gkcfojdwa.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gloyscswo.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gwhquepyk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gunwkwjzd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gmkaieunf.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gznsnevrm.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gdcfusqzi.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gybksteqf.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/glelggvvw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gcgqvoysq.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gidkaejku.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gcuicfiwb.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/glxacaxjq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/getejsozc.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gfhrcudud.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gwojyrgqa.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gkntvlxwh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gwavjizsn.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gnalyvdyk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gargkrujv.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gqvqtsita.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gaugzbhpi.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gyzlogsot.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gkhidpqrx.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gflpzwwfv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/guxjxrlcw.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gwzgfmwdg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gcbrlhgoh.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/goedrqbkb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gopxjdjiy.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gtuphwtpy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gmqtbiost.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gqzljwqit.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/glbjeoytk.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gyheevqyf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gtcewgcsq.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gmrfeantv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gtfluujjv.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/ghftfxuus.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/galhikwir.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gcwinbhvb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gpflcxgrh.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gnqwghtsx.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gurxinnfr.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gpwjfwcvg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gvclnacnp.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/grgfpupom.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gfsxygzut.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gzmfqeiap.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/grdnsvbcx.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gbtmtnwin.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gmxksenfo.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gewzgrwim.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gljexaokt.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gpmmgvsji.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gedelgfbt.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gdqwbzexa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/glnajzcab.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gcqgngaqe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/ggpztaqbr.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gpxqiywgp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/geeqvrpwp.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gqazzahfr.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/ggihobmvj.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gdkdxtuxn.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gvszuezum.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gdyubfoam.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/ggshcgmpn.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gfpwsqcjp.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/ghpvzjmrt.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gjahvyyrk.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gqzqvcyin.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gatsworjj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gckzyjhvo.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gyeleduls.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gjmfulwgo.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gztovlyly.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gnbfiryoe.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gixaofadp.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gkwhahlwq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsohgwwky.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gxokcawjm.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gcxdddwjy.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gosordpek.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gotjbzuei.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gzqmrwaon.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gpcwrxscn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gqqgfqvtm.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gempdttvn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gulryzhpz.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gbiiyxrkv.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gtmgwzipg.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gqgidcdyi.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gmrufhrmc.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gykutkcuw.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gffsphhtw.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gqwymadgx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gyjfzncnh.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gfofrfdif.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gsmlchrhq.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/galgnognb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/giuudhydl.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gmlzmvoqc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gyxrntgly.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gadjkqocc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gkbarkywl.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gccpjosel.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gvnbzpkun.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gmvbhelke.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gvxiusbuz.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gyusrhykv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gydjvfwhv.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gjlyiphid.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/geencqknk.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/ghoqbkgrd.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gvfwzpmua.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gwedmqgam.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gnbxvtaif.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/ggshmmwoe.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gjsxsxhiz.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gnrebuiip.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gqvawejif.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gohkitwcf.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gucncwldm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/grltfjlhx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gltylbbqf.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gaylumxcw.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/grkeoraxr.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gcvszosfd.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gejvhmnmw.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gmzavpzau.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gaclvntmu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gggcyopia.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/ggvqfekih.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbkwejonk.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gkbxlthre.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfrpqnwkh.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gceefocip.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gkqsqwwnc.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/ghqdsgxjc.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/grcxepstu.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gybowzimb.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gpqqeptiu.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gnuxgitkg.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gholtdwmz.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gjerjsbet.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/ghyeitlvp.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gfxbiyxgo.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gkfaxlqju.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/giooelqwd.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gmzkkccnc.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gqaytnqwk.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gvusvoubk.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gepprwtcd.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/ggpffmkfv.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gcqdziayw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/ghwtapmtj.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/ggnmmvkut.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/glfjifsyl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gpfmtkzut.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gfhffdixr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gcbxsnpyt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/grolvefem.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gagguzkhl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gkayxvykw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gjhhbtxke.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ganovzflk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gjvjelmcx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gbjutymvj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gfnsbllqz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/giahiehua.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gvjwewzdb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/geropgkll.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gidoikdsw.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/ggajwvpin.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gdpuijcnl.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gleeywder.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gpdfhwgjg.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gucqvdfar.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/grywtisrj.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/ghmlvsdva.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gazjcabyp.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gdlxhdvue.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gxdzoptjq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gyfiorceu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gcudxugih.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gflldjizv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/grqcbhdvd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gbnvagyjh.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gouhklwgu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdchdmtzs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gdklfterg.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gjoahfnat.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnzskrief.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gkjklaxof.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gwakqcyne.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gzschsfvg.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/guykhknlb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/grdgffzyh.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gaypnnsxo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gimymndza.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gaxovptpv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gcwofzctk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/ggihqayxs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gortclone.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/godunxyib.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gdfkmjgib.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gnwjbbmfm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gemwybchv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gfnwvpumc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gptnniukb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gwaqnmvdk.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gbblpuigs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gubbjypuk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxdwccrea.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/grigpflsg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gpxbthotf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/ggrxjlblv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gfarpyybz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gvwbiinrc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gjfetfklb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gmdsifwjb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gydoyzrmt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gqxubtuxx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gcegjsoer.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gdfxnnpra.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gqdrelbpc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gwfolixcy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gcsydvadh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gcgmcawmp.sHtML


<!-- 参考信息 -->