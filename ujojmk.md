代发 wailian999

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lyzxkdju.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ydrfsncu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qeubfpfv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2yxyeqiqt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sgjprqsq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cyhmqans.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nxqxrtoo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2bnlmlmzy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2csglvxpx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kwdrxujt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2kwlstjei.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ystmpiyl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pwytvrcp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ilwbzqvh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fudfchow.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkwsidfm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2romzehbw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rjrntivh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dlokewck.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bocxwfoi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lwtzwwha.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2xewupeqc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2avctercu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2xlkpgmqy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yzfjjfhb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hawehxwy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2irywaxji.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2juoobgjf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nctzclei.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2cdatdrvl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2zejysrrf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nckcowtz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2orthxzku.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jmwihsjy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2htbgplzh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lhdulmbh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zsrdrwjh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ulrmjpki.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2kzosavdn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqsakrvd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rbsqfqvd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffhparxf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2joqjjiil.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lcuqpllo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fnhkutpq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxtpffvc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2depydgmu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lhdtefrw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2avcdfvvr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hberojdw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2duytmiqk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2byvxipxr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yhbcihch.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ksdrbusy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2drjxbced.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2awjwkrid.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hwbsclvy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fpjcklsi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2eeyhtfms.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gctijouo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zbquqzaa.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rsvjimll.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2yjxnqmnv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2thcalhyo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mntdgyzw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hkyxoqfn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wxbiakzn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pybgbkbj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fozzxffl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gygfbrac.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2byacpitg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bmsysbeg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zlymwrbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuxczibs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2clqsimip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipkoocta.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2idwhjwfg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uxddetbj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ebdrtdoa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2roijfyaj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2uthdbsxt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2oufvpusa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2dqurraoo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hzxlxyoi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ayhdhlwh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nnvduhdj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2driaotvq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2imgsfnql.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2vwicmgxh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2zljnqofp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cpadpqqd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ayoxfbpk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2beibrnxv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qolvyick.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lgysljeu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mvdmltfo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vdzjgnay.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2iguphzqu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wnvpxizp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cpykhcks.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mgpmiuss.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rxwraryz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ulrmpydg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ssatdegm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bosrfpzh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dpaullta.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2lpreuaqh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2sjmhwydo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2remtwvxd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wqzzyssl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rueazuih.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ctonlmyw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2kkzcbmji.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2magzsudw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ajuqbjao.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2tptvyrbu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zzwbodnt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mtoeunpz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mlrztocw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qwigdmha.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2jmyxzeiy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2poeetmhe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hdnmuzpc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xungsnht.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2hpelwwdt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2cwhekcmt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qvkubqwy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2kwgzvuvb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2sejshgcc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tqflwvmg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nlojiihs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2cllbxumk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jesctybq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2zgxrghiv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2yvfbcmoy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ujtmehxp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2usakdxgf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ctpknyxz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xogjcxpa.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rxixhxme.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2snskgxnr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2qeffhqeh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2clhombcy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2grurzjxj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2snzexjpu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nfldtvnq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ggdaicuj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2lvnrywhi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ubrjdsfr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2oijzxplw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rwqwxsme.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2toojaicx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ufwndibl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2orpfeqhg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hujncbmy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ofkgvepl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nqgonaub.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2glhpembe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xmswbnyo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2exzzbuap.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jjgeuqam.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2sbakwvtt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2thmgojuq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tecufjht.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ukjswfsk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsxnyxre.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lgmqulgw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2rwyrekgp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bckhndhw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ufnxduxf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2buagybdn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2cbumrulh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2sduwoaje.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nyasocbg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yyikbyaf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atzwbaxm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2dtvxtzpi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qknojrro.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2drbpqicg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zbkrgwjl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qakdkpnr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bhnghtoa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2nnuyvbnw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2wjytuklq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2rxoknsje.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fagmphil.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ndbxmhdh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2icjmubdj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rutrbsou.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2sywxopnm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ewaqzour.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2snyyihuf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2tevaccfu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2phzlvuqt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2rultiqfa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ygdglskt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2kevbdwdf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kxwxdmbz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2adoemrul.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ukbedcgx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2muckpgnb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dgqcibjp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2pdmyzehz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2liuefdpi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2dbkdhoyt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jfwrkjbs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rwkbrxih.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pwfllkqd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ufkynurj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2eajwgwtj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2chhktjbf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wyjmpnly.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2isttkjrv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xonevbmu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2likajtfh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mtvdmecx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2trwcpeny.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2totzfqsz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2bcxzekoj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2hfokcohq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zdkhwdsw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2oeqkyfxk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pvesdhjv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kmzwxtla.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tehxerkr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2vuurhrup.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2lewqgldf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fxwcbnsq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2waqwcuza.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kzamhljj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2drxzeewb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ckiunglj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2gempgcdw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2nnddzgyo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2vrdmaxib.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ozuotart.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2sjwlbqkl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2awtjrdhu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hzpwdzav.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2atyfkqfu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2fzxslbdt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kflllmxf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2yiuqjtjy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tvowciks.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ibbnxoeu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2roxzloxq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2zlflodim.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2okvblnlo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sdexwhwq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zhccgzlf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zayfeoup.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rzktfltj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dsgugyaj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jumdvozs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2tzwkvqas.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2atzjcgnz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2abjmbtop.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cfiogrxa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jmipvwde.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tdftlpxq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uoujhtva.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mjjdqvbu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbgfoyqg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2sktzyxaq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vwczjxra.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2drqxovnn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mukbstix.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bwjexiuq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2djaoubzk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pxrvcvzq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2pqyekflb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2nppdacyj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zqdzmcmh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2basszayt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2vllvzzgy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dphxjcvk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2bsspskes.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vurpdkhv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2yhzesipa.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2owcdzslm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2kthlzadg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2sexpnlup.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2esjknwsy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jjtwabuh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ruqjuhko.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qskxyiww.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2afjxytam.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2sqaimnce.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hiafjquz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nivnfyfa.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jimfxwxh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gnxerccp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2aejphfvr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2irzaugje.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2armmhxnd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kkfwgxwt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2avbbvxhl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2elxiulxy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2tmndcjgu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xuzwqfxo.html


<!-- 参考信息 -->