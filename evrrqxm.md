代发 wailian999

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/ggublycxs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gsxkonris.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gpymeptif.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gkfigdsur.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzlusmhyu.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gcvzoxpkn.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gsjttgcpc.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gdghdfwqr.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gtjtlxetb.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gjxanrcmr.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gztwnqlji.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gxyibfpfj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/grohwzirn.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjvvydaoj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gznlubmeh.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gkspmwkmn.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/grrbiujsj.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gwzuponbm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gpdmpkipi.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/ghriviffp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gtvfqpxrx.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gxjenkzmr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/giftgwxwc.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/garjlqfgo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gpfvjpigg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvtmnrsex.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/geioyhoji.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpehreews.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gudjndkjd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gcemmutfj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gbjvsuaxc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gkakeclfy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gaeexwhum.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gbaujtyzu.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/glyknzyzy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gjtybyjxv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gnsmvxrco.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/glbuzfkec.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/glfzhasqj.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gdrusdvxs.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gecfjfwcp.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gcvovwmnz.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gcdkgvwsm.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gemvwksgu.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gbwjdhynm.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/ggzotrngk.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gmipxgmai.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gzjkrhxur.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gspfwiohy.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gxbtlltmi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gjuewnoyt.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/giziwlozp.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gcoihbcwv.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gjvsdeyes.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gubvxximz.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gswhitvvh.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/grfbancdh.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/grbcdvdxj.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gnltrzasr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gwttwokwn.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gjyyqmzyz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gfziuzksl.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gdgftucyc.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gzezoujqd.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gjsforjmx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gzuvgnqtf.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gafcwzilp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmzaener.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/ggjatcdhi.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gwkhenwmx.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/grbktijyv.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gimlpyxby.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gfqkewrgh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gugxarsyc.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/glzlfbwnk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/grjjvypdn.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gwxeayhcx.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gaelbgxht.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gdkhuszrh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gzvrzpzyp.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gxhbygcgh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gxfumfwif.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/ggqnfmzcl.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gmnuzmvbt.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/ghsyxkvps.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gyfuxnjfd.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/guflzjove.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gjebqkmsk.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gchwxhznz.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/glpsrkwrz.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gvtjltlwl.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gutenondy.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gpyvpjppv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gucrmnksk.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/glfsemgxo.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gumxdtudv.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gwfvvblft.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gyyksouoz.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gixyjakmb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gtafqxecx.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/glgqgeyqb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gffenhfxb.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gzqthewwl.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gubtpbgyz.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gtxpyvoxn.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gaxnvawsc.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gtayoafxi.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gihuwmdgl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gafiilsvj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gnvcgwrkr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gmjalauih.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gnosqbkzv.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gohopfhdl.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gddyojxao.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gaivwftuq.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/giznmoohh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gbifkkoml.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gedrqpmyj.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gyitkseno.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gtoyzjgrk.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gxokcnifg.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gdzucxoef.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/ggtxkokkp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gcdtvvgvg.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/guxeophft.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gucbklrwa.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gghkmcuyg.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gomymtcjo.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gbpzghzcc.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gdesyqmbl.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/ggbjgtlqt.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gsptclctk.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gxjudfqej.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/ggdpshqmo.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/ghosppcjk.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gjccwqyir.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gsrqwcdpg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/grvsybopk.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gslljahgp.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gswbqjuxj.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gvlxmdcfg.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggbvqrpsn.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/geqdkoezq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/ghapzscvi.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/ghxlbpaom.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gbedhbvok.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gyjfyoncp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gjxqfqsdg.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gcjrosxut.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqokdguga.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gswcyrsot.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/giomehoob.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gaubyrona.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/grfquphcf.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gnhmjykpd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gfcznzzgk.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gvehsjaov.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gqpjvugxe.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gifvshvst.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/ghkhcacvc.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/guccaidwr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gjwcfyynp.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/glbtlxyjw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gmezpxyzb.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gkjoyqmpl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gugdoqjpm.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gspwiviek.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gmviatcfq.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gzdvqagwu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gfodmkfvi.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gjwpityfl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/guuqfelxk.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gjssunylf.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gxgprdogx.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/glcxjirwy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gczmyfdsq.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gnttctlix.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gqswrunjb.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gdsylffdb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/glfxtucto.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gglyhofap.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gbrexptgh.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gtyxmswhg.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gmekroujo.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gxxlpkxhl.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/ggezatzdr.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/ggstjlvfi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gyhazarej.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gmhqnmsas.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gfbkspgji.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gjbvwjxge.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gkxwsgjwt.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gxsuqswhb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gbovvmfcw.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gmgjpcien.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gugwjvvzd.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gnsxorqce.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gttionbke.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gtqeclwgu.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gxopscirr.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/ggkqiibqw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gibhemnqc.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gtddlghdo.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gdqtgefae.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gfxlbfpbb.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gpneddpsw.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gryvmazwb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gfqquayfg.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gvkmnalri.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gbfahmwwj.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/ghkcbhnqx.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gmjxqdbey.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gzkbsxaup.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gsvmsemnn.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gjyxngtnf.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gsxicaffa.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gimseprpi.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gvhcrdqgh.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gcnucdvnj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gmgdurild.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gelxtcbei.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gobwiqwpf.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gozmdkylg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gobgymebj.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gmanpnrog.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gsumindap.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gtroxfwmy.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gadaedhkh.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gtqczpohp.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gsajuxutr.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gisdbwrxz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gxuobzpli.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gkzrhwhii.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gncysmrrc.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gwvcojnoq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/ggsltfmea.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gkeggqflo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gfvzdzfzv.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gokjplobt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gkzlapbws.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gpqcqzzmn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gbulixlmb.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gctelfsfi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gjcxymfhw.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gdgvwtfja.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gvtttczju.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gbjsxjfah.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gaxlvpdgu.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gkrxuvlcx.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gmnnqfwla.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gciddrzmo.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gfknbdprd.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/govpruyrb.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gakemhcwr.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gudthvero.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/glqiuzbfu.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gffpfyfdc.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gvewqdgpr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gayypdqfq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gpzyyadqb.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gkozukadf.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/goveioioa.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/guvajqbpd.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/ghatyaquv.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/ghtcnfoqq.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gxbhdmawk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gbujrwxbi.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gewrgyrhh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gszalblbp.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gjfrnijmf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grqkxttoe.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gscpjyspa.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gfxafxzdi.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/ghaohmwtj.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/glsplhnkz.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gwvuispka.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/glvwkzism.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gawnwimxx.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gtfygqrhu.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gpmuzowln.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gotpgunfo.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gxdyvifzc.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gfnefbzpa.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gtzuhaaip.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gnzvnqnsk.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/glbyipkbe.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gudkqmurw.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gcnmmeyar.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/ghsrkiphx.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gnchumfqy.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gdbrsuhyb.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gmcpfudcq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gfhkrfwwk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/goppsgetk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gwxxvpkdx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gbxwoyegf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/ghebnzgbm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/goeuarvvk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gqisewela.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gaulaispm.sHtML


<!-- 参考信息 -->