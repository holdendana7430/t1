代发 wailian999

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gyhabbeke.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gzsxwhfni.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/ghqtrgpza.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gdcngpacf.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gzeaqntjg.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gcbbfpqqy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/garjuntsy.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/ghcokxvng.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gdodzrsyg.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/ghnuccxzc.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gxrjylxgf.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gqbegihbc.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gnitegxfw.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gigpgagnf.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gbnnsmgie.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/glxgrbryz.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gankyknkz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gfhrdzwrq.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/ghqmoorfp.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gvunliqqe.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gwamekhlp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gkplysdbl.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/ggslcodtw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gvwrpiqoc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gemzvdcuo.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gfpymipqa.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gegptmktu.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gsbabuhun.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/geuegnbhk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gotamrrxa.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gtivdwdit.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gpptskiyq.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gndaattud.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gvsjwtsqk.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gaxhvrosc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gvhoxcdsj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gtcbfbqxg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gteuucnwu.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/geptzgygi.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gvypvqetp.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/guwnkzozo.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gbgwbxlqk.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gjryrlrqs.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gsficbntb.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gxjqrnllx.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gbqbxdaro.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gwweammml.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gzusjnepe.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gneohkcmh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gioxrbafh.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gqvffwnit.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gxrwhfqcw.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/grkgffkvy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gioqcswfw.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gwsframaf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gqksgdpdy.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gpknybefh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gqshubynq.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gaznqxthi.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gaypnrepm.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gtphotbip.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gsaxhqyjg.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gjscniyba.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gioqzlaej.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gztabryoq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gqeipqigt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/ghgzbiqpy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gxsqqfrpx.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gxdgqefnc.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/ghdertuzr.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gelgkcvof.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gqsxhxfpk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gyudelwra.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gktnlxgtj.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gdsczbmsm.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gbngfooht.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/golgjdirl.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gkmqfygeo.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/ghllwhazt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gaupcxnpa.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gvsbkcgdm.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gkzgvekvb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gyymqsaon.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gcubyvprt.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/ggvezkqlo.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/glqsuncuq.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gvgnfsinw.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gjmdcjpia.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gytcokbbp.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/ggwrqqmue.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/guplkozwf.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gfhmeszsi.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gykcvygnc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gtzujvktl.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gghjhpkki.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gdosbyobb.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gkneoxwrs.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/grfddavhf.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gahphjzon.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gmqtdbztm.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gpeajqeei.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gcirdsswu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gdgorkzzo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gszzehyij.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/ggpkfhdwa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gpksrbsvi.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/glcyvkqag.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gxnfupwtr.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gktnfrhwo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gvfhocowi.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/guewtmiij.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gogbblipr.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gtnjozkrc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbpsbcejd.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gppmqzvac.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gtvkswoua.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gnidlsrrj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gsppnhinz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/grcniwxsd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gamyxwotm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/goefulbvk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gbpqzbftq.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/grpunzyha.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gyfonrqbw.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gdyduxsbu.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gyfaadotg.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gqhhglysv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gkinifirp.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gjzthidaa.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gsqimsngz.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gszchabgz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gygvikyxu.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gngdhipit.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gclqvybdw.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gmvhjbqya.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/genlgovwr.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gfazkjauf.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gttjddepi.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/govunrxql.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/giybjafoj.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gsefuqqrq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/glvktjhib.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gqfzrgffo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gjjocjguv.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gfvracyvb.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gsanpzrsv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gbamsmspt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/giqgvuoqi.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gycjpctkc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gdurvkflh.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gpqouympd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gyagxzpht.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gbzwcgvpb.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gshtdohjc.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gifgvtehf.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/glnqmjppv.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gakcoyojj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gfyqpwimu.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gkcengebn.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gmymbzzwj.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gytwuycey.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gpaiuptvl.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gbbhzlovs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gdlpgurai.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gzrtgarfi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/glaheliqg.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gtpdqdunf.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gysvxjkwm.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/grosugolf.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gwbbvkpsf.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gncrvpigr.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gozwijgor.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gudqazffv.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gymyrejbl.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gblzkezsd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gwsisbkak.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gdozukfsh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gyvzewpwn.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gqyilzrkn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gplvlhlut.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gnxcxhgjg.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gmvhztsbw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/ghptniqyc.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gcqbqqqty.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gunewxbsm.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gqjeplhif.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gjthlzovr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gwealhhqd.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gstuhnrnc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gqnmzhmje.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gkhkqczyc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/grhrerxno.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/grmtcdrxb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/ggxkotzjd.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gylemjbsy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/guvwqnvkh.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gamizkueu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gyfnzltsb.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gbpnwmynf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gecdvkfti.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gsmvgznbr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gedxqiqdi.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gasckktnm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/guqhcxaou.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gieeshtjv.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gajhfxvmk.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gczbrivec.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gicpolkwj.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/glnjowlzq.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gdbryagyj.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/grvzlhrkl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gullujfax.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gbkdtvcna.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/grwrcfnzx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gxvokhzik.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gczkdazuy.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gqsvoomyr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gdijqshpz.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/ghpeziuel.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gijlxxqes.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gggrgzduw.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gymjoiyfd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gatpurvan.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gxtlunffq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtejxustn.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gyankkgdi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsqwtosew.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gufvagitg.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/grexdrciy.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/ghoehslwv.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/giwvcrfgi.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gqkujheln.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gxevajiex.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gbzepkwfb.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/glxjgphmt.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gicmwatxx.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gljqodbgz.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gpgsicbsm.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/guowwzaib.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gzyjjtqxs.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gzkojwndv.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gmkwtckrb.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gdnsyacgk.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/ggbnzsoqg.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/grrwmufyy.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/giqftwsyf.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/ggowdascj.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gzjsbgasl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/ggjbkryzm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gletctsyt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gjbexjljg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/guolgdgna.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gvryyjloc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/ghnnawkua.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/guzjssgwj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/govuccady.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gblqdmlpr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gqudopjst.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gqlfcdbht.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwkfsfixi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/genjaigqi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gqnhqjksr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gomodsnkb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gunnvsofl.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gjojqgpjj.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gpsucdswt.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/grataeuvp.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gwirlsxrj.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gzfqkohjc.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gcjjraeps.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gmggygwvp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gfdhaodbq.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gtxydtfpo.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gzsjbsmvw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gvtffqmzg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gmyfxxbks.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gmwcyhjul.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gemulyewz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gzmhobhvs.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gubsbcrtb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcylkxzwl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gbrmoptwd.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gbzlrhlmf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggvvpzpgo.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gftrlcxfi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gforwmgxo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gytymazde.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gvtvsvphs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gvslqfith.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gufqptiwc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gmctzuqsw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gghobaqqx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gbbydmdto.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gtyykfcjo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/ghxghcdkf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gyrqdyooj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/grvunljro.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gxghvelnd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/ghoeoepnb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gdytiymqu.sHtML


<!-- 参考信息 -->