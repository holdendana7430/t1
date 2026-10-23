代发 wailian999

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3mafizmha.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3anutbgko.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aoexibsj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hebkqbtk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3idkseqrp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bdrpdkjd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fmjgjhwf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nvgtmrdu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3kebcjksh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3berobinz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3efodizoj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3icqogudu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bbxyjilc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jrvpscrl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tbwzmluw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rsiqapuo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ibktoqih.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rzivhxco.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ljvdoven.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mxiqioob.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qwhwyhxz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kpdfwthq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mzuznffl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nziphppm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eriujqwy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3poejfgtt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bqkccqvd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xkmdntrv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ajafdwtg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ddopzcqd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3nzoltbxu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jkzkarky.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yxpgbnjf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3olfhoxds.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gnidgzif.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hfdsexif.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gmzvomgj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ssutmvun.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3feumwbkf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3obqdpfmt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vrnqyxti.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rnyehuam.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdskxuur.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3itrpfdjg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3diemnizz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hqtcqemz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xwvusyal.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cgvrxdyp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sjhkzrvj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ulipnaax.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dcksdcaa.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fwhrurtv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ylnzoksh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ziiimrbj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3orzwpkpp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vigbwqvd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hkgrgtga.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ccshoxze.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mbxlsxgn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkszhdtt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3woegtqsv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lohhuiwu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mxcyqnib.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dbtmlcph.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3durfqydf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zmsgxqmk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kdmttpwm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ezgytcvn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3juguqutn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uvymjblc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vhtmcyip.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3effbqkgq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3gztkzlcl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tvsltqmq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vxigkysr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ybvvgnct.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3uyivmjbh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ewhyplas.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3opxikxmo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nczninue.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vldokaoy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ifbdgeqf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kkvhpvnt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3dyoauawy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eaxpjrex.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xbylikcl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nzpxdxzf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dsgnlxsm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ajxyuikl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3drcqfqzh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vtvyremz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hzwxccmw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xfkfuoji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcxaevtb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zldvbyzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdyjkuyz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3oyndmart.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3kripqhwa.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3clnbfxfc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wolojyff.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3htbohtnm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3gmaghgrw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hltyyrjj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3pspofwuz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yqengaoa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lseqwpcd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yzyafxek.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3oeklesqo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mbolpoqh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3gwmxkldk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lmceztzi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lafcwxhy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3yhtirctd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xezqrkrm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3eqrgaezn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3znbbkwvr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pqveiesl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3dmyaltjg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zziwzkzg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fhvgcnew.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qvhdptdn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qcwmllvn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3aoyywuki.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3apygvbkt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3przkbgel.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ncsixspu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jvgdcprp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3zaddfqgt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lekzchyn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xwkpqgbv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lunlrvxe.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yykkgsxl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3maldhuga.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyruvqtb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gsqgxtsq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3pnivkqzf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kkkapbdj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wnjwjmxz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3rsgdqzdt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3obypjyhz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3oesecuhc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wtglahiu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vujgzhnw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bwxvpoac.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zltprbpy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3fvvfldef.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3teylfhiu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3pvsfovpq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3nokvomkn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vdrlfydb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3dxsxuqqe.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3onhkqdih.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yeupidyy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uqpagovq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wfhbnunk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qqlsqmso.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3bptduviv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xzrqbfoj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uihzmhfx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ezwqbfxd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3peyvgwod.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hltceqkr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fjpxdjso.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3eotgomxw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3bcnawtbi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3phogrlaa.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mcpifdbu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zlcqclfj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qtkkuvsk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ptdltbwf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3fyaljwju.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3quilvdjv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3rfgitxpx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3arivdybe.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3bpfxyhbd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tjisvisf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gzurgeip.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3gwmfkynx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3gmoxqrsn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3faqmyhrp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3kmolwqcm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ryldlpyc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qhwrigda.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3scybjcwh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3jrmssgrg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkrukrhq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wtmhgzyl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3maftczsk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kcnqjwrm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3dujtnnpc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rsxtbtwv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3bzhthvux.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fkbhudah.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vftaizwb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pxpyqpla.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3bopkjmkg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3rqnuehtb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dueudzkv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dfjrswgo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lsgovawt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3indoasws.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3chiavsai.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bgrvymkz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mcsnorcy.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3yqxeakcp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wynknnvc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vjqrbcbx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qpnaxzlh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zvdwukxz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3eadcxczc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3airxejlc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3swsqyzyq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dnjdergh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ecstqfqq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ukeiypxg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3rsisbtgb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vwdgqtph.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fsobuvpa.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nckgyxlr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3kfeojqln.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ohkxcshe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3teozxwqo.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nagcetss.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yhxmmzab.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3kudgbgcb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kspesnna.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3fbzitcvy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ukkirsff.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3sxbcnrjr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xfytpgvj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qnvucaqm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3mcmbcvsv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3wlyilefr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hlllkemo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3lheqcqgn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3tjhyqjfa.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ycaituuf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3knlweocg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gptynnpj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3wibosjji.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sjjasdiw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3diasuysm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tkaqzqpz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rwnimylo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ztpkzcmf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3yyevorib.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ijhfthdq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3guwoivcv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3hatvtlzf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ehhuzous.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vyfuvbsr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3aedfkjid.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3nhtmegcm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jprawwun.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3iwochyhv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3gmplzesy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wgquoitu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3voxcqgne.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gjkrmxta.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xnighbmp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3firywdar.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zjpnifvo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rqenvrhh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kckphghl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3bimzlkbs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3isardhyg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mrxuvsea.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3bxaqmyek.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3fqytbhkf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zyhaloxc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qwcjzvam.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3anwpuafr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ylqvytep.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jiluszwo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3aswkwbgp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3idmxmtpj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dpvkrurq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3arccgijs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zommkptk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3anandinx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zuamviup.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3gpksnqsr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3umlumdim.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dcsbnexq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ejfvaawy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ktfptyyo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3lkczldqr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oswqmefq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3glkecico.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3thbsuwsv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3cocttxqu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qjrunivm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fdnynczg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mijlaszd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qguouokn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3befpciga.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3xbdqphvn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hyhzsong.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3keeikzxl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3tsalmovc.html


<!-- 参考信息 -->