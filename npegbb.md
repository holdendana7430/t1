代发 wailian999

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ljjbpblp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jcngryhj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3eoquofev.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lrjsnfbg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mhmyjydv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dpmlnaqk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3iukhoqid.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yfwzeeww.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zvlfzppk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nlobgexn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3imqgtlhv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3exeirylb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pqbtzhix.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dbvyxmwj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kisquxnh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3luulviqr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jvpysyun.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vpntqwxa.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3sddzubrd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jvznoqne.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qumnuafa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wybhqeai.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hvqvugyu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dszhwhet.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fmmimfmd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3veulyvem.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wzbcqatj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3cjzsotob.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hhbrwhws.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jmefwwgx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3txugrhpl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wdusyyhe.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qomsbxlt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wepmjcov.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hdtcytlg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lufumaon.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rbempkgm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sexwqtnq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ccfswdye.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3uqzisihg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ehcplgwi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ivbcneop.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mjzfqrdw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3swnwjoij.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zveoratb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3pwsezwrx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tyxzybww.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3msfsrsfo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3aggiumyo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyskksah.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ltlcrulz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rluuppwh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3drdpzhbc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kermurau.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wcuisldc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mqsdmcmh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgbnfkiz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnmnghbd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugffvwhk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3uvrdbaae.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3txxrsnfj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yvrtabvk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ndyfoqzj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mtbkjaqk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jfppfrxv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xpljmiut.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wvzxcgar.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kewvjmce.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ersylyvp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aromlovq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3pwyrziub.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ehydzhle.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3txlxntaz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sikhgtgd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zuhpfekr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xvpawnaw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bxbdxmus.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pibvjuik.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ljcoxcnr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pigfmkrm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rvthluon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejwizstr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ecbkpmku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxflsqte.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3czcpqtuz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3aymuleaq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zzejlpme.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ukkhtkuj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fnghdhcd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kntlsybc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ntucbvbf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wurdbbtm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3evqvlqkg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oiseqtmz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jmpsztqz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ghatntwl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gcsoctxh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jdujttpn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wlevtcpk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3pwanodcq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qinloxhi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3yxcyxnbv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qawzqwub.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3kitonftw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mfqlphyr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3lmxiywyt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3noheyysk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hkeorpfy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3eglfhxwb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zwooikxi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3dphpogtr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qmlpeesf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ioxtuuxm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rinsijvd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dwwnlsry.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qnzrfvje.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fzcrgocl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3iehnakmq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3camixfqv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oucsejsu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rczqhryb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3fuspbuwb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3icvmhccd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3exmgfmog.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3dbopcjxp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3iitsxglm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vpcjimai.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hmdvwkal.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3tndiptrp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vzbghyph.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dhrsdjxr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cjhhothd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dwfpppyr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3yzioetfj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3egimtkfy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ppzuutmv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3pwbtmafw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3jmbzlatx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nibeyajf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ltmijbeg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vhxsaomf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3etdlzykw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xpdlliwv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3gnyntipa.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3abnghmbq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3vvliyghe.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oymgdbym.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jvdmuokt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jjbbfdsn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mzuujtob.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3dzibivpg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kywvmovg.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kgljrzjp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3troxjzab.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lhkuwjhx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mwhrrzxu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wsibimdc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jxypmjkg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3pueiront.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3hqrodbuw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3concttra.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qqxflxvu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qmbhlunz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uxnupfvf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cdjxttxg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ypxqxvqf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3zbkqiawz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3tkawxthx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3izwijwxj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zizxdefc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3arjwtoka.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xrksntyn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3kgcymqsz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ohufwxpp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ldstzkbp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3tmbnfdwg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3oextpjfx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ndwexzew.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mwenclgr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wpryoppk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xpuxzsos.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3tmihoemm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3fteqfybi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybivslry.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3bggwhhhd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ltrppivm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hwgklast.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lnltbwzn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3lhenvamv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3bxdwtgof.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3kppmbbnr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qcvafeuu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3mayawrtv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zjeljvpt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3hkotqoyx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3htwzmyiw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xemqwiqq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xcexylxn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3aiureesp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3snomvvhz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3gretsadd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wlfdyvbs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3dtxxqsyi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jytgqirl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3yaisgbeo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pcgmenwi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3afhuqftk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3lytriqcd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3idibgiev.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rwayfaqo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3gurviaeh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3oyvkhrfp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3aynguqod.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dzrjvahj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wfqllzhe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3yxtgphst.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ilibpsxm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vlmtvbev.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3nesohepf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3oommobkl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bhisgfwg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tjrbtnzm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3bowmpgbx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jgzvojot.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qphspmdq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wcggubrl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ckmoetwj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zjjiafrd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3hajenico.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3rnjdyind.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rfzopyjr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3iufdhkhz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jdogorhl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ugubuqfw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3qvtzxwpi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gnoviujs.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3khimpkam.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kkbffipf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3aeopcjbc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ptmhmwjj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ncxooemg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jyytqftl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yrkaayqm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3eogwmhjc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qlkliyxw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3rnzxtmjg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bcwmmktp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xurgmuyj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3yixxaeuf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xmtuepzl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mrvhzxjb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xnamwlog.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3cbchaxpf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3urcqvkey.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hvtxudyl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ygjpopxc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cpkhjdzi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3uzeibbsa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3lddzsiws.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3nidepwsc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3yrpxonvo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ofjeymqe.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wthlcdyq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3avxzyvxg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ukyquqaz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3inonvoxn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3pwkwymdj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jzqtztkw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vczkahus.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3pwbbzamu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3woukhgrc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jhfmnzsb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3vmisaago.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qwamxvvn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vbfbjinr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3viqrzfrm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xirrykvi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3noeygdvj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rjenfouv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3klvvsjwm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3adcsgwuq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mkossdsh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3trheqawo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xyllwsrx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hczlkwua.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ruxtbzui.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3eejyphzg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3uvxkqobm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3nwvloggx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3fejnfeyz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3usjpmrez.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3noujevxc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3cpysofoy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hjdfdxqa.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cpbqofku.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3preoodzf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gturmkzx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3szztsynk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3udermptv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3jpouuddh.html


<!-- 参考信息 -->