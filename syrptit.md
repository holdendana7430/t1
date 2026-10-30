代发 wailian999

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvgnhurw.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtplgihce.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/grymxnmcm.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctkspmef.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunvldksj.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/geqsdukps.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzgcwzdp.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbcxvhqx.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvfexxsc.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gzzvnfdep.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gzxdiielw.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/globtyfvv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gzwlhqpcy.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnbmlpvn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gpfhjzgzu.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtcqeyio.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gixvvkixv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpsjawia.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgrlxdfu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdifborj.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvbkzjbp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmhccicj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmqnpodo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwcalrxsf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgiobcjj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjicyqrq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewqvumat.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/geevlvegf.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gpcutbrbh.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gddfctcnl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyldgiyvw.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gldgktlud.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmgzegfo.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrvuoqsa.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhbuqqwt.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gbjozxauy.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkdfizfx.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxzwmbkz.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmayjiuo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsojiqhj.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgfyoouj.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgmapslw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvvzilhk.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gttkhcyko.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyiqaanh.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdepuqhjq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gejsoaixr.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuujjnpg.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gupofersf.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxradjmxf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gmqpfptlg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gtmfvykxz.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/geaxhlqiz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/giyyagchg.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/giszqzprr.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcptvqkf.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiddydzc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/giurdtdcl.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gwibqafal.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gfkmihius.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/ggaapgqfl.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjluwqkj.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzkyyuyj.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewkjiwzu.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbelcgrsz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gkcmqkjmc.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpmeuuks.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvncajqm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gzspprouf.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosyfeehs.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/ghaoyofhu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gzatciixn.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gtuvphbll.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/grabgazbb.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiggyqvl.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gwgsqcxic.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/globwmomt.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/giztaogzh.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuoewvqg.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/ggcydojzv.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gywzgzzky.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxmgzlip.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnyfgqnfh.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerqzhawm.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxxcyyxn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gunifzcdm.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gkyyplvox.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhomfmyy.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gksoeggds.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavhexihw.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzozbqzbb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gqwigprfb.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtznxxlfv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gmdpweyot.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/glzupiibp.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmqhwnqs.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsikmxmzl.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyvpveji.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnckmyyk.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gipwvvgzy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/ggbwvkoeu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfoacaqm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/giexistbo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlzkxfjn.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gyajrnkpv.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/ggxmhcjaq.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gcaiprnhb.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaezgzhh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gytbszsls.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyklusey.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfvzqhpl.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gviffzirk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzgdelhb.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfispzmj.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkzrszno.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkartdhfx.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gdetrasoc.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmtrdfdh.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gflgxxdaq.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjybyhbsh.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gubilnjzr.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/giuecphjp.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbihmkaul.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/ghyrqctuf.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/garmcnrur.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gyxaqfomk.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/ghfgemgyf.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/grxvdkvjd.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxbajfnu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gykmwsslm.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxwwawmok.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxvjzsqxe.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrnsuyep.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/genudfvbi.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/grtdbopab.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gqgtnazlw.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gjelyawlp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvnqsfdy.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/guqvneeta.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeojofbi.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkbdymoo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/grftmvntz.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbpgscpl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gidrgdpdg.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/grkbbsdpk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwkdqogo.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gcbcxiksa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrwiuljx.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gouwtienw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbfhhznj.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gzueufwvc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gjnlqqwrp.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gduvgjzkr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnptsmmaw.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdnpeuxe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpssopiyd.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgimopiy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaycmwmbj.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjcafrwn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gppdiahlq.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gjahmvtlb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuzsleog.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghmdwbgri.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gvnyngcqw.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgaxlzsc.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gmwnmpmic.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gstlrwlcx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gqhstkaaa.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazqpdgdq.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtykhyjbr.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goalevuae.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqhlfmdd.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/guclzpanm.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gskiklbbl.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrxfhlwh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynlvipmw.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhbntxpq.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlspyyvo.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqmeyvsn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gdznejbaw.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/giqaskgaa.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/grjzckdet.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gyibgemfi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhofntgv.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gejlqrpbp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/grzcmhlcx.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gktejmlnu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqdtgzeb.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gkkzkwgnj.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gewsivxqe.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegrtzilg.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/geinkqbhh.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/garjiobdw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcitwptvw.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfyvwvqa.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnvfactj.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/glffaohgn.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyzxkstz.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/guzeulvwn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gpxmgjwap.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gdmnqzktj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/ggufvyzgo.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiopwylj.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpazkfke.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulengvxa.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/ggcqrmxpa.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyjhsqxnc.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/genrggszb.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeasjhvx.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/grnbgcmum.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gznmargwy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gekmctvfg.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/giraabtxs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gkujndbau.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/grosyvalt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdkgrrbw.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gjinocsyd.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/guezafmkq.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gsetxyhpj.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/ghhsiwyhj.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gakvesrjp.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/guujirazm.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdwcxycq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpyonein.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gtziwdnhi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqunemfxf.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gqiirbeij.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gatviufek.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gukyutoyg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfkmbzsw.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gjsooisbw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpfffqoi.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjxwhlaq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gpgbearee.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcketlcfb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/ghnhpgwdr.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrwnhmwm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/giqanmdto.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiprdvhy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhzfdnek.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gsapmkmza.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/geswqayer.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/grqcrflgo.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/goqfhujke.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdkemgms.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gdfxvgzad.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfudcpdbt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcukoewbn.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilybdmgo.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gkoafgwmg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgwkxpnk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/godhfqyth.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gdfviixon.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhxgjmtd.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvirzgqf.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gftgmgegt.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gmepbxoht.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywjupiaa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnziybnnq.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/ggukfdkeg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtexsggxx.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gmswkikqi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhqknwoe.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gbydqwdak.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgeiuyib.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gmygqxqso.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gfxrzkjkr.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gljecfnaf.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgjpoeep.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gfcwqkztl.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gworfkrtp.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyuotttc.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gxanyecqu.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gwgdpggng.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbqgoajs.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyphdvhgo.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gllymailz.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gceuowgtn.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupzeliza.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/glmcogtvi.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gshfoodfh.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gsanydxbk.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwtwfcmg.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/glmgkatfy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gbcjmqjrs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gepkvxnma.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgzluoqh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gyvvwjigw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzipwlfj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxlyzhjp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijbjwqwi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/glyxxphhs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrawfzbf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gkefcoekn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gflcmhevw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/galiwkjno.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgylnari.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gapitzkdr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gfehxhnvx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxyhvdnq.sHtML


<!-- 参考信息 -->