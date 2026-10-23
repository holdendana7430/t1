代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nzbxmtbp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cloarsgg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3lhvxzbet.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tnwtojoo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lnijkmdt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xxjyxkko.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3saqyzdmc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3jylfhwwb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3sxretaad.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lvkckhna.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lebfhtfo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3knpvdspw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3mkqazfhk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3njghexzw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mpbzgakp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ymnzivdq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qfhyufpv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3oblcfctk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nrsxexpp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qxwabufc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hnaernmy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tknmxxfg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nveghfbv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ibukqtdy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cfqilpzz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nbtgsydy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dcexqfee.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mqqixplr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kbjaaxsm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3afenjqex.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fdryzwpo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjmrdmzw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ztwxhlfe.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jwwfvjfw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fbhbzrng.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3yclizicm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jqixnknx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwdmrtuu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3fvicgswi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gfyvhixq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aoezwlwh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyhmyfrp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxseebvc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hrhkqjiy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiackgro.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pyoneenb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rzjuxydj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3shfodsyc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qqiomuhz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tpnazinr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lpfrzsom.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wecpyuwx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3glpzveak.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fejkvase.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yfgxotox.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3uozhrbge.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3coqmytlg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qgqclgyv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3paaxeutp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3srlnrglo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3osrarrzb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3baingkpx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nrrxslgi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mipzipts.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ajasrlyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkeejtjj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zqomgxai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsspeqaw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xkpvqsyh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3pqzrecxm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3yzfbutai.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3amboowqp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kfcuqsqp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3apmwewdy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3lbgflqsb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rubmdldc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ptifvbfz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xojdnkby.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rixruykd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lydxaspy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xbvqjilk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nrgaldji.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3rtcepebw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3vqkmnyke.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3oywpmgvk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3rnlwmorb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3skhpibwl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vafxucyr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3clxlmrin.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wbeyipzb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3cxaygllh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3cpjnvamo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3egxfumyy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3keyhytwj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3biinasnd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wdhnezqc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pnpmqoxi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3udqfjztm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3axzbvnnm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xlyehmll.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xfegdwmn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wbibewxe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3kooamiow.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3drtvidyj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tuqowxrl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3evstozbw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rzfyagil.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wsyzgrft.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ptqlrmzp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3howivnwd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jrkznbmn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wdtartmn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3clopdtbw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rmrumigz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ssckdrgi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3upyhaftw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3etohsziu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hecinjpr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cnpzkxxj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3kcrqwqxw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3juhgnfvv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3roenlqjf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cdbuvgsk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zknfawxs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3uhtefzdl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qnnbpgnz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tbwrtaqj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ooxmgngh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3onunfnuq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3onqcvbgt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jdlogjap.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3otnqkkbz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3tnydsvpu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qsccwlsx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cvgcjabj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wfzmrnpq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3msdpeqey.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qnohzpvt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3gkqtvweb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ntqsrrrx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3eyvfqven.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rvmbghhm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kgefsxnl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mnuxciqy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3foxiryxb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3twtgklii.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xatvtxms.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yywqerhr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3kniwbujn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3souylrll.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3uoeprwph.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3dqtvjfim.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xusoeofo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3egsvkfry.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jyevvkov.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wxzqeyow.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ceynrlwv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqdbicyf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dcqccsep.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cxceidkp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3yxyhywnv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3yiwuqybx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hrxsxkac.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qkrxqeyc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dojftohz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wqfjekqr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3unatlgvy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3sdmvtqne.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3yezhmmfr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3gkahpyhx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zgdhkjrg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cugngkhd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3yfqgeohj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3dxudkjwo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3pvwzbilu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fagkxpgl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eqcjpqio.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3sgpeyohe.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ptrmzifz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qbilehpu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dkxsphyl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ndfixbuz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qkmvbgub.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yjbhowhg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ulyfqghy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gnrsjyln.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3exgtnkuo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uugsvffr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jmceqony.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ktddejjs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3jwevaceq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wdroivil.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3shiauxmf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3dzsdbzbm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3kdsvqdbr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3htyvtxkb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3twbslzql.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dhyyxpab.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ywqbzbmc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mcoxqyvz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3guprdzlo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wqpfjvtj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hfmsmsxo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rlihuiqh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3heqxzrxd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3asgmagtc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3shogpawx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cnhlotht.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3umjjdgrv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3znbwhgci.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wzblkrqf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3slsdkrdy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3klttkmgm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3axhirvic.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qqlsxliy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3msqljfws.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wyvwzwhv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jfzjtafs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bqqjlsra.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xjndbyji.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ohvxfwsm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3oefdcgwp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qejmthxu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3nbeyovwk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3dovzmzip.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3kyrxfcze.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ioqawpin.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pulrjgom.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cbvywvmy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3uzmotzpu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xhdhwohv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3feazvuay.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qttpaefm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ofvbfcbl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uagjzjkm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3awpmloto.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3twcobpsb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3aybtynnz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wvdtxtra.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3crugmwvs.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yxenbgay.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3afhtwlfj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xsjqpvxm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3bmuwtzth.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ydaylrse.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fwwsbzkd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ltgdmtyg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrebrzz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ycdvoxjv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rgtlsdrd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3hucyggxy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3agzcdyxu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bmqqdmxa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3txecugpw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wpoylyql.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vuxojznb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3bfofzthb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pwtohjiq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3uypdkazm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrepdjsk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3zsxoeatj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iflomako.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ffarrsqx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vunuidmy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fhtsavel.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cdgylewk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3zshumfrf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3nfeoupop.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3uudaiulo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3gcbxhwxf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3eyjzlyyn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3reoxtwrl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3iczaceut.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3vashsykj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dfnzwcuy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uuehzmod.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3iqfokzgd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nxxtbopf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3spwvthnk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zpdgsina.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3taxgpjqa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rjyqnnjv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3uibtyksa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qeznfwqn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3unyjsitu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3soxmugko.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3mjjipkdy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mdbfdxxa.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xgdowpbc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wjwzaizz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3znyqlzjy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sqmkltrs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3tgczqzrc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xzfglouk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gtoxnfkv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ntdljtud.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mlipnnpz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ukdpsgta.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mwmhrqvv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ziamxwph.html


<!-- 参考信息 -->