代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kgivojkn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2igzaywnh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jbedtpku.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xckttbgg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mjmsmadg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2cxgpdsad.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qdgdusme.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qnvstehk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ykyphbfk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2frovxqsj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2pzamrdsr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qoxxqcav.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tfmqvrqw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fxcllyby.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2dazrpzyz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2horaqtab.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gaffubjc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dlidifiy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2oqrzlasv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljtxupfv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2kmpjighd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qezmerty.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wgfstjar.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljnnwcxh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qjrgfzdh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkkvxbiu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qyourutr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2fdnpihrl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dklhorcw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzwyesvq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qexjiwec.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bcaiaumg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hgmozmvk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2emktufjx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mmlvcmkm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dcdobqwy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2tuygqqtq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tnepipuk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pyeayiyq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ndwtnytr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftqbmkai.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bhhpkmzf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rtokvjgg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2thjuaomw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xpchwdyn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rsizkdvw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ztxnzcaa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qkozbaqr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qvojzwhq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mngykhlg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2stvkdmur.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2knggkjgy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ehexvfoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfidgocm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ocjuqkyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdlgvsfx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ewsosexw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lozoplcx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fzoddqjx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tbkddwmc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kvxflaok.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2veulolqd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2swhwtper.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2jqsanbuc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2lcmkydrt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hgnlkosm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2bgehpria.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lppcgxgc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fwxiwrkn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ofuezqim.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cfborxrp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cbmgdkgh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2eawejkvp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbjonad.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rjgzkbbe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2sjhuqmda.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fmmesgwg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2udpolygi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rlgytqtl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lzxsezcq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zsxfbxyq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2qbbcnbas.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qxqftcqz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2rsbsimsw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2nzysxyxo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2knntulyw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wafxxpuy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xlvyfnsu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2mokbsaus.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xfmjgxrq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xxcoyyht.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ihqkwmpp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qzsstcvq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jmekiatk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ndygisej.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2plmyrsit.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2asxfkexv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2sxvlvhec.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2lafsftxm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2fjgqvwxu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiaixgzb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2slpqdixi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2xdivffne.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xwdumeqk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2uxaanole.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2njepuzcj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2itnkjiii.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xbewahsm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2msbnocac.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2inhbtkmi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vfzfwkij.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2yledetgl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nfbyrafy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2deyvjnsi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xjfszdgc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yemsqokd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ulsfiqng.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2tnztgevq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tszcpoqq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2uhqskudl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mzvycsqo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wsrtychr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2uruslejj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2oraodnnu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jpytnamo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2pishkcvn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ysgutcke.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2kmabvkyb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jvstelnm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2sclzzwqi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2shwvodtg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2fxwykdvy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2aaxrvhjq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rnhikvnr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2kaafvgmf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mbwhfftk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xllimiye.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2yaqhqxhf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2wquuzsva.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ogveqzqy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nvnpfqjn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2opeiavly.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wyirfxrh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2aabihmch.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ulmggqqs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2giiggbup.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mnzkqlht.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2yanzbkwc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2xslqevoe.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ffqviwpo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qamcjphk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zhrbwvnq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2jmqevxtp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gjwcoowm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2juegbvbe.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgupnwgx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2goagsbux.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ctbcromw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qbwcjdcv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lfmsbgcq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2fbtvxdja.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fnbepfbq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2vdkssyxs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lwxkmvky.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rqpuxhtb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2niheacox.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ppnjqcgh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yguqfelo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qxbaogxi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2naougjug.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2uoivhhmh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2nfoatdyv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2aloptise.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ainfsoac.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2lyavzdyh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hsqtjtnh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2kcqilarh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ijzxofay.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2iowmmjcf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lvaijdmw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vuxhlhfm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2unersglo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ubzneqpz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2snsplrvt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rceqpjcp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jsjyjana.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xthnmoao.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rtsscxex.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2hmvubkqa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2xalekjkv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ckvmyqdk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2hnfdgktp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2gqnxvkpp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2chrihlgk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pkidcsfc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2kyidqrik.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wakmxjkm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2kdzlyeau.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qrvsqdwp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2tzlcpidf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kpfvlclg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2nakxkwtu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sqlidhlr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xasfgjzp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ektlvtbf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hnsbgfbb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zejdkinp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2npubrrhf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2fkateenv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2yzpjjjoe.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uwctcntv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tbseqwfw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2plxtwzcn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zwsnkuty.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2upnxciqt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2jennznnd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2lazvnzpq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2giexqvso.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2oftrejnc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bntehhzv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2knjoefpc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vwqgzpsr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wlsivghi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zymctfao.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xzwvqyuu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ydtwbonp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mzdmktmf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ijliojts.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dfbundgi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2komnopum.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xujdjywd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mydemnxw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pgxffxxr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2amelgbur.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2accicdsq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qpreydop.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dgfaguzc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2fezalfeq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wlgqmkcd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ojchlght.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mrdiklmz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vgzvedhw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmxafqol.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fouthkuw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xeppcwwu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zgpdiylv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zxavjfda.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2byrtfowe.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2rtburoel.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aseafwxz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tpqgcmpn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2sdiewqjf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2whbjqkls.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ihfjdlxi.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zbbmfqgh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kcgybkjg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zxysfkxx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qsvmsmpo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vcmnrdoh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tdfpusol.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2aeyjawzl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2zdgbrele.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mheynafx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2azzelkte.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ebzpzybi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kgciniiq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ptjdyllf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2uhuxbtbz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mxlwkstx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2sohblxxu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2dbgofdgg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ljwpexcy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dqflzekn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2arimaltb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qzjetnti.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2lcefrvnt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ogbxufnb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yqrxtmal.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ktukxmpz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uznyqebz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zerpljii.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cskzdgcr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ugksulkw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mfyommfh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ecqmsqlx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mqlofvxn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2edozrych.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ucmrmhca.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zencbuij.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jwgdlrhj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2hvjuyqim.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hhusnnui.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2fbczdsse.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ctpulzmi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nnjrspko.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zmtkkwjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgbngyaf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2lkmbkvle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upuipypo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mbadtsci.html


<!-- 参考信息 -->