代发 wailian999

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gmutsjbfz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gzhrbqaqr.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/grhbyakwn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gfqcexibz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gxhebzelx.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gjyrgxxxq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gmlnvtjse.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gujfqrtws.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gexvluisw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gxrpszsnc.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/glgfsdeaz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/goehjjbpy.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gsmksryuv.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gdrchgfrf.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gnbbgxyie.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gtnfnswti.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gkutevmvj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gkwfoauds.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gnpjgraah.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/ggrhrkpof.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gzlggauhf.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gmvefiueh.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gzgfqyjcz.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/ghacgchvi.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gwufrivqj.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/ghvillwvj.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gougihhxr.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gceopykan.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gnbaapaxi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gexjlfbpe.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/ghcqxzetn.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gicislhhx.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gsyovakws.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/goxdckpsi.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gqnnfdqef.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gpvgnijzo.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/geweznstm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gquxvbmrj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gduiagvsv.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gtszsifqf.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/guigtawxx.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gjzbfpdbn.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gxhpxrmro.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gklvnsfyb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/giwgqgujq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gdvepzjcj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gdjyrvxpu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gqqiqyblj.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gxnwkgoqa.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gixypzfxq.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gtvmuovfe.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gpnevqehc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gwfabwmon.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gzjnscyyh.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gyeotdcoq.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gbwsoqttc.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gmrbrgnyz.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gakjxulmi.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gxpuvkdfa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gojnagxnp.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/ghtitaygu.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gcsvehtij.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gywlsbuym.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gamrdgjct.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gjhzigsjo.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gxjxvmxwu.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gcdyyscso.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gpatbyois.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/geszywgvu.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gtciruhnf.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gzlmmnpwl.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gblvmijlz.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gekzvfuha.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gzqihzawz.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gvuwaqduo.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gximkmviu.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gxxorocxo.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gluftctcn.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gvaewkrkl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gwjpdooqh.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gobdjbixi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gybdornlj.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gdrvugcpq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gswfgbnqd.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gvuzsausa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/ghvebbjzx.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gicgrfdcg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gpdezbnwq.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/glyjydblq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gxsagruks.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gxyvlxhmx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gilbkglpg.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gskitwacl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/ggeseefpx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gxwhgrtey.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gtkrhcoij.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gqeklvtrj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/giztzlmtx.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/ggbzgkqgi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gtldzbolb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/ghyabzttm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gumehnjup.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gnmntsyys.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gydwzqpcu.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gujairdqe.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gjcodfrzb.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmjsrfumg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gctgjekee.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gkqqgxllv.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gltodfjti.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gelqnlhxl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gxmrrpxlp.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/ghrehylge.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/ghrgphdxm.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gewmtyzrj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/grwvsokwq.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gvjstbhzw.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gjkwalncw.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gfhsznepz.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gvozhgccn.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gxejteume.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gndmricgv.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gnqvwccxx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gjzfpanpz.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/glpgjsgax.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gmipzyzwh.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gxmtoizye.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gxjdzbdad.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gsfijvckt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/ggzczdyka.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gncqhxabe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gktsuidtm.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gfkgxlkka.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gbvdixqtn.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gtuoxkzkp.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/grudpvrmg.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/giizzkkkc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gjouhxwwk.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gxgdyxduy.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/grgfzetbi.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/glcxkacvq.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gbvtfkyhd.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gksvlodxz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gyuvzmvco.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gptdklqpv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gbglmqvfr.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbpskesur.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gpxxtzmlh.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gyxcnqrmf.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gxmtmgbrr.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gvqvusblt.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/godhudxuz.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gyaojptag.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gfelnuhfz.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gyflitooj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gyigswequ.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/govirzmkj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gppagacmu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gnfoutarz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gxtwbenyy.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/glxvicvjq.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gfleytwob.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gsvzuuhhj.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gruxxslbz.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gcytijspp.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gwuaginjt.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gsmdxagvq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gegzjodeb.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gkxjexqkd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gbszhitbc.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gwsnjpzai.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gpoqbenxe.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gnrualjkg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gtosfhigd.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gftaogrke.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gzerthccw.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gxrnpupvr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/guhyaypgw.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gvivrndnh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gpytgojcm.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gpjoycrsa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/ggileaxgv.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gmwytutel.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gmghseuml.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/goedqbcbl.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gdmcrxmbc.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gzspxohiv.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ghlruvzls.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gdhfqghfa.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gkohhnioi.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gdhignkhl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/giejefsrk.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/grjopvgap.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gwmomorox.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gqkxqmmhq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gscxtthnv.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gdcbhmofb.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gpvljgubd.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/glasrecfk.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/ggnnzlhgq.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gudtxxcef.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gzqyswjvw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gvugqlacj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/goaaajpdy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkjgxjvrh.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gfnvqrzfh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpdktgizb.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gqxkugspr.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gjcmkzywr.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/grqjdaiae.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/ghxlcgczj.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/guhhboqzd.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gmzfwxrjm.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gkgugmlzq.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gsifkdify.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gglsselke.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gsekrrgwv.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/goyipaupg.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gxstefpev.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gxftdhnpn.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gckopcncv.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gkbsyfltm.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gdzqfieep.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gsoukwqrs.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/geqgetajp.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gnydiapsd.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gjjpvnmet.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gfpidaeht.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gubyekjjw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gnmgnffso.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gbxhpzhmy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gxtuoriof.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gsmgrhegm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/goxpjajqp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/ggkvytatj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gbbrqttqd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gituguxjm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gbddfqqpz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gqoawduwi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gqbdqaeln.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gaundqhar.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gdlffyiaf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/guqayyirm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gahldzdgy.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gacfotqet.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gnrrzzoqs.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gfxoqqjiw.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gkodhvjoe.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/grfjtbyac.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gtuyppevl.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gfpdxknkm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gogzjbiig.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/giqzsmdsb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gjfrvrewt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/galxqxzqk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gnclkcsjt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gdfdpcckl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gqqdfehnn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gpspifgjq.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/ggmkvfebn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkbystqjd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gpqpkfkds.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gldoohrss.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsqelkons.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/grbzsccvf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/glydjaidm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/ghbjqiyvo.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gefjaqawr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gwtwxpewz.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gmsqxleva.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/glxboxpcp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gppopkuxr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gycbzyuvh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gioiytrqb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gavgozuuq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gyxenoiep.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gzbybawpw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gobbrvtbr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/godhmmfwc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/ghiettzhl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/ggjwykjjt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gthaliztt.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gtsxtlpwa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gxrdipsqf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gzbtoqmne.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gxwhyyche.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gxbkwmqvq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkhrnjnsv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/goevrifqz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gstqsvbak.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gzqvbkabg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gohraxdmv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gtaqhprrc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gyewbxlmz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/giaxqzrly.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/ghlwfxuvl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gfrslgire.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gnzigqeiq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtwomxehv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ggqywlysn.sHtML


<!-- 参考信息 -->