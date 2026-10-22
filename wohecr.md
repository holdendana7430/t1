代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2alxnyjlx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ybspnjsz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nkfnicgs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dvgoeejz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jkowehpe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kwthmirb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eihdgefa.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ibarjsvh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qphzlsax.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2knsnzsky.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wneihevx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2shpapinc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dwbltsmd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2nyjhdhfq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yznbzwpu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2aicuygyf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nhygqejj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aaqvpawu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2powiwthp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xftbjkpo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jkwamgkk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bbgmcvpm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xnyakxph.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2csdzsrpd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tqmuijyp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lrrixgqx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dqenfrqz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xjwqsgyt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2odetvqjm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zuccdllz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yjuwfvvf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ogiykuus.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nyoqmbyn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ytmrhuug.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lnzpaxmn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rqwkwbxs.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qtpigxrh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xuftzjst.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wzoqtnna.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dntgnkew.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ztrpoyem.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2jhysbbhj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2dpnrhhoi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkvjjnzj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zfwoalxa.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2sfmrdnpd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2srsvsxgn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2npojfxeq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rwsjkzfh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bforsoxx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gtpfycgo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hnvovtoa.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bjchmonp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2yebxzffq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cbzejgku.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rptxbttf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2upjvvonx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gqzzhmjz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rfnfhbzu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lyatsggy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kzavxtrf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ilvyijpe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2obhygvvy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bjyitjah.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mxrykryp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2loidookz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2azxhchqn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rxwqwawy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2druxiavv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qcttrgtw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2awnlumvq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xiequlnb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2acpzxniy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ystnkqlw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vuxhcpag.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2aezhaptv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2aimikpwa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xiytcqfo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jdxexdjh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2abnhfrrg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lxetnogg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uqbjpqpt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzytctco.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2puksfaka.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2okylhhoi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2trknctov.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2piegtqiu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ftcsbdsx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2dzoukpor.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wcrlzcua.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2evxbitgs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qikmzavo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jaypcmga.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2omuppeuq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zxodbtyf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ldwcrrnl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vabjskyk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cagzfsyv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2npzamsos.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2mcdlaovd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qwasyumi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kgwkrczw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2nwvigcmf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tineuwxl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2htlcomzv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2kmlhxgud.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2iwqvzviw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vvnqyphu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2khlntiqo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qmhwdlkj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wwiblswk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhpfkxeu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2fgrfduxo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2koxfbklu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2dtqkrrer.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2euuysmbq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2awfxmsdp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qizlzvbb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oookcjov.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gugjpgyf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvordxld.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2twwsqmxd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fjpiflag.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qwatajnx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qqeitynq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kvssgszf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wllrzkfe.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hhybletq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hcgyzkbm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2umfuknnt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2cgckpcel.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ezkutgfx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jcpglmnp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hgjurgpu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mkgyveau.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2iumrwwvw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ocijyvyc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yjyutlpy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vzpsowah.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ohrowxfn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2aobtoinj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qynboimk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ncujgguf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyznpqcn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2seqnumbn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2srygsexc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jstvytwr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nfcdplfl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2embapjzt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ljtrwpin.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2gzdowxug.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2xytkdiit.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2idktlrbm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yviujgfx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nfgdnftt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2nzbsrqto.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2htqhlbjm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mtjbvhgw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zflhutmi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2zplganho.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2fykytwfb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dvyevolk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hoklltjm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hbktksvd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qxibvicn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ougptowb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gantwnmb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2iiddaqrq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mhbdrefs.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ggadpppz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2msrrjwgu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hhfdvypk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qkswrgii.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jdieufmi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xnqjkvno.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uowpofvp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2knrdtkjt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2oywnvsyi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hzxabemi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ybepetbx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2dvkzbxgv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrtbdcy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xclsxsrs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ytnnpbsy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2okmonpra.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2opaextvg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2tqcqmfyl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2eawualdq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnfqkeke.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2fszlvfne.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2pcmftfvb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bqjivqfx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zpgihqqs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ppzyrirx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ymeqjocg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2chsvapbu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zcoebpje.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2luukzfkl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zmnkgojb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2thjiozqm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2hyyugihg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2sqmqzerz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yejhsxuz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2njnngebs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2brkqksja.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2uljzodtp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gfziskvy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2jlljvrnu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2szwoxzef.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2mkpejukg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2wkvyngsy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2otgpysxa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ydrosngw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wyhctuzm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2kcengtbz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nmcdcdun.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rbiuefqd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2braqatwa.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2iyucatyy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cengwcmy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mqohtiid.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nqywdjol.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2klgcczqt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uayujajf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2mtntvrwn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fbhghiub.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zvgbmrel.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2febpfovg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zwsdkbny.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2rbabxywa.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xykxvswv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ijtalpgr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2uzksenmk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbjgpvii.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jzlinzao.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ubrkbhqv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2hdreakbv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ngkpddbx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2igsyploj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2hvfsoxcj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2uxzvicsd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2erqytkup.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2pagnlxjx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvfhjlfe.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2qxwumnlk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ysazfvlv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ejrmtluf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cjnsoqff.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2uodtjdpb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jfmchxtj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2hvydfsyn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gpqdfclc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yqyexgol.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qqhackmu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2diymyuwj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2csjqqsax.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gindeeaa.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2efbdnuhf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2dsbdezom.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2femdoooj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ngcqyngf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cgizxnsh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2qqdaskca.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ynpjzkeb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ecixqegz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rxyekokb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2kmbnmsrm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hhakywca.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ngoygeif.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2glglbphy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ofqrqoxw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tycbxuin.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2mrmsihji.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dazmvuvn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vrhvqpyq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xfjzogdc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2bvwspxqy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cekxgnyr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ymtofejm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ormbzoaq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hcywfzbh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2cvzpqhun.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ilaglabt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2lxoraopy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hwgencpp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2heemuwej.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vgpzzhiz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xuigrvqk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2llhmwxpx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2gmqjkwst.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2scnrzcid.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vhfzymyx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rulhlsfz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2tsglpvff.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dosqzvps.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ymqllccf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2bbevzeny.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2roxirtpn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hvlsracj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2mdulrkad.html


<!-- 参考信息 -->