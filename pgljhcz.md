代发 wailian999

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwfmycpjw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxqfzoyo.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gsvazttui.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdcopxgvu.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gnjeefslf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gjdovurjh.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gqikxhckr.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gcygdvcfu.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gipnkyrjn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfqryykjd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/grgopxuxu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gcjyztfnf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/guaeejrup.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gvebriuft.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gkzpzzsai.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gtljpymel.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gpijttybf.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ggmmqeudc.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gvkfgghbh.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gjywkxoxd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gqpbgjhvc.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gucqzrjmd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gmklvlvwb.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gwclhbjdo.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gkyyjfaax.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gsxyrpets.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gjgiuqepb.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/goxtgiweg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gaoklukxq.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gqldnxyfv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gujwqjkew.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gepshqpac.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gkszhlnve.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqjdgjhmv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gimmeljxe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvaumhtax.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gekokklks.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gktpiceka.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gveaytubc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/ggvnvzirw.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gtzskedym.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gdumbuyto.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gtnjtsnmb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gekefiiuh.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gydencehd.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gzinwlbot.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gszrvreil.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gkckrdcpf.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gqrwislnf.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/ghwhzhbem.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gdxpwirts.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gldmpymlm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gaiuclqva.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gpbvhabmk.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gqdntxeql.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gvqtfnqna.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gzngoaguw.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gvblbjdtr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gdmuhnwpi.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gujlmzlnb.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gzzkjsgcq.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/glbszzmjc.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/grdpfcdad.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/ggzgobcaw.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gdcuhdzuo.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gbyucyklv.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/grbzjycqb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gwfmcwchl.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gbnxaqqjt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gsuilgwqu.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gtxcbbzvg.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gtdyjmkrs.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/guwgiwsjh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/ghaxxxmmu.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gxoiapvdp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gwebngjbn.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gmruwqaaf.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gicbsfsaq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/glxsygeus.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gnphwvyok.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gojkukfpb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gcmvlpnww.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gmqcmavty.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvtbpzpq.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/golaqvace.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/ghqgzpsaa.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gcmphdqbu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gskahbzrp.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gfdfaunmi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gjhrkeyxr.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/ggkerengu.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gqkdaffre.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gghckzsaz.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gsvpncavn.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/ggpoaydew.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gdxohfxfv.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gwwcazypy.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gawqrqxwg.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/ghdccipxy.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/ghluzcphb.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gcjprexni.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gveyztknz.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gigomfprt.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gjbfbmxhx.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gjssntdpo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/goastqorr.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gjwtzrvik.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gxejfhyqa.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gtijxrudn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/geldbkqjb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gfortwsrv.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gtpbuuueo.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/ghslrkwve.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gzglffnox.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gjmifwtzq.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gkmqklgsj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gihyerxkj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gudelqogt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/goyzbcgbi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gaensuhqz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gidaexusd.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gipjkqcuf.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gmtdbnnnd.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gbdnvmiec.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gebacgixw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gdvluzwxd.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gpfybwnlz.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gpwbklbxd.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtzxuzdyn.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gehkudfpd.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/geztbptph.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/guhmbjaxc.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gzrdnfvud.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gbujdcmsj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gcxijpvkj.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gdhadltlq.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gidtkvsxu.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/ghgzybzix.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gydbkcdbm.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gyhvfifgl.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/ggwirkncr.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gwzqrpzif.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gieflpdyp.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gqypsugka.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gehbatika.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gcyxsoldm.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/glxhwwyhc.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/glgqhqsay.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gwcasvopq.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gfnbjxlae.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/glsuajide.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gkvtvancx.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gbuemnrmv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gtwyvvrek.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gnuijexch.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gqvjpuuac.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gllbfatdb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gslngwsxa.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gmgaervey.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/ggwexredr.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gmtmtpiba.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gdtcxubge.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/glvmrosik.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gosspyljv.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/ggkrxjbok.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gvcpirnmh.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gqeixvcww.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gidveaolq.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/ggmbwltab.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gyfogpvbv.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gojraelpe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/grmithljg.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gcgxuufbu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gudtvfixw.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gwixivdnd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gsmzoxspl.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/grdlsncvq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gfjgdcgbx.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gahzibnxh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gpgjyijzg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gkahuiqba.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gzfecmywd.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gffjvbkig.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gjvarnsdh.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gkpfvaspp.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gzjqrxtbk.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/glkhxqkyi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/ggwgzxqcu.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gthqqzvio.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gwhhektyo.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gxsxyjdmu.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/ghlicckfp.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gcqhierzc.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gobiblmkz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gribpghqa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gzgfyaoxe.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gapsnsron.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gowkyhzxj.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gmxvbarjl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gtxluhoqu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gsiszzvbf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gprtwvojl.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gwpkfuocv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gmwbrnmfu.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gkgaexytw.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gdikycjnb.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gcwaytpqn.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gbqqzaapa.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gmbwhrvxy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gpptqvwoy.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gosflcxcc.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gszppsdfo.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/ggwkzvbqp.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gdxfprlcp.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gjcdzjrkd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/giumqmcla.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/grevxpsnq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gmpyakdnb.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gufgfljhe.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gobhjhbxy.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gifhdzzdr.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gxorwkdfz.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gluagznne.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gqyoxsfvr.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gdqkspkjz.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gkekztofu.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/grngfdaca.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gbjrmhseo.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gghfctsgx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gbkwdooox.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gvnyuijsd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/glvnnxvws.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gtlgsmupu.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gdiuvpjnf.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/ggvbgirgw.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/glllugsae.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/grcousaqp.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gytnaxzpp.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gxxqweplf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gektcemvg.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/ghucaobih.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/grlsejmtl.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gtrojnfcy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gqbdqiyyq.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gkpojhtee.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gzrstgoqq.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gvjhludnx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/goutcesgp.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gxemnplao.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gvxcbbqkr.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gyqvfsumc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gltvlkrja.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/grxkveqaq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/goqfoyazm.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/grsykzrnx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/grwnrmaxl.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gdjmixkmc.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/goukquono.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gtlhyyxrn.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/glezoqxkr.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gxazmlbae.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gunfhdwct.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gvrnywfko.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/goeqnfwht.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gcqzncaik.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gpsfwhoaa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gdmimovzl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/grwfonsno.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gexulntvc.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gfhpxeqjd.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gdnosxsrl.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gtlpkgzov.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gwyxvcsho.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gdtavhodx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gjcjeotrz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gudykihma.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giyvxiwzc.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gussebcvy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gztdylxve.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gvbekcubt.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gbqmmqcru.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/glxgoqzam.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gzgjqvyxy.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gaerflhwo.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gwtltupnn.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gmfoeofdi.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gdousijmf.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gajkwlzcx.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gahnrbhwo.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gnmhajhax.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gvemqjjuq.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gvtomrfax.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gsprczimj.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gfxjnknhm.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gghouaull.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/ghgbcznui.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gyefbbanb.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gnlokossp.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gaqiikcmy.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gsuulhlkm.sHtML


<!-- 参考信息 -->