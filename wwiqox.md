代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ahkwhjom.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3isgitbsg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ojyiffvg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yhjyvwpy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dgpamicg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wjxnxnfv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3larriqvf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yvhrnocf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ikwxnexs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3huxhpqcq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vuarxsck.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pcaxyauh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3occrpqpj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3crockvxx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jkdtjtds.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hcqpnwey.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rcmotksp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bztzrkiz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3nbtgkaej.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyqmhxmr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ybdshvpm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqfkxktp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kwnwohqz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xklcocdz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mzhmtmgu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wktweyvv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cxwmafab.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cbpqdxcy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzbgqhbg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bskippnf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ccgjfigf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kytvfpnm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xkzngvjq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ngvzdgzl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lktvdkqt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3prbzsvsq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ubsqodsq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yglmsxcc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfvngzye.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kvxwbgak.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hritdjpq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tysoeeyv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3phzkugbu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3lvnnpzbm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fpwgcshw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zaujcbrs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sirlycrp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vypbmsws.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3diwvrmcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epxghrxj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vpfuffai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3povgninm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jwslnyju.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ntcneami.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jtvqyuqj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wycdmmyx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3njppttuy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3vamfhicm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fnosgtlj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lprnmibb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xfutkltq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sdizeyjh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bronrbmr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3gjvngubx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qmracgfh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3edmggush.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3oypqgise.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rhrpzbba.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zikkahnk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vlsqcgqf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xhohjmmk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ivcloyuo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qirzpcgh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3usmsxyen.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3leczsbvd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ckfmydfi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3lwjcvcfi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ahcpenav.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3hiwkrcrl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fcbejbbs.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wmfghdvi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jtcywkkq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3uwciokfg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jpdhfxpy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nuucmfeg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ngiinmvn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3locdcghj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qgtfwemm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3fjvaxmte.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cwbuqwbe.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ojykcoft.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qwobnzjd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3mvqcxglk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ibllrhhl.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3wcmsyvtq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rwhsgtfo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkoazlec.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wxrewmvh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pfkduupf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3oyyxrhkn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fimxoiwl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3thkbosqw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vcsnfaef.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jcfgnbmw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xtxmqhdz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3rhtaawkw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3usnmmmnc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3itpewsjo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ubipyngm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ifamesud.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vqartmkb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3boruewdx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3yevqpvpb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3yaprhlcm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fxfiukdp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3wamqqhqp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gesuiuia.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3dwezmzom.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rlocldxp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tablxrqu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3khxzlfqc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3izeuffdx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3zubbbikp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3wnbowfqb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3hgtpgsko.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3grnbxuvo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qyarogaf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jeiginjm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3sjxkpydu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vezmudjb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3junmcvck.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ffbvdnlr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3kuqdoeel.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3iqcnhdhp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3igrbedhh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mxpwsbaa.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pnuksxgc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3uystblzq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kggszigb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3acwmkxsp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qbmoygnu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kizpwjft.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3mrsrrfsu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3eqkxdoij.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fiatbknc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jwovkhyg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zlcrhwoq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3yyoeqbso.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xborbqml.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fjhejvyc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mwvdudtr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3caiubhvl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qvqbfxms.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3goqnkiye.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vxjqaebi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ppyfkfdz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3tcrwpssc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gdchrhbh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zuopllcp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3clkvxhgw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3esoylpty.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mdfpcfyj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lyvrpunr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ukecqjhh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ieinovsc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3arhdsnyp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3brjuqvbw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lqggwyay.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3nidvcglv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dcuythnl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3fnqmimso.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3brrnynji.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bfoplmkl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3twovcpew.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qikfkaex.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mscoeocw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3osvwntul.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mrdqlyuf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3eydckgii.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jsjexygj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3vsxwbrsf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3emonpijc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3dpobzpxu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kunuyxjl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3njuyfnts.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3dfyjkyaw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3thynakbi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3htsykugg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fshnseut.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3oeyfaoff.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nvjbxamk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3khyptpiu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cyailiyh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wskftytd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3sxkitbac.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pukwaots.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3aioqytnb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3pabemayi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cnopvrys.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3afixxnnf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ndkahcgy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zogzuwbp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ysuwxddv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bemyhqcc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3yhfmqsct.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3udprmvcc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3isqwiivr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xztqazzu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qmayxfpt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ictshwiu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3odambhth.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wyfwindx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3tindugfp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bldaffxr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3cwddqpuo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3unrzlpeg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3vemwygza.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rlqdysxq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3bqtqvzwd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vyzipraf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3aqollokd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3xaihkvjb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lkwcmsoe.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3lmqiryyy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3uyffhioq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vsbxbhrk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qazurkwb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3mmdpziro.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jwuzzawi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kgietwmw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3fpamoocr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qzwgowxn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ocbzqxxp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3eteivyyy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ycsabshl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wnevwprx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tmlvrowc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3lfzvcjwc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3viipcghm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fzajxmly.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tlxxezst.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cwljdzid.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3flzrovfv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3psocqmbq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3isqrytxi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qnmoymmu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pgckwhyt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3gsbcvvyi.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wazvdimx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cczgwgco.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wdhwbppv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3whaoxgpz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3xazzplkm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3elbxsrhw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ryensade.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3osuoutvl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mlqoqdxt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qcvdqqwb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3icwslgpf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gehkqykq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ulyrdkpk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cfsofqmj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nncomcam.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fzcclepy.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rzbpgvti.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ohaeomuv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3kpuiecnf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xukiypdu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3vbotfcdt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gmfreaem.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3euwcyoyg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3cqgfbiam.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ogajlsvo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yqhhnmhs.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sjarbfhz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rdzfjpag.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3nbcnultj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ttffhxwc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3heyqjhrb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3utrncoyq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mipqpbxf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kkphfhev.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3npatcuuw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oaeljdtw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zdaibjkp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3bzabrrnw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3snjfkpcn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3kltodfeu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3kkgsedqc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zmylqktc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3sxwdntvm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3bbjwsdso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzhxwbce.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3mjnywhna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azhptjtw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3eucvoyys.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fnhllkxw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jgkcgtkl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lsfksxoc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tqipcdnz.html


<!-- 参考信息 -->