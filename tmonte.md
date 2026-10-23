代发 wailian999

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ghivaemy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tkxwchxj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ppllxrgg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3srmaawcd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ptwzcdxp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3pifnlgso.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sasyjpya.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tzkqsyyz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yaotejmk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3szylyfyh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qeiwygjf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmcblbdp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3otlrvjxl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjalujrv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cmqrizgk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmhhzpqj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ouytlgyt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3akefrmxd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3iawodirq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lydhkyaw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3guifgcap.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gflncnld.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3huhtrenx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3femeeiuh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjdodag.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lxxenttk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3itopmahe.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3uvxlozpb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nkjvsuxn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3awkdorhg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ovwawxwv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ktsylkhw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3dqjuzepj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hqtiurja.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpgmfqgk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bzvzbmqa.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cienzssu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qftldlvm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ylyvcmpp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3trkrzkpq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tdgjrzeh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3whnijmxp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3auvkzhri.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3glywgmcu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3arhacdrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfcepieu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rzkbkfvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qntfbqkj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3mqsfexxs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3upofcmfj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gtyvskyo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vyxcgudf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3oxzflcgd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bfczkeok.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wswctjhz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zxivzzum.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3zuzdubqh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vingxpom.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dchhoxql.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3trgdxawn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vmcgjsgu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ejkxncrk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vlzqohvr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wmvjedhv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fcmiseuk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3nwpnfhmx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3caacymtc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cvltsslx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3lfmtzpct.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ohfrkkjs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bhqursbi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ezfpjacf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ytwvnepg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jrygmhaf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ciadcsjg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mjiixvvb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3imyfemrl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3hsbrniwh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3kdminpye.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lgpmssvk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3sfeqhvtr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3psgnsuad.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ibkuvxbb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lecqbopt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3quciatjq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3sgsrmdnw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hvpfeoeu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3esgdlwmf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3vjcahhdh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vhzikmjs.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3phsprfvu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3efoxvozm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vaxlqsuz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wjlwwexr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3grablbwr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qefwqskn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3bjhblrcj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vidsfbuo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nhygvnyn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3oljahgdk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3dktowhcb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wandntyh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kgziltgd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3liqvfkbp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3qesjfkty.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ezvygitr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yibghtda.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wsegfspb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wnodgqlq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rrrnldqd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3syxhisns.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3yxszxyyw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3repvhsfv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lknzvndk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3uhpvcswb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3dkuocbzi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3aglxduvq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3omvkmndj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3algaxfkn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qejlxfok.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3bczrjskb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3kecrkqrl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hmjylmvc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3inyfypul.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3oejpganm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cnlmmxor.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3lysonwvj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfhmzpgu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3butizgfi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3spuflnnf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3nfdxgrmv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3weorczin.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3tvxmpksn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vrmrugqs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3dbxlkruv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zacsokzg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3yejdnrcy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vpbnxdxs.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jgqppiin.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3duuhpodf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dlhdijhv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3dumeeeec.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3edgafizz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvgdsjzw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3imdqcahy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ugrhhqyf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bmunrgba.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3apyogodp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vxmvyoyr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3eizazbvc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3upvsubay.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cmdynoic.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ltzgpfsm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qxwsnaag.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wfhvlxun.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3duyspwyh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lvmxituu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3sjxnjtmt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3aiurbnrc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcdxmis.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xlpojebn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tsozzybe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xbfwgaeb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3zhtmelhu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zjhfpilh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tgvjnczl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ojnbbteb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jgsxgixi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3tkzxlsmc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mchlqtpa.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3odsibpge.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wekbleph.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ywpznyft.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3oyphibsk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lsjglnpx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3poekmviy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3oifffooj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bpmapmvj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jkpxvdeq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sejxewue.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3knuvncmh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3iosulqxk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3uvdlwsam.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qeawltwb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3spiyclva.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3tpztzcvu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bjgkbmzz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3elvhvahr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uqljpcvh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3alfiqjkd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3nmrbifco.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vlegiuie.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tpryiqwi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dleykpmx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xiedsksc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3xnvznocj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3cjylplpq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hoiykryk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3msndkdyc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nxzkdbhu.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3vdmrraqb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3hvxficin.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3spxsiztk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3zxakxaki.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xrnkulwq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tjwtydkg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3sqevnswy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qokscmzj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3minveway.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3psrwjgto.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kwdzaean.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ntwjxahm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jjfyxbqg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3apoocgrg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3etnjbivu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ermkouop.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vzbcmrdl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ahkdmxtt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hyixbubt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3gjptvgfw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ummmgdtz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xxcqvuyf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3aptgtzox.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3tvnojwqs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ivmgdosm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cwoakgjg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3txmfgvop.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fypqenlu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3sbigvmht.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3aglemqat.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sgxffjqz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uxinquhx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3plrhdhjn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3axyaortd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fqshukvm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jaklzqpq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3dcjefeip.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xwdyxcaz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ucikmoqf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yedyfbmb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jhocvwsf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zuxoplma.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3hbmvqqzw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3roxbirum.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3qkqnfwoy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3bzvxksmd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3dxfjfztu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3usukncjb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vwkgqzqa.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ywjuqxwd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3kbnrdide.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nshzjyua.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ykdpooqi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3cuwmntol.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3lhwnnemq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3miobsyys.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3clcivqbh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zcllberk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3viilacyz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3nospelcv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xjlqyfwq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wkbgwqdt.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3bfcdzwqf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3sbbztiln.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ibtkmibu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3llpatlew.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3pepxxmog.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lnkmzwjx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nuawkxlc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3flwitahf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mucmreyc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hptxzgzc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3cwsxucak.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aapqizdu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3zixvvlmx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3omvvptcl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nrjsikdx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ieytqfqn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ydryqsol.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ehjhrgap.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vztgvasg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3qapuyzwy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qnzrrzbu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3mznbxcjz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3xssxuorb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3zhxlzupz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3fguqjdxj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3imymqlij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvwopnsd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xoqtapwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkuwuqfi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vqzkznvg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mtthrcuj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3weirqxan.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3zdvrgfru.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3avsdufjh.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3adzyddrw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pccokccv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uzygjvay.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hlgnipje.html


<!-- 参考信息 -->