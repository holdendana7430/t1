代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cbcugzar.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2dyekwxbk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2xzikpgki.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2znerkozx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vsmpgvpy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nzwuqevq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qtohnbsi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fulddeuc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2iybutwfx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2scaxbwal.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2hurtpbfi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ghaacooo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ytgeiyik.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bldwlupu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fqpripta.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hircafgi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kqwqonji.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2vhtjitji.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vjgnzmwj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2hcklhhoy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pwvvvugv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2odsozkvn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gmhjqqml.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2aigpguxp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2isfaecjg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2uqbubecg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zniwgfpd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wuujmkmr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qjsxuniz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2wmrmmzeh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dtvqhfrx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iculuoyw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yjxsuccs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrhcowct.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ejtvztks.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwajwfmm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2cnettaxd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2dbscasre.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gspxgacs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dbjovfyi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2qjocvwyv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xnkheljy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qemrgwcx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qwaynvzl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2rwpmtrrf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mpevfghz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qoxtmqth.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jfqpncin.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ozrqpzza.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uhhoglyj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2napmswnw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mgatlxee.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbwzict.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wqldalds.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jezqvwot.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pzeosece.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dtpnmory.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aipzixac.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gstzyfmj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mmbuplga.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ndrnxceh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vemdmpiw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sotfmvao.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hrvkwdda.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yxzsquog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcdlcmvj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2snrppmkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptmzapql.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dmjumhpa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2unruvntb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2pkvdmanw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vdaqicuc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ryeqwpwy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2oskffatf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2eftlzlnb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ghkyflwb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2fylrumge.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wiutrnsd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2neqtprwz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2cntxiuiz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vglhxmyg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gtyqbmpq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2wmkiweam.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ptuvlszo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2haonqgal.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dqvrxkvu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vrpwmiym.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hachoman.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fayymreq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pahycwad.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2taxrpvae.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qxaowgcy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2frpazojd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2syxbmamc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2twptmygz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hiuhqpnv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jiwizjmi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2plujaxoa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fqzaqjde.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cdzbguir.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2aoatheos.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mfsytdyi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fzeudbwb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qkdmhtmw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zphknams.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ivkhtzqh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2evaqqqvc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ankgkddw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ttkjuwru.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qjkaqmaa.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vchkeujh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2obtgarkk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vzvjnytc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kmcdefzk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2sjtzlxyt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fxvvaddx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dtyymlfq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rdhmnfue.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xavjflhp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2meqspozy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pjueljdm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rmutzhnr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pnhykcfi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nidrjwka.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2idxnzpnj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2iquwtfua.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jkpnyaps.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uxsvwoye.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2piixdtvp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wbttblvr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2yhahutjn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2iwaqqcni.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2tmygcqdx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jtrhfshl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2afprgqmb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2tmdgjean.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dbkggymi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2aqfnsdgi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2eoarlzao.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fxfcdteo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fmaygqdu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tfpxvwrt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hmvxwasq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vtzzrkyj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vretovoz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xhojeyge.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2aufqjhsz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gfxsldod.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2chncbcyo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2qdpaaxpk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ywwefwit.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2itvppigt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ncmehjuj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2magzvodm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dtqcggku.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2lofmifjd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2qmxgmkth.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmhlwhnq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2plfqqizz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tuxpbqlb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ixqcxnzw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2yjlvzkzg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qohnxwgo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzcxaljz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2oaaiqxxk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2viimfzyv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yltguutu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tempyuxl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lfzmxyli.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2capgvgld.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dmhntbxu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jhmctofi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2zibsvjjb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2mtzbzyxm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2eebdjyjg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2jmdtqnqk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kbcjiorf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oxuqqhtc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2arthzypv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qcjykevg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kozpexxh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2cbbfxquc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ziwsegpt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ttbvyxma.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ahhtdxhg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mfflwurc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2obspifqq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2npuihfei.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qwseieyf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zrragflu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jxbtrfag.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rewjcsbi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ailyzkoo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2nfwhhyhr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2skfjiyid.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2igofyuwc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2cwhabknt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pyytxgvj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2lluutfpv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2anqwpnqf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2cvxpedsb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hdicnvup.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vhebnxjm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2fonscxvj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ahxafcmu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fdlwkmte.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2coutbxnu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2qeuypmid.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zcpseiug.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2aasnxwfl.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jghscnbh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2mpdammdm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qlozbnes.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sqoqkuzz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ouzlzmhv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2btqjmtmp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2sdqoxmyn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tjgnlosi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2quovveux.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nynuxctl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2rskcsdxy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2muujpvrx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2blzgdakl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wejqmzqc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2xndedbqe.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2biqozlew.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2daovoyao.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tyhlswfp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2omxgatco.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ahgxkugz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zrkcfkxg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2uqiceyyh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vwwcfnsm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nrjcdnhc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2kzlxnjyv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2amsnmxbj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qqnnizfr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vbzfwkai.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2otjkbrkv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2aqeamfez.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tdqfbuqv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2vcapnneo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wyfzmnnb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2jgdgloou.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gtvjdjbb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ldcjacul.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wrlxlhzg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mazjejju.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ekkfldnw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2nzvifpwu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2sqogpakn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2frslmhdn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yojulvhr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2edvswzzy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tkhogoat.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2euwkwavh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2qsvxuagk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pdjeacqr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ivjtuojw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmjgwutn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2usxkrxaf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dvkydxsf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2npfnejdh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zgsweqgq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2pjxmevrr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fdhgmpcv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2gajwyric.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zaluwbqi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2odxeworj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2neqbpgrd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qukemxeg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2vedokxsk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2whovtnwv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2fwijtqgb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2oeahfrah.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ubslshra.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2uvsxrwib.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bzmsvtrv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2evbvrfth.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2suauepwf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2uoxipdjj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yztrijrt.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2iihbgett.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2whobsstk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2agdmfcvh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ewrvzkjp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2scydstyz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2lhsojmeu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nodlwmyp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2piwiyrnk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lnpxrpli.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2khduzvyp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ysokypeg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gpteqgip.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ffjjgqci.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ljxipunj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zozagnqc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xijlplne.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ebdvrpsw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oifioqfg.html


<!-- 参考信息 -->