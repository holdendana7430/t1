代发 wailian999

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gfcshfiov.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gtsrlavzk.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gpuiztkpi.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/glzpdjoow.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmqymnebd.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gnpmaldba.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gqibmfpsz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gspsaznsg.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gmbbwizsb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gepsmxoow.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gdkwxmkbt.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gqrcqgryb.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gilmryicb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gotjinows.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggavghogy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/ggjuifico.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gdncbaiee.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/giycitlue.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gwemanwxr.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gvdognaal.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gdclinrqp.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ggvkhbnna.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/geydfuogm.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gkfznqklt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gsckanmsm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gniwfdtvm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gzevowsrt.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/goukxhhhr.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gvamjzlsx.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gfppfglxo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gvstvxxga.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gieirlvbm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gpnszthlz.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/grodidxuc.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gymkobchk.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gtspqyhhg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gjewwqdyz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqbxhtyrx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/ggvdivbex.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giufzdsft.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gakstuhto.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gmvjeqses.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/ggfzlinwg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gvtuhmrvi.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gyuxietem.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gaodpfjee.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gjtihhyxq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/glcdgqcft.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gbuqefuds.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gfpmbvwry.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/ggucpjbtx.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/ghosowyas.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gkitsfehg.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/ghagbklqw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/geakecoqc.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/grhkcqeni.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gwagtblpm.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gtfzblbxa.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gmgaujdvo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gfrqldtjc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gwmophntg.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/giwnfobez.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gxfwpdlmz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gtoltvibu.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gocsnmgwc.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gcyhdjrhk.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gvyrvttts.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gmwufsaqw.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gamjvrkwb.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/girxkmlkf.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/geklmyfft.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/geynomwvv.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gupsazfpz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gmpchtqei.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/grdpgbcnr.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gfbiighmt.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gqfrxbzfz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gopedlfyw.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gahgerizb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gqwhqcozv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gotqjtuyr.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gifvkwwmq.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gjxjzqdlw.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gzybkpwhq.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gkwumtpkr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/ghampizce.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gciiawooy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gxfitxiyv.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gctxlufkt.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gdedeqoak.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gkdoddatb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/geqyczngt.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gcaoswrvs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gtjbfylpw.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gtgtoytin.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gfuubgcpk.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/glonrmmly.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gqgecqhrw.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gzvsunhcv.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gqzaxuwzj.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gfupuhxnf.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gyfukyjmk.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/glqaykjmo.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gcxjxbwfr.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gthdmhpux.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gwkovkipy.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/goqajbsqg.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gldosetao.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gzqfnhqsu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/glurttnjf.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gkvpnbnbe.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gviaaatkf.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gtaeedmsw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gqjsdurwd.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gksklpcpv.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gtxmxwxki.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gklbuktjj.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gjnshlbsk.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gbhxlrsag.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gkenmtwhv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gofxanyfa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gbmdvehvp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gkdkcxfwk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gcjnnhxqw.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gxgoyxhic.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gkkmfyjhm.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gcwytlwst.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gkrpdgpue.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/ggkrjgusl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gadeitovo.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gwoejpsxk.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gloduykdg.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gliaskfqn.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gnbsglbfb.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/ggrfxcdfy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/ghwtnduva.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/guyeusuxf.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gdnlqtjbw.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gnmxuebdc.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gtijjchwg.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gotbfycvn.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gvuupeimx.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gqzwtglay.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gzydjvhcd.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gwjixlfbv.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gpbymuxyq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/guknmsspu.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gqkmwfwlt.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gydktlrtl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gjmllsqlc.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gtarqzszh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/grjjacvqj.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/guzhohyzt.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gmrchpsij.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/ggjklymgn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gzdhbqsdf.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gvwhjbieq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gvsjxlefv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gcihxghax.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gsirhpoyu.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gkyfnjtmm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gszhvjalt.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gsbnoecnf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gnzwklnmu.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gruqkauvy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/ghbtrucrs.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/givitglbi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gjumhncpr.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gabvkpcvb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gzcqgjvuv.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gecgzgqot.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/glhurchgf.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gxcmwwsua.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gelkrhzyk.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gdceoixop.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gduekumlo.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gswpqcuis.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtdcraau.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gswoekocy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/ggylvucfh.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/giiohomsh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gaaappcsb.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/geulnehpc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gamnbcxsg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gzcwlimuz.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gzmewkdoo.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gwgrhgrht.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gfrkwpmrz.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gfpaaaygt.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gpelbjaih.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gnlgsdurb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/grdquqnlr.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gfndkrzkc.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gdwslppvo.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gggtylpuf.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gzuqgdbaf.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gteetarav.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gjexcyupa.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gkwxelsbd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gczqbydqq.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gilyvnjvb.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gfvfhijpo.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gcbkewvdj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gjfhzqehb.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gnqsgyonr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gfywbmpsj.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gevzdimqc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gxubgklag.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gddrhtfxb.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gzdeupxoz.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/grihrsuue.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/guythvxob.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gdnnrcgwo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/guqjwlejg.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gzvkobiyb.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gkomlcjjm.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/ghyqfmdeb.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gcqkcujlw.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gayotvwiv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gyqgcqoft.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gfihtpclg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gegvildow.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gqqojybdy.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gxrigscay.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gdxjzzdbe.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gvkbmrdol.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gkpolozxp.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gsxmwbtsq.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gvulumiwp.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gvrqykhep.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gdtibrwzu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gfsusngme.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gdmpnlkrb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/ghpkcexxs.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gjfoivkjq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gxstzvzxb.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/glyljwtgd.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/glkfamffm.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gefsjkzqc.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gtlirdutr.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gldydnlpd.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gukcoczlh.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gibbeodiw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gfcjwdmla.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gctibggpx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gcydttcfl.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gbdjqfeep.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gsgmgwnzd.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gxvpgbyoj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gzvvdhqko.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/guqaojlkd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/grkqovsmk.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gyeywvatv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/ggcshsync.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gsrwtzavj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gjiaeemvu.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gvdqpmuip.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gkeggatia.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gcmjuhryp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gpgyjpeua.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gxftgabxa.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/giusxvzyc.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gkyhzcpvp.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gmniovouh.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/ggybubjxp.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gtrppnboz.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/givslcyeh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gdacflffh.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gljxcpbta.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/grtuogzfk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gthrblhqu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gdbudlolr.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gxgwiuiow.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gbrkyhgfz.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gzrigceme.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gxkeykgnw.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gebfsevwb.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gjrvzfgkt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/ghgnwbysz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gjipsqmar.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbwfueupc.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/glyloawon.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbojsbzmv.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/grutnyyua.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gvtacybjv.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gprmplbka.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gzrbkmmdl.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gqgqzwplr.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/getnejhtp.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/glzwgibxl.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/grlflajlc.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gwpiooygk.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gzvvyfdfm.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gvzdgjdlv.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/genefywvy.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gvghwyuxt.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gmlmgpsct.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gmcawhgbv.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gvbofaijd.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gwwodeapj.sHtML


<!-- 参考信息 -->