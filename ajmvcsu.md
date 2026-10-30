代发 wailian999

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gjeujmseh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gsoqygvmf.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/grvkxzccu.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/guywdfugr.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gtvturhap.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gjacffaxk.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/giiflzglb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/grovkytlt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gadyzuwtv.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfhxwiebh.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gdqksqcmg.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdluamvyz.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gketobzjz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ghfuwdyjc.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gtqakaqkn.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gvrzznqij.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gdxjstask.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gyodmhwsw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/guhmqdxps.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gcellzgbf.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gapvuyzty.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gpxnhbshz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gxqtullcy.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gqcpqyqxe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gbekvwodw.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gyzrbqsgm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gkybqlrlx.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gsnrpoicy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gxpxagncs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzbbgwpqg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/geetzvioz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glmrbhubw.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gpxgjllwz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gzcjikkwj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gdxoygtsr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gqifhwpht.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gbocgnwct.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gmfglrhpf.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gnakdthvs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gpbuzynir.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/grhhuuqxg.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdvboiird.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gmibrutwf.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gifhsiedd.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gzjfmvrsh.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/galsjofse.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gqdlgzclt.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gjkrbqvhu.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gpxtxaohg.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gfhjpmmdh.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gizcxozaw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gkifzffeh.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gmgiutjxc.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gwvdlgtim.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gungyinac.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gjwmvefsr.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gpuyjdtuo.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/giyfrddch.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gagizwghm.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gvdmsusug.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gchidxmja.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gmwjlczcr.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/ghhiplxwq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/geuxxloim.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gbhxlxlhm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gccwjvuub.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/ghzjnenzg.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gaqevqzrf.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/glkbjxqce.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gdfkydhrn.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gmkldwqgp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gfvrxqunh.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gvrggdodv.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gtukwzpts.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gfgqgyyfz.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gmvpmmjzj.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/garabprmh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gjfxcljis.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gxjwxsato.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gfmbjqkxt.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gqngtejvr.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gxlutmdwd.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gauftrggd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gxrelsyac.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/geatbetoo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gwmbhppxc.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gwnrxnjra.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gzbxckifx.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gacwfgmxk.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gdpiwahkl.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gxrkkyzxw.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gzrjnwffw.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gtfnidfjp.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/ggfjvwknf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gnuxcryva.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gczixmjxb.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gtwdzavpr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gbmulkfjx.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/glxqypucr.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/grfsqockn.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gcydpcwfz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/guxhhotht.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/grdcpxdem.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gxgchblap.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gpkeukuri.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gepjftvhi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gyvzbwkdi.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/griexlmfi.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gmsfaehop.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gyuwjzyyw.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gjjxdculz.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gssyjsbxb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gqjktqsoz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gpsixmclb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gkugpggxy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gnrreumkb.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gfjzcircq.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gqwomsfyo.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gwfvwkhdn.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/geyketypf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gnastdchf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gznbxgtlx.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gganklevj.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gsmlghxno.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gjotgwvzu.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gqtvwgfix.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gqlqlngda.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gwkegelzy.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/girxqnwbn.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gbqgzlihn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gfurcqejr.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gwoejpgem.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gdqrlklof.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/ghtfatvru.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gxbhabdvp.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gkwnqrkde.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/giezqzkhz.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gggqpwlio.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gagzvrkuu.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhysuoe.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/glyagkdcn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gmxgvjszi.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/ghwevvhjh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gudqiogki.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gyafzgziq.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gktlehjay.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gqmzlrwoh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gefqiwjvw.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gpkmqsdeo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gcnbyikpl.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gyfjwijso.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gqwhwxohu.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gatdsulec.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gonxzehoq.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gxsyouzes.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gqqsitiwo.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gcplfpjmr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/ghfwzdjwu.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gdjysnrjd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gwgklodxm.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gncutoplq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gcerapvhx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gcippjhjn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/guqhxnumz.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gwnvzacoh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gtdyyamxx.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gjsufzabl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gbxowxmvq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gbzhhlwmw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/glsningbt.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/ghsqcizhm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gvngjtdir.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gldycenxb.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gbslfpccf.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gpywejfwr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gsggzgtxr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gtdroxdgq.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gvbzzmqey.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gkxzwxnhx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/geojgvike.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gvmpnbbwp.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gkyptdsqe.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gvwmfitid.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gfncuqbrv.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gizqmkpcp.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gtkifpptl.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gpylmwcqs.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gkdrbnicd.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/grghlakhy.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gntxhcjbj.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gfmkzjxgs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gnhkvowfh.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gtokwewja.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/geculqhkd.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gsdfiibab.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gmqcsxfek.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gvbpmxshg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gdgvrjejc.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gfsbglyer.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gugvkunhx.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gqrmbjsxe.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gcrhggxyq.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/ggnuayzru.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/ghqtsgnbu.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gswgvmzom.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gthlvybeq.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gcnwqqhjz.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gbwspbcwl.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gxaytzqkl.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gmkiicjxt.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gpltatqtl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gwxscnsex.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gbpubzbhh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gdgarcyjy.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gkzgkitxf.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gwpfdeslu.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gfgagqklk.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gixuofson.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gmqthwydf.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gvosnhlgr.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gscwfllfe.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gjhrqxssq.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gthrcrrpr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/ghzqomwib.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/ggnoummeb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/glpvlhxwi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gddlmnebv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gogrjzyqz.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gaafcewdp.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gyttjllgl.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/goiycgnbm.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gotajkcor.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/ghwyeyoyr.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/goxtirxyg.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gkcipnnib.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gdynpjeai.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gbsjvzrhp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gvnzbdybg.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/ggecprrcq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gjlwxwtci.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gpfdsqsli.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gougtfwrv.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggawwtmcg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/glontpvjq.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gxgfltvur.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gbfspecep.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/genqecqbz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gfiadzxyo.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gkoiptsze.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gzemzlsws.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gtridieas.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gslvbazmh.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gjsjpcggk.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gfhcrqqnx.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/ggnulcfqk.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gvgzxaehp.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gjmrnxwop.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdfkflejw.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gzygydxvl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gjupgdwsi.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gjybngowa.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gjcdwgrzk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gcrghydii.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gwbxgbvjc.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gqdbhwfnf.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gciraxgfm.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gegxtunmp.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gsxgixlhn.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gydvtloqb.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gsdrxjgmu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gzhufgwwr.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gxwohlglo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbmcuuwlk.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gzajmksvj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfhiqcmba.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gtaoznojy.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/guhifbwoj.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gqhykrunu.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gpwhbnbrm.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gnuxodgxd.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gkvatqiky.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gehdofqvi.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gyjodtujq.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/ghsoyrulo.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gqzvssgch.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gdpjwylli.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gtzcusahg.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gtzyurzhl.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gnnxmhdxk.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/glzetnwog.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gkucpizsr.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gygxwxdqb.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gkcaxlanm.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gwaijhxpl.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gzybqtkwe.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/grcfukzke.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gjzsngrwa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gsrjxmtmt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gbhhzqnwp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gohwmdcsc.sHtML


<!-- 参考信息 -->