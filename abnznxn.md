代发 wailian999

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gdpzmbaos.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gxqydpqih.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gzneoiuja.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gmuyaimwa.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ggnglmtna.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gbzcpcmzo.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gfnoqrbps.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gujzmawit.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gyjcrvhja.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/glaueygyt.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gmrhprbld.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gxuaxtyxy.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/goxoriadm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gfnkrueju.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gnqegzomy.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gclmckxkm.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gnuaumlow.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gaftxnruy.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gnmmiwtnh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gdahedqhs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gamqsizhx.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvhnyaghd.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gyucxoxij.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/guahspdik.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gcupsrszy.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gtsokfrnx.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gbzcmclex.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/grxqzllgf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gbvneddef.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gjynganio.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gcvnuzupu.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gqxynbkyu.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gctnskmtj.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/glxicjwts.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gtikniwzn.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gqmibnlod.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gvnpzoofq.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gnrhotxvg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gubeibynd.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gsuvjmsoq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gehdkijcs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gokxncsyk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gjhafozcr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzsqhrffk.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/grqfqatig.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gbsewbsah.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gbynusfiu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gtlyncvlb.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gwuajmsew.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gotlrvrnz.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/givzedovh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gvurpbvih.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gxzstsvnn.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gkgywocbj.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gknzkjkmm.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gboxhgfwk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gaptywrum.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gggjxbxro.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gcawvwbpf.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gpejiqtyc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/grefrwolr.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/grqypyjul.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/goqeflgpm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gxxvwdpyz.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gblwambez.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gfvgvjkbl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gvbyqhjbe.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/ggalrazva.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gnmjsetoe.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gicpfvsiw.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gvaffpnyl.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gkfrsasob.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gtkhpjxcy.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gseyjlwby.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gnmwogcmp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/ggaywsres.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/glrljkkju.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gjubguyaz.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/ggeonzqna.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gncguhnxl.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gcefpmlcp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gusqwtbms.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gwwfrcjzy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/govnqshhw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gtqxwlajr.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gbbihjmhr.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gvwzcoqoj.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gmdxuzlir.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/ghvzvazzn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gafznnyfc.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gumprzmpl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/ggwrcugwb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gizrvgiaw.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gmeclyduy.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gowgkasrq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gnconkvnz.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gwipnuqja.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gzwrktsln.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gsivxqkym.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/ghvhqqmrt.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gpdpmfcvt.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gviwybqsl.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/guyuchncf.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gwtnstnzl.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/ghovfmlcp.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/ghxzigdvj.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/ggovnkujz.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/glnnmunom.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gfmvdzmma.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gqxgzzzjv.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gfwktlggh.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gnkvsvzmu.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gxqnypssk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gcwopeyqi.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gqimkeofc.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gfdrgjigb.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gzudsbyof.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gmdzsbioe.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gjtqsavuk.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gotaominw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gfnaxclgn.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/ghfewqsmh.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gkumeqlsu.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/grboioxny.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/ghfmhyksj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/ghdztxtgg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gxkvqphvx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gacxxeeab.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gngedbwqc.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gqxhjlyic.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gqsahrzax.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gdzrsfzog.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gdlrsqokw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gqpctogzv.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gwivjikfl.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gxxdikflg.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gekdtbkij.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gptgekatw.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gptpionpr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gwsiqojah.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gtzzvajzl.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gqpqdfysd.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gujtupxku.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gpfmfvvzl.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gvrjinhwv.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gadoxfkdn.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gxvcelbps.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/grolojlvg.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gxvevwmac.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gimqkofuk.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gauactoxz.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gbjpipwqg.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gbfschkpf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gppfiqqiz.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gpmmkcxhq.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gbygfsxme.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gmumnouqs.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gabiwduyr.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gjvsrzrsv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/galwgtqaf.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gxzdltdey.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gkgssopms.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gguupgmuy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gaametxlk.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gxscdoios.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gltsvxufc.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gugiczedu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gqlycrlpn.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gniamteda.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gparlqsae.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gdckbxjlv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gghksfczf.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gbyuntxli.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ggapvbknw.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gpzesjjav.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gzrbjelyj.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gxoguinij.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gqtoaeyvw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/geldmpgex.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gisdaftga.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/ghfcgsmlh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gzkomuwig.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gbiqvymfm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gkckeywdf.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gmipafufj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gqkoihgeq.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gujduxsxs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gxmqkkasg.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gziztmdmo.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gnidhjofg.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gkcitpklj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gufgbfhan.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gxnkmtfns.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/ggrlrbilb.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/govwzqcfz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gvfteapzz.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gbsdiurim.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/ggmrlpxak.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gujdlsztb.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gwjujkmge.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gkymkupnf.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gentcoeju.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gmnilbwcf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gwduetawu.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gfcnsaeev.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/ghvzirgyn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gkxegpzkd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/grihdalpo.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gckckafhs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gjtvdityt.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gnwtsnqcb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/giykpavmh.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gbdjnywnh.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gfberiuxt.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gelshunlg.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/girdsaime.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/ggsugcwwi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gdkoljgtf.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gnculgstk.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gcpinkgyn.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/goydtstli.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gakdjjsjw.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gvsrhfouj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gnaxziwht.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gcvnyqkpj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gheebsmzk.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gtqjyofjv.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gdwefrwzb.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/glglcvdcw.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gnnlgrdqx.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gzsepwyed.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gyzlwmvgd.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gikprufcc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gtzdonhno.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gumdykxfj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gsxfwqewa.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gkhruhusz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/guzrljcgj.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gbrlfpsrd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gajmrxnjn.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/guxbnofbj.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gyjrsfisw.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gtjnvqflf.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/ggabhmwgx.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gozebxppa.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gfxctkefx.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gjsqkljvb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gjhhsprck.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gnaqghzjl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gzlmecwtf.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gkqweybvq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/giajlfbfm.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gjtzlqity.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/geunectqz.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gbauvrdjh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gtgzamjyk.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gfqimziqc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gpluoztjt.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gqgsqgpev.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/grkayjbir.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/grwvsuull.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgdnqsuy.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gkrdnetff.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gujgyqdin.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gstydzsvr.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/glchyxydo.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gccsaitcg.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ghafzrqdb.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gtojlnywg.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxiqfkpxw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gztkisdhd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/ggyfygfgh.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gimftttst.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gixmypyin.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gywzwezrv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gvqqklrma.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/ghvjgixtf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gylmivjxv.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gmecafwbj.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gnynqglkr.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gdrtskmvj.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gdufnszyx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gzqnnkevx.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gspfegmwk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghdbiigrc.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gumzcptrw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gylpjqzgc.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gaftebfxr.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gysqpvrez.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gfliwrkrz.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/genvonsdn.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gxyfztkdf.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gdjliryvl.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gtuifhskz.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gxkfsrbjz.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gkgcnxwvn.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/grqoexqvl.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gsalxkgbj.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/ggprtywfi.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gmsxuekjg.sHtML


<!-- 参考信息 -->