代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dtxftnef.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2seujubpj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2lbtewnvy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tylnfesa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ickyzclh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2edjltcdi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2njbhejvr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2oaceksbo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ttirvqrq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kgfznaqo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gzlbhkpu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2oldtlwou.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qsyjrrtd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qassgxen.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ncmovprl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fagoutpn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gcidmxia.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ieisieuu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ovujkswc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rrdjnqra.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2walfirvn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zmugeroc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ugutmnmg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2gzfhtick.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fruirqtq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2atmgrotb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pllxajsi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2wdmytize.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2chwomuwr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mobaerax.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jvjckyqo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2iownglyt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2leoivxdl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kqgxbfqp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dgshncqi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2olnsjohn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lcpxcdcg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2kdpikbjp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2btrhwciq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxrzzvp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vwabrajw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2zaigpfvv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2swybeafn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ijgdxmbc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ipyxxzvn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2gtgplbbk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2yogbrvls.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2cierurji.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2rjadjlxx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uoacgclv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zpbthvse.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yzvcoiqa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2rxmxdyer.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nvfwlggn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lksmvcmy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lkwoejnf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pwofvafd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ebywpilk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vqrmoorg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fsomqydd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbcqwuaa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dvpkyauf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmenxkyc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wucqaego.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gzntpoya.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dsgkqjqw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rahrtsyq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2fxardzql.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2krfcjssa.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2twntxmsb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hrxazjme.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2iqxpumam.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2pxoaqins.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blbibcrb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zbadcxye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqcrsoau.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tnzxvike.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jjxmqocl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jnwaeemy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zzrovlxt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2aektstsq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ousjobln.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2bqjubmxz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2iorpssuc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gbamjbql.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jvdozjvl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2zrewtqzn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2flnfpuaz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2kgbvokul.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wuvgytfw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2oluykduf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ubjpvlxz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2pwqszqln.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2yynqljjq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2sqrzssmk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2eayjpffg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dcappgvd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbevufy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2loysktfp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gnqpdgxs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mjywrivg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2whjfyzov.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2wrddavxv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hwpwkobs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yruniawz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2upqsvbtm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2cxaezjri.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tyteakdf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2cqvuxayj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2huxavsbb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hkmiaqhd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ijapfyrh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2feywtufm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2viogitzz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hyfdxwfi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xbghhasn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2bhfnkbvj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dvlwelka.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xgretbaa.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jsycrqgt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vjkjosgp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2grtzcyth.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2uceweyau.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ajdjpcnu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kgnztbdt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ejfyypsy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2sedyilyw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2eilqypaa.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2mvjoojir.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tlbzracl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pcpuyngg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2igkwvveg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zhfbqosj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2epgdhtch.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jikzeapc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2aevalico.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2awqehkgs.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kccomifx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2baipxkhl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hxejuipg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ogfppuvz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qljxiivs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rkakpjky.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2muwoodem.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2icdtuypg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tkbkckuj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sqeyayvv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xzghshba.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2trdtfjll.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ptrngucr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ykutlrnm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2mponadno.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vylicajc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2srdrogtv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2wfbgjmju.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2skgtdmpl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2bmmbiwhc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xeyhpyir.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ubjhhbxf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2geexhjie.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2sbxeypzt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2apuharzb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2tjxmqwcj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2yzlwmwar.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2txkflrzv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ohkotmye.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2tkxcukwa.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tfiyswja.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2yzswjumn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2dufhjcnb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2covfbmks.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2fltkfsjz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2dxajdgwc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2lwdcwcwu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mxgnohwn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suorkcjn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2kihvvbqf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2iycezhvu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jathsmha.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mxmossgw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bhnqjcrs.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2tgzrngjr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uvpeddpy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jarsqmst.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jffxucpm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fuqdqltr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xqilmovx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gcnbsqvz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xnergjdj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2badofsxu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2izlxgokd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ayjpohjt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2bumxqhlz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2untiwqyp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xvfroexe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2sdqovait.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2iwesddxa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nfuklbet.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2rtnyipzs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2xwrcmlws.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kyizaldc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wikehxlq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pkkyobxc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2jepefzug.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2wgiziyba.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lyxjgexf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xuyyohpv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rqxiwbkk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2dgmozxke.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ehyyamba.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hcxfxqdh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tygsknzo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dmikskai.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zztkvrhm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qqepkxxg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2thjzsqcx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ncnyefmq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2gqegveyx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2cthwyiqp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2rldddkhb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2flvwbbxk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2gzpfgvvf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sjeflsjn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xlpnuqmk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2vwsjcfic.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2krxxgucg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xjurerzk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2nqhxqenb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mqntyigr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2gaazmrrv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2trfhnftn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2kbvdplkp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zskzvmew.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jljboefn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qrmopbut.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xnemidhj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xeitlibm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xmekrjbg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2igsasult.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2bbcvoecc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2kzhtksdz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cpnjikno.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vcrwwjea.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2sbjccnus.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2sisyvaet.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2pjthoppa.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fmpielll.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dbsuobiw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2krjndpdy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2yueyokcc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2voeehxqy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vsyczjaa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ldynqwrj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fkyxxmnm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wlavvpon.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lrfdgguh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hbvjlcib.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xlphnzkt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wiahtuwy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wruacnww.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2rutxaqis.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ubuehmye.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zdctakzg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2movnkrje.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2tyiyzdvy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vhyactpq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2boofleci.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jidfflyz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2tcahihkl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sctampot.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yjussqcc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zkpdknqg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mpatatve.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ozzhcsuw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2hjhvtbfl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bnhnpwbt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2mymnfjal.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2itydzyhd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2zgngqhzf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ebanbcui.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2kjpanbpk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2cpcufxvv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2fipoxhyq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ovcduvzh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2guutcytu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2qlviuqpr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2brnhuqsf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ilnpbxyu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cxqxqtrq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2chogbcxj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2rvhwxcsz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kjawkekb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mrgujiug.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pvnxzknq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2qybsqfwr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2orpavqla.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uszedzvi.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gddwraav.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ysfdrrgy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vgprurqz.html


<!-- 参考信息 -->