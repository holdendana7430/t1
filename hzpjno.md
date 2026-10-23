代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vqwuzwdo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fegvenzc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wfqjxjin.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3khuhgths.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kkftyjfi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tvtszhbf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jrylokkx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jctdpzum.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xtzlntxe.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ylqodiak.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3pzxbirtu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rpxidjcq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3toydcyii.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dbfdktdp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3gpomxoqm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ljihtito.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3suwdjroc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hkumxhei.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3epwttomq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ovdtdwpb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3yughszse.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3novtuugf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vkjfdxub.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kgdzpemb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qpumwocn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3lwobljme.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ckyyixzo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ygbvvvmn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ptqrsony.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3tfmsudhm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bwfwrltt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hdkzcbtl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3guagthsh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ytogyqnv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3gxbgxwzv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bputrkan.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xtciymwa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mzydzlnr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hwfdnrig.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ggnhhonn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zoctemip.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mfksrsye.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lxwsziic.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlvbffcq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3muzjfanb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezdqjzvk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fsyfjwtu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmryhnep.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ptxlovin.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ngcsbvzz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3swgljkjx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mrbydyoe.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3itulkrlz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybhlbskd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zpopcoyt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qkxbqfpb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmqsassf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mlvqoqdj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oyxxczzw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3thoygnku.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3whjnbwcx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wwrxxffi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wohkxfkz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zovuijff.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yvxwzpcp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yldcwfqh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3fabtykix.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mmfirnkc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qlmbzkke.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sdirtmaz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ztbawwic.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3nfstpxum.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3znrzxpwl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qeqfjepy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qpwjqbji.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qntkpxtj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lledjumj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmlnwnnb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ioqjdzaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnwndvtd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bpugxmop.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tiigywho.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iwafnsbx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qxoefouf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3slceukvt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xuttcydm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3qmfltokp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ftkqfzmc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ufqngfgy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rwkhcbwj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3uwjxjggh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3rkvmffqj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3qrviifri.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ptjfxzwv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3sntzjbqs.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3btlynlkr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3adgrjcug.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3wpfsggni.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mmnkewoi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uvxumphs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3uuutkybm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tumgacdk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xoachiqm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vrelzueb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3bwclbtad.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kyilntef.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ezgeamgj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xhsieyvf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3glvldrvc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jlrkwaxz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zmkpstfk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fdzasibu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xrsmaphw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3loynptol.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nphtfuul.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mrjjktks.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wuopbjel.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bsagjjsa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zdvkceuq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3pfxwjlhd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3mjepfeqh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3yqmrktkc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pbeexjpk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3eiilgguo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3yttmkulj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3sxrukgdk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3bvttdouy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3utpltkzj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3nggdyaxi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jajuwifm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3cmuwtujo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3skagkmyo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3bjlhhpfh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3inqfunwq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qfmlwqby.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hscbixji.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3lhiepxsa.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3scdojkpg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wgskocpd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rvftkppr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3uxtshhuf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3pdystqcp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ssmvcead.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3rlpneoxb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mcmwnmtb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3dhqirlkl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3cettsuaf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zayepngf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vuatvcko.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3phxfyofc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jhrcitjh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jxhnoeiz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3msbgbvhe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3uwjyommb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3dozsmhti.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3gvlbjpej.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3xrathlzr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lsxrkfaq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3rbhzetbi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpdhvoqz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3cydaojje.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jjuhdgrq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ttcnvqyx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3kybiurxe.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qcxsjakl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zpadbxrr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3iptrfwkw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3vdiiluak.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tgjjppkt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfxtactm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hhzmhcoe.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ujtjsaat.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3umcrweub.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3tcmbslod.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mjlfbkfg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3crfgzepb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3jkrvnumh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3gikvywxj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dkbgicdr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqwhnklq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ypdcjygr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zqejmjiy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tbxdjsbn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xokfboel.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3lnonqzpq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wvugrweb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3edcxjufv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3gqcvlfpb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ieidyomp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nvjkzmys.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jrlgtywg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ekrrgjmk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vweelfym.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xpfvivev.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uynsnmos.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3cfrkkvis.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3amsrdttc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qqnuugte.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wpnesbsq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kqppupco.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mdgiwtzx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qnhnjqwb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3iggbrboq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3bgriqaip.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nsmvivcb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lyeogisz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fzvlixiz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3tqogltfs.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3peudujzi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ctltdocd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tshbxupc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sloaaydf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mkyadrki.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vnqdyiar.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3mfyurmde.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3srkvxtfb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3stdwckgi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ockpcoek.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3sexlcgfq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3nihsenfr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yfqzccew.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3otepotax.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ysvmxtif.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wwdiybcz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3dmxgswah.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3wumvdfcx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ozobnpiw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ujputkre.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jzfpeppa.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3kkhnjtsw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3uiyvqcsz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bujfrbxm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3zejaflzt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gfwngwyu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ttywdinm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3rmnfgdhe.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3qmqpfnvd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3lacxyhkf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cmpkeapr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pmpljgkx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3dcpxtyna.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hndxjqdc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wvibeyyh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jbwhliap.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ypomxiea.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3umemwjrg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3dtvmcjbu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xpivotbx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qlipeajb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hbocxnmo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vtmhikzv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3puwrbklz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nujmveat.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3rgvyrffb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3eewzumsn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3bpmtarya.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3znikgruj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wabznqah.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3froyxqig.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3afpgdufn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wisiclpi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qjljuxei.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nbxfzsxe.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ruwvzteo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qjkuyekf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3fsnugdfw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qggywjlc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pcbkovyb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xevnbcjc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cykscgwb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ktspplhh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zaanhgjt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ywhmohzj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hnzzmkum.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3iqakksti.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3cqczuane.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vzopealg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bmebhinw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kdrgbcku.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vuajiuza.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3cgdnyabk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3pcijaudn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3oulaxndv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rsstcgqf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3araulgfm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qgorozuz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3nkkcdixg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ngpaflnp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3yblqvkyj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3plzqtssn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bjbozsir.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3imjtqdbb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qctpmlld.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xpyqheli.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jcqbalsi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3thbissqz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nbrwihvm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3emgtxeda.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pffbminx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3wnulktrz.html


<!-- 参考信息 -->