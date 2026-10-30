代发 wailian999

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gohofjjyd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gshuigvnp.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gzwjhczrm.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/guswzayae.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gbrrgxhxo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gvaxbxrni.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gnylhiqxd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gpiafbxvk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gczltgnpu.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gneqqpzec.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gjavfztyl.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/grtrrmruv.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gbsdfhkwh.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gxwnqlkft.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/ghanmekyb.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gudczrxne.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gznpqhokw.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gmosoraqp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/grlriunrb.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gmpfojhqw.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gzhrvwanv.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gzreytkfm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/ggshednhw.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gyxeuvkum.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gugolghaq.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gbkhktxhv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gdpgsvlxb.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gacxnmkfp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gwrgmocan.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtvtxxlwm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gbnlxoqul.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggztiehln.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gnzblgjdd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gbpdixeah.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gtutfsomr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gebegnmmn.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gqgatojfw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/ggeodozet.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gbbsbvqff.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gcqmvhqgn.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/giiwilefe.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gwprqiruy.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gshsrzhyx.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gixvvxabi.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gutxdseyi.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gkmlcutud.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gtqgovelq.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gntbpmpbs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/ghezcmntz.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gqxdobykb.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gwcrbgsop.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gsqiwxmwq.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghjemtthm.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gwmmkikiv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gjxiuqxtf.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gjrsuvyep.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gsvwtzbxl.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/ggcbgvzux.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gbqyuldmm.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gyavtsmdi.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gzyowhrzr.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gnptezmel.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gvdnjvidk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gbifdhhky.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/goqzoudex.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gfasvuzzq.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gwbcfewwf.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gjhxeexoq.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gerxijkvs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/ggpydmiax.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gjpyjiaia.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gwvajljjx.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gqcmjivbz.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gicymsuro.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/glokjvsxe.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/glhqbfdiw.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gjyceulkf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/goxfqteac.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gsegxfjev.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gaklcxpqs.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gmxkueznq.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gdxxgnblg.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gchoghzbc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/grbpywgoy.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gjioagcyu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gwagslhep.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gowfjaxmt.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gqecuixft.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gkjnnjnlr.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gxycvtxyo.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gjtjsfuni.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gawiiivxd.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gdxebnrza.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gzmjnbhrl.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/guhpxlorc.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gsysktfii.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gblbpinqt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gyexuzfpd.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gddirfcfl.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gvjwdcisf.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gibbvelmt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gyycxgnbj.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/glgzgrsqz.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gjcocxwzp.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/glgfbotbe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gcqfgccvf.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gukxhdshz.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gvlyqlwyo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gdtuccyzz.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/giehqkzza.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gxzokyafz.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/grkfczztg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gphfvywvx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gvgsoslek.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gddekhrjy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gqtmiltdb.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gfdfzzfam.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gbfhhwfra.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gsswaqhko.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gmmajqmdn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gqdlwixcn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gfdldpyrm.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gjfkwmxnu.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/galvdpotv.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gfdvzonte.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gvtlspnhe.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/giapekbox.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/grtasiprk.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gngjlytvy.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gzwjnpriu.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gwbnenloe.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gfzzghtjk.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/guyqqkfnr.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gekahynam.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gytgbrtcb.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gqwzyzuqr.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gwalmrcet.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/grszskppy.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gscinbrba.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gkveattpk.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gsnhjqrqt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gxrdtovtx.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gopzzspir.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gulobpasz.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gzuxgorwa.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/grjjkrnpi.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gykbqaxws.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbpcvooqb.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gmjlqhuov.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gctuettsn.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gplivsopy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gyczlkzao.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gellsfufb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gvtcyptrk.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gmatmiafo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/getcpwvmv.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gkubeswlf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gscymidys.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gtexkuluo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gqcrtjofr.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gcnofbabs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcdycxsrj.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gfwgjjpeo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gtpmwiifi.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gttzhovll.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gkhgmfjym.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gzxjivpkv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gbfjlyqfr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gpyvwcbsi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gspdkgioq.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gkpgsxyix.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gkjvmdeqd.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gbebezncg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gfzrvewop.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gtwmzqhsq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gtrywmusm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gdixfvkil.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gzvxweqtv.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gpxzqaiea.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/glwmazsko.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/ghadcpfkz.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gdavtmlgr.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gxyijiebg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gkfcqcyye.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gwfddnokq.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gikwcrgyn.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gpvtgcdjn.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gvinfwsbf.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gvzodwpjl.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/goqlxeeyk.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gxwptlisq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gmgjvuuea.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gcbomgslp.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gefizcpij.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/ggeydjcem.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gyuumzbou.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gaavidtwf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gnghkczvo.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gamyzmiwg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/groczzpxz.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gplprexkb.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gzvmpawdl.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gfhxgpwmh.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gtzgmsxyp.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gseafxwtc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gpguoxifc.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gdoikvbmu.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gpuoemswc.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gagdeijqo.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gnrbkmmgz.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/genaeuvzz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gjvzzqbpv.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/glzcklxae.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gjrkmzopv.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gntczdwhu.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gtpqjnsep.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gwtttmxob.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/giozdtsey.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gwwimnbse.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gpgaitoem.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gbulizhkx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gywrmsnfo.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gvaexzmsz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gmebfkszx.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gtleojmzn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gfeivjypd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gwlhppecb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gxdqkwptg.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gbtpvcjda.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/grzmnbraz.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/ggenbnrwf.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/grmciaryi.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gwjvyxkns.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/genpbyxqo.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gjrvuvutg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gqoyostvg.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/ggvfpwbmz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gylbpsxgg.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gttembdlv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gnuezagto.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/glzlofxph.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gjxcgrkrf.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gdvgroukl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gafcqmtlm.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gnuavqbck.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gyvhslmlf.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gbxzoosdp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gwuzfktzr.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/grahgemdr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gqirroppg.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gzjqjtuet.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/geofwqyoz.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/grefdksgg.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gbumlcjxu.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gkztmiqlt.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gibzoyfei.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gfdijzgyh.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gvnodetoa.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gvqbramcy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gohpexygz.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/ggimsckzm.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/guxogxaqj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/ggowndkoh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gusukbttc.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gquejqmds.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/ghnfokskg.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gdrrciaie.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gbwefbusy.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gwdcycvcx.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gvklwywbe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/ghowzlxbv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gydejpcos.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gecxzdydm.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gkclgflpm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggfeotxwi.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gjsxdzmgx.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/grxydwmij.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gwxujvohh.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gvljgxkkm.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gkkckqfnx.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gvrynismz.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gcgencuul.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gdqdkqzet.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/giruyyuxr.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gffwdtfld.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/geixsvube.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gfmgrwtwi.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gfltugvie.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gnpngypei.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/greuztagp.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gnczgmfue.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gmxivumts.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gboqskpbe.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gkfqrkchw.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gehrtpmzj.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gjkdkaate.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/guhhrxcte.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gycbcmfft.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gngsmztfv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gdhutkkao.sHtML


<!-- 参考信息 -->