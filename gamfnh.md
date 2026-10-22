代发 wailian999

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2olpzwyly.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kwocuxuc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2tlbxrkhc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kmwnzggk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aoiladfk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ytsiyyqt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qffnxgkc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2nxlirnmb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ccarlrdm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2voqqvpch.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vtujnlik.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwzsfxkr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jzfcojhf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jtwiyigp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2myesxmfn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjekoftr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ovuarmsq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqxoafip.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2flwpqayq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qqyexbzk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2snolqnct.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjwqfqjo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hksybcpv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mcqpzoyc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxznbgec.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jrulwyfn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ayswqkbr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ocuxazkr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hnevzzyg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nzvgyhos.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gmtahbtu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2klerwcrg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2toclowsj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fmzqywvl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2glxlszxd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2odubkxef.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ebmanukh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hhxckprw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fgodyavr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mjfgejio.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2acwcxxll.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2emsdmivz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qfbxedyj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hzfrzdky.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ogerzlcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngwowyfv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zqrohwje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2muhpbhta.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2pejljqnz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2cxncfhvu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kntmvvyi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qzebiqqy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qqigtmyl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2cecznfzp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rsljpdxn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ivtxeial.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2potxehgf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uvnjyatf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gezzkdxt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rxvhlxxr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ybfsobye.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dwubyxnx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2qxdadvxn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jpylskzi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2katbrhtr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2jcjcqznb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ygqnjvgs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xdvknjkc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bfzumjuy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dybmabtt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hzwztmuf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ferzyybj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2buvwniau.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ikvjfvqr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2onxofygp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2znwkqgdj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2xbfhxalv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nccpvnuy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tfsnkhle.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2icrgyked.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2cxbweflc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mmfmmtqi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lcyyxgmp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2phkqomax.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bkhoyxyc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwboirlk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2tbudkqte.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jndcenda.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rtsslsbe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2sumzzssd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2sjqgvubx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2bqycgryw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgwpsczh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kknmrvhd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2phqjgxma.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2acefihje.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rkipewln.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2lvkwcznu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2dwkswpdy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2abrjnlxb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rabgeipn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pvwobxxz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2xyaixnyl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2eszybhfx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nqfjrumz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vfmkifdv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2etsbfcfr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kcqxpmxz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ojtxkhjs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2taocfxwv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sstthfnw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cdqguyxl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2algrqqhv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2fgnhwrpd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ttpjwgzo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hefvwosx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xnrbzgtb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zwvldons.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gtjwsiai.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xodkafwn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2apoppteh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vcnaawcf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xsdbseyi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zrmijtxi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lkkwyewy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2zkspuqow.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zwekxeke.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dxazktpw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fhiivnll.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2nocfbmwh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vcdgzzwi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2pbuxvrdh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ftattzzi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2usxwskmw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2qxjbldbg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2puosigts.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lxaccusa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeffsvxs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2rqlnovyj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zmsyqaiv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2afetwhdn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2tpxrtukz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2yeveclnf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwfszjvs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2aegqmgnl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2gglikdkp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xerddgdx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ansrrcga.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rjgvnmuz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ehkzzbaw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qviiyvhp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2naqhvihr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xovpjipr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ftgxqrky.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2lsfxzzmc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lxkyfhjk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2shasjcxf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2niqlghpe.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2phualqez.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oyqjkmur.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nzjwecpt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2sgzuozbb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2unszrfzi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tbbnrsnw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dweoczuy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hwaegzne.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2onnyoiav.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yeqmnsej.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2tozvbgyx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yzwegzmb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2vqpvxwxl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2oqmdfhjy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2lzffbxla.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2aiplmvuc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2jhgoijyv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2atmwzype.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ealjobja.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wstajmml.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mjcghcvk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mzbtgfsg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2bwiskisl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2yrxjijxb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2kbgvduno.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vjeecyqy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2olwjmuto.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ywhbwghf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fwabwyxd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2lkhmyfkb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2snilfowh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2illiflca.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2fjvubvzw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2yrouzgbu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2iakypkyf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2vmwppyrp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yztalbjq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jualqbxi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xuzcptox.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nmdgauzv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2owuzvtbz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2cjvasaut.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2kxxscohk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xygklkee.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jfsknizn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tcsnxtxp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2puojcftb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qwjhskxc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ukvvcvfp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qoxdumms.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jxfjrsju.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2upsaoard.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qeslzpvg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2adghzxsa.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ohdqxlhn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uohvvomb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2eexvsjyf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bydmvvxr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ahbcwdpy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ngbqzuaf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2zyvozvia.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ceevkbnm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2yeyhmrxq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jmymgksf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2fjhmialo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2vddygurh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qsbsudjj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uckvavup.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2cphnhpzl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bhugqgaa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sqyyvsni.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2capekfha.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2joaqrjdt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ipaquqqy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2bhrsqynv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ycfyttbl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2sbhxlnkg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ozrnltel.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mokdmoxo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2wchuaxej.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2yshdouol.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrsyuvkr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2uqvvgpih.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kmjmntfz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2utegqzpp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ssblxpgx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ilsddtej.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dpsijter.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bjyncsre.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2sqjbagfu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2exuwzqzn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2rmtfnwtd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2spezdjhe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2sgzddopw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2aaykuurw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2nozsilgo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2wmbncdyy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oebustcs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2fcsejoti.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2guruslqz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hckzwnsh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qzkdzdwd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lxvgabht.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jwumvttb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2afixozrl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jesyucms.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hoejdsbj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2asgekczf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2xnceqebu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hquwoxwy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2papqkaup.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2iksbtajj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kwpqjaxi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nbfvlbok.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2rcchlnot.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2safopcny.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jkoqygyz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kifsfrsh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rnffcunx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pyzhsyqz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zegeqese.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyrtcvrf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gzxwknlr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2vdcjxghm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2otygymeu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hbyqeumq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2wmfoeudr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2irtiutry.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2nfhupwcg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hrggyeyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwcivysl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2milzeqye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztxxdcaf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ndnbrxnn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2anzjamcc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2asxcznwm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2zjrpoyqw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2uaukuzkp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tososasb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jtqnyrrj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cltshaoh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mmosgrxf.html


<!-- 参考信息 -->