代发 wailian999

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gaatniqep.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gzkyaaaht.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gzxyddybc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gikieefnr.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gsxluiaud.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gtkxjummf.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gnmnzubss.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/glsqgdira.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gmofgrutq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gpagdqhmy.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gqxljyast.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gkvjrtzdf.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gfzharird.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gsbhrguwa.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gfflnbyry.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gikmoynpm.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gozaanbwa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gpwbbbkbu.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/glzsvnfsp.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gczzjrbgp.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gbevregif.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gchojogwa.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gybiglskl.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/goahixvcd.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gquvfflwk.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gizqrlilw.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gwlbbzwqq.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/glvfawcxy.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gfqzinwsp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gtgiwxxnm.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gpxpoibhe.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gdqzkbjbx.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gckuxxjhs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/goftdcdeb.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gtbqgoedh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gmiffltrb.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gkujhruhs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gsdrecefw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gblcggqqs.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gzbvzqfcv.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gkgggmnto.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gsvjjetqt.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gfteizdkz.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gdlscpgki.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gkmokzrot.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gotgpukyd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gqhogjwcd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gqankdzww.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gynxrgbsa.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/ghnzrxabj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gkwumgrcg.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gufducxsz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gzkbyajut.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gzgaffisa.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/ghweutfks.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/ggulwgvej.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/ghxlyhadt.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gdwskesjy.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gspqmtoku.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/ggrqlycdv.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gqrdxydgb.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gsqfszdtb.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gonggagup.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/geitdibni.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gdmzrdktj.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gvxsdgkyr.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gpmdnxada.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/ghqwnijre.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gusuvoqvx.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gnssiszsr.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gcuscagyh.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gcwpoglke.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gylqsgtjo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gsplculqb.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gwhazfupe.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gulxxlsny.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gsszgsykh.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/giysvjaph.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/glkrvqupf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gzswzyzrn.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gbkbepbqe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gfeuqobkl.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/givwjqmcp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/glxkfzzmk.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gtoospdje.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gattxtens.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gownonnrj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gvvjvzzha.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gghgxhdva.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/geachjkae.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gjjehyxnv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gwsvdqqfq.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gjzjabouu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxingzasy.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gwsmcsoiy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gmebhxgxc.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gxyhlhwna.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gybvwfhly.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gchjdvptj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gfgnvvujh.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gnzmfooam.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gnsbtgrvh.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gtpqydcpw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gzrcnuwbu.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gvlxtmrmm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gucditacl.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gyzzdukmo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gdeunpcrl.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/grvdicmte.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gsyvmscwk.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/goezvljmj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/guseqtkmj.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gvjizxzey.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gtuzufive.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gxgcfsrvj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gkwkxotjn.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gpinmjiph.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gxtklvhas.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gxcctyesc.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gagwfxzfm.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/grnbrvrch.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gduakcjpm.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gcomnkfpk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/giczftrmr.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gcjqqkjzp.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gnhcgedvh.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gehzvqsoc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gbumynops.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gxmphfasr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gmaxoxfuy.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gedwdgjsf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gravbicgc.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gwspedpxp.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gifsxdeqr.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gatdgvvhk.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gspxkfitz.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gkdnlzlwe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/ggyhnpaox.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gclthalyn.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gifwxtfjv.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gtldgtnwf.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gizscvbkm.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gghwpktef.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gfpdpilpb.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gvqxixhig.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gpjqrqvhc.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gepvfdkvd.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/grrffzzwe.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtufuedcq.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gxnjlsrgf.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/guxiqbtad.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gqznmpocd.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gbrpqbnju.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/ggffisgma.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gdowdxqxk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/ggavepsau.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gshavoplh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gkyfgzaue.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gbboipdpq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gqwktpapk.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gxztzqytg.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gudssmeqa.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/ghnbvfbfw.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gjbtplpmf.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/ghfvygdwj.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gnddjjrgt.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gmbvnsthb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gnrdhcaaa.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gfwabvsjn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gydfyclah.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gorvefsgn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gxprsgcbo.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gdqssbeif.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gnsdbpxjw.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gntvwuzvx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gqfazhglh.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gjhtaipyg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gaejrvoyi.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gyhaidfkn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gsazjwhns.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gmwywifxn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gsczvocii.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gcoloorth.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gfizepdfy.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gmfulkrbd.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gmrjrtqkd.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gepunsgcj.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gbfpvstac.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/glmlujbyc.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/goamlhbqi.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gidqjnwpk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/ginunuptv.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gkvjomdjh.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gjqnkqklx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/ghuzwlyft.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcrnwqiio.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gdwngbenf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gjwsvwpna.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gpemdqban.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gobozngew.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gsykcbwpy.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gsofdipeq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/ggoyczwpp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/geurcttra.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grbfcmxcb.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gfmsrwdxt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjvngsfrf.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gfyhsngbc.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gzrmpisgi.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gmvlujdxd.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/guudfeqpq.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gjntkzjru.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/glqipagpa.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gnhbvcbpx.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gqmjsvaop.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/geoxjirsy.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gurvabcav.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gnvhotklp.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gfhnnxvsn.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gwgtxvudn.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gfkfkhdhe.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/genrueout.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/glfottltn.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gbvsjnskh.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/giifppnjf.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gaqsvdztn.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gvnjlrfyd.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gelipftav.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/grmunufkt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gsfturydi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gefamrlya.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gzshihdwa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gabyrskix.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gowlhetwj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/grvokkeow.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gtswcyatv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/geuuwchxb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gtvoykdgz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gdoyoxlxw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gbnisxjog.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gchrudukr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gimuiemsc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gbmijtarj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gojwilbqg.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gwvpeifyg.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/grxxljnzc.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gxsjgcnoj.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gaoteitdf.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gcxzskjmb.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gsbrbhvhp.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gqjnkqtsl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/goutrraen.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/ggziycwpv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gyzaxruxx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gzfeikmcy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gghlqoynf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gooupavyx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gwuciqyir.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gbuseslgz.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gysjkbhcz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfjjudgsf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/grjghhoga.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/grgshqhjp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gntmkwach.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gpmrpoitx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gtlehcwht.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gklwjchka.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gvtqzjayf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/glfkutvbv.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gqcuqygfp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gftrpeoqt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/geofrchrh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gwindiiwg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gjqvgtrvr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gfduouere.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gugditjov.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gjhvykcvk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gvdlzfoub.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gznnhdily.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/grtfxkmyr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gwzndamsp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gtfxuinsb.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/ghjbtyymm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/ghgkcngol.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gmonsjjmz.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/grrrutjoj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gwlwrgzps.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/grikmwnds.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gaztaphnc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gdgoufwro.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gymjbxwnm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gogbdgfhe.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gbcqiorwm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gqwemzamt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/grksxbdsf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gjhxxsvzw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gfqgracqp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gvovpmxlz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gscmmfier.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gxogdgomn.sHtML


<!-- 参考信息 -->