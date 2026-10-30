代发 wailian999

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghryrldgq.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaqvuosa.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfatkvxe.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzhxdrgb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrlnckug.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gwhxplyaj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkdvtoxs.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gwmfbpgqr.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcktojrzt.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gycicgvkx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycamfllt.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gwparmhjv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrnzmllx.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiadspxy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfimgalfe.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gdusrjkwr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfkpofmp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwcqmwesx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gcddkcdel.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glqiilqky.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gbnpykydq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gqielkebq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsfhphok.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfznstzrs.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gictqmtiv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gjphhdbzq.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjfnoatt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gglokylap.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gdmdobqlm.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gckfjvmiu.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsehfhvo.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gymoofdou.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gpdkahtpg.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gkqnnnhyp.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrivcqae.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gurrnccvz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gagantdaw.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfurdeafd.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gvsmdsoom.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmupzeol.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomyihhwd.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghufbypxb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ggncwlxjm.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiomrkvm.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gonsljyqa.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqlisxyd.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gtnfilpqs.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaqmvzly.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpbloclv.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxlcybiu.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecufwlcm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gbreyoypj.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpdebvis.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyosfjod.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacedimon.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gbgomvadm.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gywerclac.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gyysijate.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkddosms.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoksfmhx.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaneuvop.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giantoccc.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gjmiswklh.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyzeocmu.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsauzwixy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsroooidn.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/glvegpxsm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsonwpunj.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gywgclhms.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gugkxcijf.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqgnccgc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqullohdk.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkriieffi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/ggokleayr.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gvxyyvlmp.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/ghvhxjzmz.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqdlrypt.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gnjlzuyao.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gtddehtgq.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpmkrsxn.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoporibd.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/ggtqudqfx.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gluynnrln.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/glpbdrspn.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhzfjetm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxfjosfp.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gykmgueey.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/ghynzadza.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gnkaewtji.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gmesjccdj.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gygvcpgov.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/ginbfovoe.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyqwzvfw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gcwkzeisj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtyydujp.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gmdamozoy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggozmshxu.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gimbwiwrt.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhxenwuh.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gwypgafiq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqrdgcjh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/grvzqahca.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gauxgojdz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggejcqvtg.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/ggqessahl.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gtnurmqgz.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gpcqpweum.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gqjtydozt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gxprbytlq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/getmxmyim.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfimokhxr.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjgynlqo.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghdbohkrc.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gfyqyjtkw.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhouakss.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxnovhyah.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gcieczgmn.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gpybdrfuz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gmijgckqy.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/grumuvqhh.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlnshnse.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwclgdiiu.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvrrgymjh.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/glyvthyzm.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbrsqbnr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grheweqme.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuuvmtpa.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gitmmslhb.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gscysludr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsuqgznt.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gutmhvros.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuvmfbbh.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gcpwbzonw.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatpqgrde.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gdubyoolk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzvzzast.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gilzgaqhr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvcozxuk.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gxvyyficn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcihuoxem.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvdhcsnq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gfrgkdxby.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gclffkzzc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gvaxapyrv.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gqhjanwmc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gkfuxnjzo.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwvbcbldz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/govjkmbsc.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gydktapjs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaikbkrj.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gjemljrzy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvnythjd.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gjbgbzbgg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gpatjmqgv.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqllvatgv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gqtlyryag.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gswuiqqbt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjfcpayh.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gjhymausp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gckcqkklt.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjplqfrb.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gmceisnxi.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkiiihmd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqgbulsz.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmzksedg.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gdndbgxem.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdcaanfxa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghymekgbs.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepjtepkz.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gwaaviery.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gbokmnqmx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gevwppkuy.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwhbtczr.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gysollpvb.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcwzkvwu.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiiviqvb.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmclrjbli.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gkujievlg.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gojctbbtc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtdyaabt.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbvurrzk.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gtopviqrl.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokmigiph.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gcbfqugio.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gwplhmhte.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gxrnddzsg.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/giykispkp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/ggjeqpbcf.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gtqnzcpct.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gbatqvyvn.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/ggjgkofcm.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjqmzfjx.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/ggwvfnput.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gayuhipzb.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gccicqhbk.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaebhnqyj.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gumpuwtxa.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/goucapqcw.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcqwjfkj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gaqfdavgg.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwscrnlvg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/glhpiucke.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gearnmqdf.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gxofkngqz.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gklfvovqu.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqelmamet.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazopniff.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gmofhnvsz.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gjcrucnzr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmqaffzp.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutibbxhn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbeawxwy.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuwqoija.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvekokjtl.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbioebha.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/goympyvrz.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadhnxqar.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gnemvlebn.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnpvlgyd.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzrmojjc.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcvsxrcx.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtvvelex.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/grxcyshti.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/guubjvqqh.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gkbshunac.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gfgbwukem.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gmegfpata.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/golnnhymo.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gaftbvyzi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gbdunfgnt.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gmoomerqe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbaznhii.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/giqiyvjif.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/ggmuofswh.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gfuqtdusx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnmpkerw.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/ggmxnhiev.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcidoafqq.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gopzhyqsb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gurjrqkuh.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwiafmzu.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gmyhbcyzr.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfikncau.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkwptbwz.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gfyupmlgu.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjepmepy.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gnacfrdfh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gmxrqamgu.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/giimxmwzi.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gekhvtruh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gifpddrrc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gsrieoyan.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvtnpolp.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gwvfmqges.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfvhpice.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmrcjacx.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/goevdofbq.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxpzjblh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gxtbcuhmf.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbrshtgh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvueeyuid.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gyfztwgir.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbktmrcl.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxnegduk.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gexeocdgm.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gljbkyfzv.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyumpxcj.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gafroaoky.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfriucmq.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbobkshf.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gufniehla.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdfabflj.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gljfpqkgl.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gecorcpqh.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkllgyop.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gqrdwnzku.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaixlvve.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gravbrafw.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjpfbgri.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwxlbxqw.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmxhxlko.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdpatgec.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnubfkek.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gfadoitjb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjjllvvs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgbbvbeq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gcpyttdjn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gebglcefx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gcomjsdoh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gmqircmfs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gzugrwjfu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gzpcigdfv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gaiflhkpp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gqujqbyye.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyuorlnn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gndxzeksw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gpjgonhcs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzplwsxmn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gqktzshax.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gapmegblr.sHtML


<!-- 参考信息 -->