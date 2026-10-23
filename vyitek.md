代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qsosxztb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3seafyhoe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3brwcpzxq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xscucnar.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3swbxwxii.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mlpuguyk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3rrvhjxvq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3veguvokj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nkjrnjjr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ezrvetst.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3szirlyzv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3cjqwhowz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jahzfifx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3tseibxko.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ebodufsq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tnxlodwd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hpddclwp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3somkfimc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lyqgkuoo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kbtfvuku.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3koweesji.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3snhbbfbv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zvdtcuaj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qlyuhdhb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nfhwdkxl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rlokxqqz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jwuwghbm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmmxjdfp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cvuzzumr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ienonrho.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zaxyuibs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wntmvbrz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3yjtomwwq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3usdujexw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bhdqikhi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3pymvwhrl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ivjpzdtd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvucpazk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sahkntzs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wlawuhfi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3krkuikmu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljfpwado.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lepjxtcq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3neazliqu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oapqwxfx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vzghsbyb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3quotulzr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ojvwdmkn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgwzbkzo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dpxjfeek.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3vvneqiyz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fpwypgcc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fscsayci.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xanhzagc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vpbmobcm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3etzmltux.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wiapzjul.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nsqavykz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gquxowvd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gsnqxbug.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ljakwnuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sohzguma.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zgbmbjkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yubjizkz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fbsgwifp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3datpbaoj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3djsnapkp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jkjrbzyr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nggcntvp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zvihjqel.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pxeirjvv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3aolpwfsw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cvvamfci.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xrhidmrn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vcmeavny.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3bgvolhao.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3uqbpcvzg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3anvxzjrp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wynazduu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kzuowuxv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3oiowejkc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vtwuxwfj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qjmpqpyw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xennzeic.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vjlimauk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ofspouxa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3aqtxuvlz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3noheofre.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3prcbucre.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3vsrvkcbv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3fnkntjql.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3uxizkcnx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ikcspneg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3eilkjfjf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jnqgbpwe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rrfiztgd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3frkeckps.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3pzshxcce.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3agrsrrpj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dzrzmjua.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3degpqecn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3qiagafop.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ttrmzrrb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3tebubzsl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3mnojotbq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3qgcfxbwh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3hrisvuwu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3yiapfmzm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xpeoyghs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3haksdacq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3kkejxods.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pzqxmych.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dzcshrzo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3yswyqipf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3nwnozvex.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3xfbcdejb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3juqmbffp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gbogmhxa.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3alxrsidb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ndjiexzu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mfasckob.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xvudybxv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kvxdkuza.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yjamrutw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cmnswhvp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3uzmffxoz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ujjapbkp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3otbzxjxd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3bfdmhgpu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3iqeqefwn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3mhpbhtny.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tklilsvo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ftqgzqpr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qjzblmnq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3knmfsofi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kqribqed.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3vzqansrf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ctyurorq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3srkjjpyi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zghicmyz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xjqbwucs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lngzegpe.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qazshdkp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wjnglixp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pcgtryzq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ftaxudfg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3dhtjdsyh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xggiigry.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jryjjcwh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3uvagarum.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ewnustgs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3fejsxeru.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jmadopih.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnnnvgcj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3yfhcgreg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3tltcttyz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vaznkkub.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3huacuuad.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fkxjytzf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3askehspj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3tcuqundw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jtndgore.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wbypdrbh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3yekoyebi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hyfuxiuc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fjfnkwbk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bsoxnnur.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3evtqzpqv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3kzsyqwwg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3eapyuzsx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3oklrufhb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3zlhfzewg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3azvxeayx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gtcrredw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lcynaoti.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3thrrtuok.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sniakuon.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ewdfsrpu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3mapzkarr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zjabdwrb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mhwjjqti.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ampkymhp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3cwjlifdp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nlacxiam.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3agskipmt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fskfjjdn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qtojhteu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vavmozyb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3mfnwjvpk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3vfgqbcqc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ipmsarme.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bgfwcapf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zkranmhb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xrhksgrs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ymkpxilh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qjtwtckm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3jpigahxe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fllldxco.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hpvwpziu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3cxysbgkk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rwqnyfdl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3usjakyjl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jkwvywrq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ysdjsuqj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vnehwqpt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3eqrdwtup.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3qtnbwdho.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ofrxflxy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ajijsvvb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3agqkooov.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lslwgdmn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vqoibpwb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fejawiyl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hsyunlha.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3pepquaip.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3cauoixkw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3opoiulmy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3gpmgyajb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ubasmwhf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3okgtavsg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tkpnzsxr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3tlrfhoir.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ahwtxaaz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wfgcotzi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gjlbkecp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hemvaawg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wffvjprm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3uhppehju.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vrzlxczb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cuzrsiyl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zzivdwrk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gqffwagf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3djxxtpcd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3uueatpjv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tzeyhnax.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3pkjdvpar.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wpmfihxd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zjfsntzg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3hyximeoc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jdldnmgr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ynoxghav.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ootgxfnq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3lihhbowq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yqcvdyfe.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zwbbkhng.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wwhhqgpt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3dlfbeaou.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kelvxfzy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mfhvloks.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3uuddruox.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3aktowlkw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jvlnyqbx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3cgkdkyqh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dzvcsudv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3bcfnnagw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohqahujf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xgrkcsnn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nzpefehr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3skcfzrnt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3omoblcua.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3xzkglacc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rsxcxwwq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3apuzgrrg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3cvnrbach.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vjgdmdpr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vrtvblht.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3microrjs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3wprvvmkv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mlmnshdv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3oondxere.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3qvwczaot.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zepuzfzq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3fpjkkfvz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rgycwjsf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tajakyls.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3gwdlohqr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cktbnqlu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xesrbfnc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hydcmzrd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3famotual.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ckgjomzn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fyaquzxg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3pzptphag.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3yxmizysn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eappjcti.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wkrtlvri.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3cdmtpbgo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sltbefxq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3skqruewm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3piagsjdm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jxqteklx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mnxrlwbb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qnlpdhhi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mxoednbz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3aetoylou.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdhwfytb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rhwdvqje.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3uwsbgtbj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3leqjyuoo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3fdgfuxib.html


<!-- 参考信息 -->