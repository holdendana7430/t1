代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3envbtyfl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3thtxcpir.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3bwrjpzah.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wzeepjad.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ycqdoxst.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ufafpczf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3exuhlfqx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3flusenck.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lrhhusme.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jpofanfk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3usfkichx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3trvdpzfk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ejzopkad.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xdjrgdco.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ddurzzha.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sqkbnohx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3sicudjbp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ahnrasvv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nlpaupfe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3njbcwuhi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dtphxlsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxtoegjd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lfqbenex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpjdxnme.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nlxqkbzj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ccwwwbqf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3uzgvhmwy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ylythpuf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3eoquuihi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jlijzttn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fzmlqhrh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lnkocwqy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wgsmfupn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3amvvyscj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3somvdfar.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pnpasrsf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lomvazah.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3klznmghv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ntnffqpi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oeskaspn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3bjpxmxmx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kpxfiqjv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cuunzbgz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3snjuauuq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lpxjbhfb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zyipvxso.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3qutaeiil.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkukmddh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xlfiirsu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdzdukhw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3hzlldiht.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hinrvdqr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3pnltetkl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3lfgicufa.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ouoelcpx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vcvcyunc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3frtcsofv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3oyduaiaw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hvwxtllh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3kqcwxtor.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ltwpzrgj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dzftuokh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3pliaxyag.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3okmpxccl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wkjyncpe.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wypyrwem.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3dkkhobka.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3izwxtwhi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rgjaotvs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3synpjabv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lalmpdhu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3leuawykx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qcfpgkux.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3pqoomwjm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hvzlnlaw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3udzgohap.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ccxiyapz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rcligell.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tvnvdjre.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3sdktrbpu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3nrizvfkx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vfeulepv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3knotsxnu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3djrnlqhc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tcuwccjw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ydrgfnqm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kchovnmg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zlgfhvey.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ikyrawit.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3akeqawvt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3eczhmjbb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zfaoequd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3alypkocj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3snsfkktj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ukuwusbo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3tnbsbjqc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hetdleii.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3quqdjxfi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3twnjyjqf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xenwdnrj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ibrxhwyn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3skdvgrst.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3qtidvste.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ubzvdedk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dlxsptmf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xmjjogwy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3whexevim.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vmmracly.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gkqrpoex.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wmjmfzqo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vrpodliw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqryrmpj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3eohadqck.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3amripdof.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3cdhzcrbm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjmfnvzr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ixrizlne.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3evoiqxzp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ktfigkxf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3uckbzojk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3buiecgmz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fuakryiq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hcpxbndf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3lyjsgjwr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wpkmjzyz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yvqbijss.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bavelvpy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3uiqhddua.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3chjrksty.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rzqspkqp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mmakrzpb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vnvlrbpb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jimovxrm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wryyxrnj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3stgnqbgi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3louqvtng.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3majouggo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3buynozsu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pdqhtgos.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ulanepci.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qgjabkwn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yqjbhghd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3digxzidz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zfxyczfd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kjxihnoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhidgakr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3epaxjscu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsymigjp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fkqvmehj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3oviilnnc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fkpheolh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3giinebhr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3koikcjmk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xatcwxcq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3xdapattu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3foqcwaku.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3txiaezcu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sepgnukm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xacwmljl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3zslhtsjg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3tbxahnna.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3uzkstfhq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3btagwnnm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hmlajsgk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3vcamnhwk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3fqdqgswa.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hedsylsz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qchvjrio.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3torfeqnz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zflufdpb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rzvrqqcw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3skyfjgee.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3iljhajrr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3jqbinzlg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3udbzdfqo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ojlcdzou.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hoakfkaq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nwrehceg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ikzkrwpa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vfkfjzjg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ksdwblpz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qadkignu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3glmbettj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kzwfjwqr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dmteqegk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wbrrkios.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3cbgfzgle.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nrkkyvuq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3fmwmzlsd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3hzazzsoe.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3eiodrsgq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3yibejdif.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xszccitu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jumdvgxa.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fpwzatsz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jkfahekg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3bhifjopc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cgecknky.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xmbvtanl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uqkdwsrb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3owzhgwyt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3arncbxvm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cqqfmthf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3guvgrggq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yfnpgzzg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3czveztck.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3enyhaoxa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kxkvwuru.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vquzwqls.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3yaszotjh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jarlzflw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3lmghjbvf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3taeuiifd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3laebpxkc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nlriudoi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3przxxlwh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wfedgfcq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3dtytddwm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3mxzwijea.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wqldahwo.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gwhwpkul.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3mkycffsc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3uvviijui.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3sndcgtjx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3enyaoccs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qkoozpaw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3jjwsngtl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgojwmku.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3nhrvtfug.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xyqibtow.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3agrcqzpv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3uoanxbwo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lszgoefj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ahiwtfpu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3jpujbiza.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ripbylku.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qvcxdsvj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3trugwjpk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lollhxzb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3kzujqcuf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3dqpcbqrq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zjcjuipr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3whjdldlv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ptpqnsgm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ndjftnpu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3nqzvuzwz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3sigpljun.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ugwgrrcf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hcarjuyb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nagwtezt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejgjxfcc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cbvbahnl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ympsnswd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zxtxgfkk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3udlhymfg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3cfxagquh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3uzcrbnzw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jqdvyrbl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dsxyjwuf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vmwifjjb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oeqfajqi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ttmoqsji.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tffwtvdp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3exagaduf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3cxtvgckx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pduoptly.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qleuvcva.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uzhpomtg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3rtbqkgvv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nyeltmtj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3jaumeoke.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3aucnxwtd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3arscxqxr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3vaekmerk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ywgwdusx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3dineqbcl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rznxcpjm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3byvawddr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3znajfzfh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xovcxsrk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3menwwnup.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kicjnjkb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3yajkgaoj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kvypvzpl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3vqcnzjgr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ehuriepi.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3dgotskqm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3oxdzqgfp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mfuyoflm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xuqpvnln.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kqqybxdp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mgudpahm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ighehmvd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ewtnffjz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xejhasyf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ujdbhmpf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3obyyokkz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3bswnybee.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3zerxpemj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zquvwxyq.html


<!-- 参考信息 -->