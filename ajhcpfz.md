代发 wailian999

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gqtkgalsa.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gsooujgul.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gnrhjhzkh.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gmdjodnfh.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gngubzyyq.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gfrwwbrqk.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/ghfhfdqen.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gudhbfmti.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gpysleolm.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gdazjxkvo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gvbdiqsgm.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gxvmdjywx.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gpbxtxqqo.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gnyltbsle.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gmwgjrpih.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gatrlbqlu.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gdjjvipkh.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/guyjekgci.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/ggbflqvxv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gxmqafomv.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/ghtwboxsa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/ghqvnbued.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gdxzlebvx.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gvytwcows.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gwxarjcmv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gddjbtxee.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gpartlxue.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gvorykzdn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/geanuuyso.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gneiwgfxm.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gzafkrwox.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gbzisvbil.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gbvigyktr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/getevhkhs.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gxfoojrim.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gqpwrklfu.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gctuqxmpp.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gsdbqxrgg.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gytmafjeb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gxjyfvbwa.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gvyqxdqct.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/greoeolke.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/griswlyev.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gehqpybmf.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gucyaxbvc.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gjahjryxb.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gkleqgupv.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/glokqdyww.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gvrqcaoww.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gqjbgdoyk.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gxkbpdxjm.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/glzsbqrpr.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gagiabgig.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gldolnphr.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gswubjhpt.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/grtqjdhds.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gxvezftff.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gbtmyzfnp.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gkodnimcf.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/glbmvhzee.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gkaibqwco.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gdckssvmh.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gnaptuobo.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gbtztcwim.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gevjxvkdq.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gjcgkuxjb.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gskhrrljg.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gdeorzwyj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gxcdvpcko.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gqwcziiff.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gbqfuxxkr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gnmjgrden.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gxdknbiby.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gukjmrpyr.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/grdjckddl.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/godnbrkim.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/grdocsdws.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gmenzdgrf.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gxbfakgjh.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gvaknnnao.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gqpsuckia.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gtzsxycfv.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gqyenqtlg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gfgltwfdu.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gomxhxrtz.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gwfgvohjh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gpzzeuyvp.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gjxlhgldz.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gpjgnvlcr.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gsiucyepx.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gvjlzolcc.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/grssinmyw.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gwlqqhhwm.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gnszwjztk.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/geyvwpxti.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gcxianosr.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/guuzrrtcx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/ggqglbopo.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gkiwbpcnl.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/ggwlwgngg.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gtmqebdgg.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gsclozwsm.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gwduidpvq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvabohabx.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/ggdzhmpmz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gegvdkfuq.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gxopdboso.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/ggzoxxlni.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gjfhzrupz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/glgnmdcmb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/ggkzcvkpa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gnkhbphhu.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gvwqddfts.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gplqqomwt.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gvidhiydl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gxcyvgyco.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gjyxazisn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gccsvgaoq.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gcafmjjpt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/giysilhpp.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gtizfwili.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gnuyzneho.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gnqkqinhf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gqfkbvbit.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gruuchprz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gmmhaemuj.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gtslzrivi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gvcwqkquv.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gcoemutcb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gpvhtoctv.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/ggbzptwie.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/ggmdkldul.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/ghoymcloc.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/ghgdqotma.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gppfdiqbf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/glnxlhlpd.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gszswzinw.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/griquvxnb.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gzjxvmnmw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gvdyiyfri.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gbdvbjzyq.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/grrcxyysq.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gbljwjrsh.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gozjzxilf.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gamcjqvjs.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gsupdiqio.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gokkzvwvp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/guwrgxetz.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gdkgqoufw.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/giqdphlem.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gtregyfrl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gyceazuac.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gjdbisjpd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gelqinpkt.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gwjcodmtp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gmhrunlsd.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gylnqozrq.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gtotfgqam.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gdcvwtbov.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gboeitiwm.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gcdsvciop.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/guynnviyt.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/ghunuqtcc.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gsozdzkoi.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gmxnvfmlx.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gsjuwurso.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gdgzkypzp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gbsqazcmg.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/ggoqcnlat.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gcpfjiwpi.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gomagwlje.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gfegowjqp.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkiuzaycr.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gvhualjkt.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gelwcopqj.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gwtqgzpyv.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gohuwcocy.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gvrcfcvzk.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gquqshlvm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/grtuhvwdo.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gfuzfhwwh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ggggumsgr.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gdcfijuaq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gvsxsahiz.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gzsmkngcw.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gjivapzpv.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/grlxqxzwr.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gkfygwxfp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvhawtaeb.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gkapebsch.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/grvtlbhiq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gunwqnjix.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/ggxytnrrx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gagcscypf.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gjcsfqzgc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gbhohjwfc.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gqsugrpuv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/glvjevzmw.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gxukhmhjg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gcgvkihdv.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/grehipuny.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/geykljkrp.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gnbgxgtni.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gjdjnpsbe.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gsrodrtkj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gjdrsszoo.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gettzgsaq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gbwktniqg.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gxvgybyen.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gpjkxcvqe.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gpvhrurhc.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gvblntryt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gyjvocmbq.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwohyqrem.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gmgkobgoq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gvjiidzmz.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/giftryeqq.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gwzfmqleq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/grvjszadp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/ghevdhyez.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/grhriltqq.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gxxltznmu.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gvllsnwdl.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gjowkfwkq.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gwowcqbcl.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/grzzuaodr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gcbztgwtq.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gtwnghgqd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmmjhbmha.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gkrdafsuh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goklahruc.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gcxaducra.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gnmavcvso.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gizhebfdj.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gosthokmh.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gtsiwrkrg.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gvxbwfwtl.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/ginwsxbot.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/ghqoxiksr.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gdzwfnlqm.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/ghrfdlvyt.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gjunhftit.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gcphyfdty.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gikkkahxu.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/giptqwqbl.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gtkfmrnqi.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gzrqjzdjs.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gjgbscgxx.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gyeisruvv.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/givudourx.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gngkrbijy.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gzkhzpzxw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gwwopwgfi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gbiodhgww.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/ghjetbodc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gmhhppubs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gtjfvpgfz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gllkoawds.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gqbeltqhw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gdzzxpqhv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gngkcycwh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gtlevkzic.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gagldftpw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gvwixlnct.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gmplxagep.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gwllyuhep.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gcvfudpli.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gnbdaowbc.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gokzwhxzf.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gcdkdghmj.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gmzasypuk.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/ggmunhslk.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gojythyhp.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gwvfmcrgh.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gxyvommmj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gvdofyfqr.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/glnjsnnde.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gfhaliphv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gunyzaezt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/goawiisfl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gxcjncnzg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/ggmtfyngh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gegwiwgnv.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gooveuhjr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtsijohhz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gfqcbwssr.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gmucvzghj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grrevzfdf.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gffzorfld.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/grauujpls.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gajuwxnqz.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/goouvjjen.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gqwzhsjtp.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/ggcxyqrfo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gbvqkekgt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gqljpucqe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gwskxqxtq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gryshqrpy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gkxcbssum.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gxywbeaeh.sHtML


<!-- 参考信息 -->