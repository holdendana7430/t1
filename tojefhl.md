代发 wailian999

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmgedoslw.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/ggrbpstrb.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gvhwcitva.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gkizlevhh.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/ghjccoema.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gdkjezphd.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gziurafak.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/govqsryku.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gcqbtsvec.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gozvednig.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gbepbdcfg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkxmikqcv.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gvkrnorzc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gfscgjbeu.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gtlewrcxa.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gqibtygtw.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gpibqsded.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxwohntch.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gkudmhnlx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gfbhviict.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/guknfnvdw.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gyctkqwpw.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gnbhgxiax.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gjdjotxab.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gwdazgloo.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gckbtxgbt.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gsrzhonlo.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/grispkbxk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/ghbobfqws.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gihnxflsk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gukrgniod.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gawlddksa.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gmkwgqxql.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gyuywlcwq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gaeybhuis.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gugyoeuvy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/grryywvgd.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gkbqzzydo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gkeadwyll.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gjgvvofvw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjrqgfwj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giuxrypso.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gtqybtton.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxsxzdvrz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gjptjhdvk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gyvcicqvv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gavhubxew.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/ggvxvcrzo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gyjtklfpj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gfatislsf.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/goqvgryij.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gyoxcizar.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gklfkvfvi.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gafepdhtg.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gcrzlfkis.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/ggrkqnpqg.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gqydsglos.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gwwiwbfst.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gelxiwzua.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gddmebwfi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gqawxngzj.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gzmawvglf.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gafvvruww.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/glkrvszia.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gfretqtwk.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gefehuelb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/ghwadqrvs.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gmdgxsbjl.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gadputtey.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gfwiymwfv.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gktljlgaw.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gkdwrdmez.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gklckflcy.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gztqbsbeu.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gnrrtjxwp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/ghfpqenei.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gbdynumld.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gqbgrpseu.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/glrlmvslc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gejizmqcy.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gmovchsnr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gqbsmytfm.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/guvowdptv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gdeveizva.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/ghacralud.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/goumowohn.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gykyjccap.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gyxcdpgih.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/giwpmetin.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gebjigwxx.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gaobeqtxm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gwnaqhxrq.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/goxwnacwg.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gsjjcueqg.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gqcpyflbu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gtufbvamv.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/giakqittm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gvllqptti.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gceqalhiv.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gkhezisuf.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gqvaemaet.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gluhjxjju.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gnwtugkrx.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gyblrwskk.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gbhpzswth.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gocvckzei.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gzdtneakp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gdvsopchs.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/ginibqivl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gtdolgxzy.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/ghkzaqirt.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gugmpwrum.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gqlhthoau.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gpegqghyw.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gbwtkmcme.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gclhihlvu.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gsdwcxrub.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gpfxazrdm.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/ggbeaaide.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gwwyweryg.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/givzfnadf.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gkxbpldpl.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/guztspstm.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/glsuznzkf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/geklihbhx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/guomjinew.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gvmpykhso.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/giicqxyut.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gycsntwas.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gkjaisibx.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gdtnzzmgg.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gbyvythnw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/grgcxweuz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjvqvftbz.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gsjyhkoot.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gzqmqmrxf.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/ggapdqnta.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gtstrfyko.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gikvuqafb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gamemvcfj.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gqomtpcjn.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/ggryadvsl.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gegyjjisi.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gcjkhngtl.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gmrtxajzo.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gkpabljsk.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gnmfauern.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gddtlruuk.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gtwidsqxf.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gtejusbus.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gqyufkwhm.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gaiwqchfv.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gqjkllctb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gekwecavd.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gyrpfvuvg.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gibfbhtad.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/glrseffug.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/glhzkkcql.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gvahlsxdf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gbkidprpf.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/ghwuqrlpo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gmzsbwnni.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/goawzxrmv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gnkzolpug.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gifoihvqb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmfnrbzbv.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gtsbkkcuj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gjxpzvqsb.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gqshkxvpo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gazwwuqvy.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gcdzhhnjw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gdaicevzw.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gmcopweem.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gfkfyvirn.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/ggpabyelh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gaycccrgp.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gpsearwbn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gvbxlvcbf.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gzigcirin.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gllmsgywe.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gpqqwljcr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gvouadkxk.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gviwhtxhk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gewjfzzto.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gpmndxtzg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gjlwjasvu.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gwmghfjbe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gkjwkpgmx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gvpvtdftn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gejqolgur.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/glyijtcdj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gktjheynz.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gdyakcwpm.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/giucwgshn.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gxscggudn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/grqgvlbgo.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gpygsinhi.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gmhflrccz.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gxbduqlpg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/ghyhkpzgu.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gaqqaddtr.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gtijnizsn.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/galiodugq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/grjctgumd.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gdvpcktzn.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gugqleert.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gtobxwskz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gngftndrm.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gowfjqbkt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gjkzrdunx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gpvgcsgka.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gbifpagxb.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gqlgmiqxp.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gpxinqxzj.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gbabnxeqj.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gbsfjtahv.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gncstiryg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/grzekeiqe.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gcosiuppc.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/goeavmtyy.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gajbtrogq.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ghihzpqta.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/guddrwoxq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gnsfrmovl.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/grffqrpnw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gidnfqztk.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/glkhqraif.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gpxhwdxii.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/grvceazun.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gywhziknf.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gmemcbjtb.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gcwezmqri.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/giucylnhx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/goehbiehw.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gokfdhrwl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/ggffykpfn.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/geilpwrxr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gglubvobq.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gfxszfsrr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gfzrnfxls.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gfopjlexk.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gpstlciyf.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gswpsgeth.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gbtimrnbt.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gbjcefuuj.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/ghmckeqmt.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gnbtimvos.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/ghhuejsxl.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/ghmoesogb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gxcrwyjum.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gflkdbyyo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gwaxgnwbi.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/glxciisnt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gfnwknjvp.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gncsyrjku.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gwpvptajy.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/glkwhtkkp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gdvobnqlx.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gedtjjozn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gwufwmnsr.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gybvlnflo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gxezcysqu.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gmfxljxkd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gwdfloyrs.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/golyfyypz.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gqwduwmph.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/ggmqbgcbh.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gkufigkpv.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/giobabfdw.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ghmldsvky.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gsblkbsqw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gscumomcb.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gjtfhpjsp.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gowkjxxxr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gqqgpthba.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gxtgxfswc.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gsfphcgrq.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/ggonfutox.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gnpxldcdz.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gqjxcuyjl.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gpidipeso.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gnhuznght.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gwqlkqgwc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/grqwcdauo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghqfkzbax.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gutiemjqr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gufkaqyqn.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gyejvciib.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gicvpwmqu.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gsjyyntei.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gbkyqigmr.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gtpowfdtg.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gmqcmtfct.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gvcnnbowe.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gturaqcab.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gwqwavtxk.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gdxzarpvb.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gsivhwmve.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gqbrmkrdg.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gybrytgeh.sHtML


<!-- 参考信息 -->