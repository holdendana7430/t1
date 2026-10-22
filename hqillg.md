代发 wailian999

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hxbpmpop.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zqlgbmnx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jzvmkjhx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aijxuugc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rtuvijcb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2zsfdlncc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2mggurwqb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2omnbvqoz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2faqxtvow.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2upuwkuaa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gyhmtxks.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mowuhasi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2nqhueveu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2crijubtz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2abczjdmk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zlfapqps.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fnjrayqq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2pyukvqdd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2rgmjovzs.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2katwykcc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cyggwpzs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dsgdyyme.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hhksdena.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2oiljmklm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ilgwlmck.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rnmblnjn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2glxdssgc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2zbzobper.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wjooxyrs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bndassqa.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrzggnnv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ykcbfcrw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qasdmszi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2prtitrbl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eljybozg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2asyhccfs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bwuxxyey.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2elfxhclg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nprsbrio.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ujlbaacb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jdzojfcy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qxpullic.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jxotkxum.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ojzkhdga.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2emmsdeij.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bdmszwii.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2qsnoochn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gspctftw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jptdqxrt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tseepdtu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2piafnjii.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cajgbkbt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vfptfybp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeoindck.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ojstbydv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pkkpiqlx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jvggfpap.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujvqkkxx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ythtkkuq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jeumrbwm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejyncsyf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mlrzqndp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cnucdite.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2goahwlok.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2djgexlze.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2czojwfxn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nnywtkng.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cdpowgbi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2djcqoqxh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pmvvhoqx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nzpsuayd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vxjaeibt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zpflpmuq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pjpalkax.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2osggjtoo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qpfggckd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rhgpeivo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2puseybii.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dxvjfqmd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tbmjznzc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vjnqsujh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxrxchde.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gnpkcqob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gydadaxa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2uqekhepq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2uybomims.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jdwhwchw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rfpawqvj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rizffmif.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2crujdsdt.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lzpuuhba.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oafipoig.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ygmeeqdi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vxgqlwkk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2garbpxtt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xplrwphp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hafgidcb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fydaahsa.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2abtmbfar.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2poemgkpd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vsrzrukz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dtcckdrd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bmylhipj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2iwesjxug.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2mqxmxpro.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jmkqdcvo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2sxzmpopf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2sahmzqhb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jmkypixo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2binbfgqm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ziocddpo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qswtxszk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2szrvtzek.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hxaceuny.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ttmfcezh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fdaeltnz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2shjygzkd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2skxttplu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xqkplehy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2andfkjud.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wjnikxsl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2cacladfr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2exsgpvex.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2akdtmzqq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2yjrtdosr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2flnutxhd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2gsjdjmyc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tzzudsel.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vvpstnyv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xralvqgo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bfgngijd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dsslgovl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fzuylwgu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2mfwtpwpk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2huniyhea.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jkeisuai.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bebihnfk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2krtowfgs.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2luguchkw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2khqumxjq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wqfoeobo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xodefnis.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2apyrsuyw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rutfqosb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2fgevsdue.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jzfbzxwz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fkkpztse.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2omhdxkvp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2qbstrryu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2avgxariu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2zhusaxdy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ofybqrxn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kjvfcgmd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2penmzdxb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uimhpwfa.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jwgvbueh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jvpwciex.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bwiblhpb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2cxxcpjgt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2fasomgzi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2sgpttuou.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2izboxsiw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2bsfwfrku.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2upxziodm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2joblaznv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2mvzyutvg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2amhvhnpp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2oftwehnt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cvwhlaqs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2uuiuieyw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ordergyr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2slhzrvso.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2uqgnkibf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2omrwzmnw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2idbigqiu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2qflbalpq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ftcnlzzv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jwlcvdfe.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nqamwfgw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnyyguiy.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zhucrtdy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zotehpqg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2dpinqtbj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zibpmqby.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2hrjovndo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2iisywgqh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jaybbvdo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jxnijgtu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2lmrwpfjk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2viqexrel.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bdeemotm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vscwmiol.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zsbjjwqk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ioicmrqt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hcjcopgp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mzswpffl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jmjcdfke.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kmcmsvwp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gxgnyrbo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pbiwbawp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ceocwibw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uwndgzyv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2rvxvdeiv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2pekegfwi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2fymgnzdo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2svubferr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2cnkyejnp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2xopulsez.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2utrkzalq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2pfzhaseb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2drarngsm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ljugcqbf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ziyqnjtz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2slolmhxg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2shnvtzjd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2risdfser.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2bidlpuyl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2aeqcbxcy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2gzqviyfs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2fxtsjupl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vneipnma.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jbstwhiq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2aedturxk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2epnfwwfo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pghlmubm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pcvllfkm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kvkuomtq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ecapjfiv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jrafpmzs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2zrruevld.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mxbdwrbj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2bwwpkugg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dpqfzvmr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2vbmnwzzw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gdryuliz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2bbaxkksq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2edyjnwkq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2jrreymew.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ussgyafi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2bevpzhsb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2avkmrozy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2gxwvfryp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qayahnel.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dokaocrj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2tjfkmbur.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gkejzdch.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2dlxxygoo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nxjkkkhd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2seriwqej.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jlovzvtn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vzzchlyj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2nnmkgsnl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2dknqdzns.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ldhcuaje.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2izpyitfn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2zfxiayaj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2jdcwectv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2skqhlaxl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gbxmtqfr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fivgjmbo.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2yqtwchtn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wqflhbsc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2kyomlaiy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tutugwvl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2gpndmssb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2pqoizkmj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2trqolfvh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqjemek.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wkldmvca.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2maksenrt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pwgdxsex.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dapyowze.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gbykvbyu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qyxaqjvs.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2yinipgvr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xvrvfens.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2joqsmifp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gbfsqzse.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2kiksriun.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2vtkazigd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2rrsximrq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2pbnvkmde.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2shqkzxab.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2onguqgld.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2sjlwvubn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pnorkotd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2zhuxxcet.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ghcfbuiv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jkygidma.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2smkmjexw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vpxiasfb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gjgqquel.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2jsxyrhji.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nfmwwszb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rrouoymd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2vkugiodx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hyiwdsvk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dkrrgdyx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2unsooxzw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ndpyqmnx.html


<!-- 参考信息 -->