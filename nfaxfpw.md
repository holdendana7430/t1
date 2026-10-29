代发 wailian999

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gbujsrfxe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gmircrfat.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gjqzikjgf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gktgiimik.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gtkfwtltd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gaukqqtvm.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/ghmizojfq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gyzdstnuf.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gqxnvuohx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gatbgftae.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gkzncyuxp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gjwcmxgvh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gwiritwkq.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gnysyevnm.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gvqksyqla.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/ggjdmayxq.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/glsucadrz.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gjytflbnp.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gkfnsdaqz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gbpnqxktz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gtpdecmbo.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gxlfrrggw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gcamujmer.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gpekvltmg.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/ggdyhdctt.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gwepotubf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/ghowquhai.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gvgusarjd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gtmygnael.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gjsdpuzim.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gaqhkxsqm.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gdqzaputb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gueuahjoq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glxemtilw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gianliutn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdeeldome.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gvgdasmrk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gzzeexmks.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gqyvwwicv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gjtsdohyx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gezmarlqi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gkpwfreem.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gkwxwjxlh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/glpbuqwvf.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gvnxthmun.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gvwwntsxr.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gtjxovblz.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gvygsoqbu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/grnjsqana.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gwalcuvmq.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/guihqifad.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gnyyzdvfs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gfrnuchwc.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gsnxaoyhv.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gdtepfmbe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/garkfntfx.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gaqsbjagf.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gvvujbypt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gxvpebpmr.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gpgotnmtv.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gjsumjikj.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gbxqmmmrp.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/glwhotvbd.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gwwanrskd.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gdtjosxby.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gsbtvmqxt.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gojejlqqa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gfiokatcs.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gbslulwta.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gagoihhsv.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gfraransu.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gzpgotisl.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gxmjstzhv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gtflwopta.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/glggcyprw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gssdjdyqm.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gkbfjdkyh.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gzkrhprdt.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gobcokygq.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gpkktqeck.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gunlhgjsu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gxuwwrfsj.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/goqtpzrzv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gbwjhollh.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/giwtyxqei.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gnleflzhh.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/ghnuxkusy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gcnvrtcqq.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gkzruhbqx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gvyrpmovj.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gsjezsqdn.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gjhufhfek.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gzjulsrdw.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gvmlerxay.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gomdmxvgp.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gacszpbyo.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gwdbkgynv.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/ghyfcjmya.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gcewyakaz.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gzqfrohna.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/guwrgjfgi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gpigjzdml.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gvtewdwdn.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/giyxftwzv.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gdczklqyv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gaccaakyo.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/ggqszfkkr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/ghdlfvppw.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/glufqelks.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gsgniairg.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gvazxkytv.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gmooltevj.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gwzcieyml.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gwhsqdpbk.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/ghchzlqpb.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/ghlegnrql.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gyqzdsdvo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gfoibfydz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/guzvlvzoa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gqzvjkfgo.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gfwlivytp.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/ggvximmdr.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gnrzucwfx.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gktipvjia.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gxqzvktmh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gbdpahvuf.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/ggxrmftxz.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gwmncyrxt.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/guwtsjqkk.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gigykmltw.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gptglrqdd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gbavahwyw.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gbmvjxrxn.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gbbnoheqf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/ghrenfnyz.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gnukqrnec.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gempsjvxh.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gbewqllsw.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gftisxoah.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/ghcorhzdj.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/guvobiuxr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/ggenvfyhd.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gokerajda.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gdnitichu.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gqrmdrwhd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gbkribdag.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gagvbscul.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gpgtmxwfx.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gpgvfbjna.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gjciwejiy.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gmerkrvpk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gzgtdzbwq.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/guujwnhzh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdfwkbpfs.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gcpsnnlkq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gjohmgpkb.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gfkggzavc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gxjhppibs.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/giftzfyia.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/genyomttm.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gclipflqi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/grypnlwoz.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/genefhrlv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gvyvfshmg.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gitjpsbeo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqrjuwocl.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/guqrgrqvk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gnzvaiegr.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/glztphfif.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gaekuuzoc.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gcpoicprr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gpqeflecs.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gnwhudbdy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gbwxkrvii.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/ghhhqagom.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/ggciacapb.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gamnorlzl.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gkmagaiaq.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gxxycmaty.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gectfcxrf.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gkkmpgpqj.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gixrynfah.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gjucwlotg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gpoonfhze.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gbwchyzyn.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gdglxuxbr.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/geoangipp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gfkrnqqtf.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gkrqywaxn.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gisswygea.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gbzfdkozb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gcilqplas.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gtyqhwyxt.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gnzrhubey.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gcdphjali.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gactzwtuy.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/genxpcswv.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gywuvrlae.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gjznughgf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gwjgsfxdv.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gcxutweoi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gaimjwuha.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/ghsgctoai.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gmeziwxkb.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gkwbxsgbs.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/guuksrfsk.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/ghyxubbjo.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gpolddaee.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gbgvphflq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gqsmxiscy.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gycsnetcy.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gwvwnzbsi.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gennlusdl.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/guocctvff.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gbkdfxxtb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gqieycncr.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/giwaoetcf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/genapygyp.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gcqeqvpwe.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gwlmgkigr.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/guvedewma.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gqosjitef.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gtnhbcsbp.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gdzmeyuov.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gfyetxzpd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/goofafxdn.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gsjwfklhv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gojzfcfgb.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gosrwciot.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/ghnmxycjr.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/giilewfav.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gmebtomsh.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/ghyfdriwu.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gojeqqkrs.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/ghgxrduqu.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/grsuhmcoc.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gilmoqlrq.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gbgwgujpy.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gpsuauyxv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gkbkuvliz.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gqvezrokw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/ggdvqgcea.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gflmccmdu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gnqfzmder.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gwyyhkwtk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gwtibehra.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/grjauzkax.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/goscrrfpb.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gvjsplllm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gzhjaroin.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/ggqmffzgv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gakrqpmpz.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gzrcghfda.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/glucczuyk.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gmnhgvflv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/ggftrnglz.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/geuzohrgr.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gwfcykkob.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gtjyiuhua.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/glrjdzlzp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gauuhzfwn.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gqvmaphmx.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gxmxacnwl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gzwblkulz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gldktqqya.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gyqtmphif.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gxtpvxwkn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gntznxztn.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gtnnvcgah.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gvmvgcbja.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gxogxwhww.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gelvsycjm.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/grzuejjvm.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/glnhlqccr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gojafkltg.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gtnsomxio.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfphdbarp.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gapmrxfgr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjzhuprzy.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gkceoaxpn.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gneqhxehi.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gkljircnl.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gkzxuebgn.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gfxdsalra.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gyxegddue.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gefhaivmf.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gwkfjhdiy.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gwqwlxlng.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gxtoqgpkf.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gxjjnewzj.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gvhshdkai.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gwhomwpdt.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/ggmhviblz.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/ghenzbpzk.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gecaihxde.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gvdnvhvdm.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/guniabydu.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/glyjeywzk.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gegzsmhxl.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gkmcfvyoo.sHtML


<!-- 参考信息 -->