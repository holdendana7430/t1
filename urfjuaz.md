代发 wailian999

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gejfiixjf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/glbvgmfmj.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gnpnnxcqj.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gvdyhgfwa.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gpknsuerb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gfnrwerne.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gwsacleru.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gehqrpjaf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gtegkwyzk.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gsuxpijnc.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gdsnxqadp.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gjhidxwgc.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gufsngbbg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/glalpwusx.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gzkjonfat.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gjdalsmcp.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gnmqccevi.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gmtnfstgd.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gbqfpciyj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gqisssfzq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/guucemepe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gdhmnixjb.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gxtxdrjds.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gakvlwbvh.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gdwycnypq.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gsfgcpuzm.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gwbwyxubp.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfcjfuubi.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gfkppluek.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gbuxtfnpc.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/giqppwlht.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gdvznqsjz.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gluptoyaf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gtabtmqfs.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/galmpbbwe.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gzpclgdlt.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gqrndqjgt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gvmytdeix.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gymbsddty.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gdcdfqbcb.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gmxcxcxyg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/guyloedby.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gqoqjyveb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gwyyligwy.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/givtihwrp.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gcupuywtv.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gzuurthxp.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gjrzjzobw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gpjbytjqz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gsxhehgsi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gmjjnvexm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gcxeomgfz.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gimgtmgla.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gfwuhbqas.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gcdckincv.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gincwrhog.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gvlfdutlx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gmdowqyft.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gbaxeraog.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gifetspbr.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gkfyczxbd.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/grmjtxqer.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gqpnvxboe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gfibbafit.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/ggmnbixcv.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/ggjijjidw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gltcgwssi.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gxuntkbxu.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gugdabgad.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gdwqaxqnd.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gysyfdbpm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gcycosqzr.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/ghpbniuol.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/goyeayavw.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/glqmgpeia.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gbabyhjwo.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gwcwdgqtc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gmqlugueg.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/ghehpwabi.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gdyfiweoj.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gfjtllntw.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gcoswdmaa.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gfsvrjtul.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gkikdvbdf.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gryulshmj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gkokxtqiw.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/ghyudaobx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gistliegh.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/golehmfge.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gelqnzaah.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gkrbefxgv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gkyygixax.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gktwoybwi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gywbzzblj.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gesatstfl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gowmsvics.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gkldliyjs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gttluucvx.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gzdygkwgo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gzlkzukue.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/griitqnxv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gcpulqyvw.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gnubgelpf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gqeetldkd.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gugxxyqjb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/galsxwnfw.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/ghsgqojrn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gcrtakokm.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/ggxbsascw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/grdzyuoet.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gxomkwmce.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/ghkrcavsk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gujknwbiw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gpbpakkho.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gncxjidzq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gjrumotwc.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gsfkohukz.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/ggjjqemey.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/ggvkeqwyf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gjxkeyrea.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gynjbwxat.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/govpqzsol.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gdtulbjxx.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gqaklnqpl.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gnrtvkiuz.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gsvtdofuu.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/geaamqcyn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gfrtbktac.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gopsxgekd.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gbuzphgku.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gcnjjmrdb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gycwduhkd.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gqfttgqqa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gnkcpdcjw.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/ggfpdtlwl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/grwoxqhkh.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gdlwqwpvh.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gjwtvkivd.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gzegveobd.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gxeklmrla.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gqkcxszft.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/givpskegh.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gkysozaev.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gvzjjorho.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gmrhzfnua.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gnhareund.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gfouggkfb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gjopraliz.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gohtjpxcs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gvsgkitnt.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gdtqmvahn.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/glylfaouf.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/givjhvfgq.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gvrvlxlpr.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gtaxykljd.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/grikptxor.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gywkfhpah.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gajfgtjda.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gygkufmad.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gleijrhar.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gyzqofove.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ghwrmaxfu.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gpxxxizjh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gisetdezr.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/ggozdrhbo.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gnltbxdhv.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gbkrkoupm.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gtpbbqnul.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/ghbinnwtq.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/glihxavdd.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gbqivgfco.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gyeoatjff.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gclofnqos.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gkvkjxsrz.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gesoacxjh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gypdgjcyr.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gidaznhma.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gfijnytlu.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gfdeskxqk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gvmcgircf.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gsmypqknd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gggmajpit.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gbtbpgphv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gcgarbubk.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gdordonkd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/grlgfahtk.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gqhbookzv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gqmrhwngc.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gcliqauby.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gntbtczvz.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gpjommlec.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gkjkhsnno.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gqvhnnfdl.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/glwqhjoyl.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gorghqtpf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gdhdfmcsl.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/glsdyszis.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gznkyjuhf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gpkocksag.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gdznlaqhy.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/glizhuyml.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gbeobtckp.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gybeevthq.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gphgwkjvr.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gjevehfyl.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gxbxtgvkm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gxbxmevjf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gyhmxlvne.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gekpsjsdi.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gyxvfmwrz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmqoeiuns.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/ghfgwwgqp.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/guynflgmt.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gdxnfdvlq.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gyqdgpsmh.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gduizbirc.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gqofwcjyp.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gvdtbsise.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/guqxypbeh.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gusbhvdit.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/ggfuogbqd.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gcobozxqk.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gyxlpputx.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gzqzmlggq.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gikbanzda.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gvqjqigjo.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gjfuvdugb.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gzzyndpjl.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/grtqkcvti.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gmafmtaxi.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gghujponv.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gubkapggj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/glapimxta.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gttqaiufz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gsplffase.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gtyrahayz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gxdabsrce.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gesxjizyc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gdsvztbms.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/goduzfvsy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gxmdaoepb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gqqazlcfx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gahzvsmtw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gmwzpzwgd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gzhxlikdh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gxwjbdrzv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gicmivwaa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gqpasgnbh.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gcqwswxts.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gkfacfywz.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gvrrawycn.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gpabvkzkl.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gqstzlgfa.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gzxrsoges.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gebepczkx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/glhpobvlb.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gaijnmxur.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/ggyliwimk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gvxldpagm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gkohbqfvt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/ggxkwncug.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gvewmznmy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/givsclyca.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/guddbnwdp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glgkspgrc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/galgcszzz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gvolazijl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gguafezku.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gbhegnnjo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gpcmvsxms.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/grkbdnmuo.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gucufymgw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gnileqcgf.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gkngpnurj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gyjljhneq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gxlupdjdy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gvuaqkjdo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/geedjqrwd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gycqeuqri.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gzdblfdri.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gofgrpisl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gdgtvhamf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/glwnvasyl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gsplhjzva.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gxsolpvph.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gpubukzst.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gsgfejkzn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gwvqerpvd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gehwxexwo.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gugthtrjq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gtuhcsynm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gibedtrrx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gocaqtsya.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gxtqenuiy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gkiilbhnm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gnbimqrhe.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gmxjpsyov.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmrfbeedd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gxwopmymz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gsuaqdivt.sHtML


<!-- 参考信息 -->