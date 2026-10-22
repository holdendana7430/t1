代发 wailian999

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2pfgddklb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ytynscps.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zmkzkcws.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsflasat.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahwsaxaj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2evcyeenm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhsjbnck.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wvxrfrfk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jjnklkcc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ggqdzift.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2udahkrfx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jllmpdcn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qdaodacd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2frtkclbw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jpnnhiwd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wrohmcbf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qehrpdcw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2cqwvmsov.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wpdmseyp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rntjctvo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wmarhepv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jhjzpdon.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qdycyouq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rlvhexnm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2phndvdrl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2etjnaixw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kpqvxucv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gfizkjzw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kpzvqmzl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jtkuffyx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lzijplvo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2egknfzsw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2riazzuay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slgenxlq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2uxicgsrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2makakflw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gpypgjlp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rijxzvwn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bjddbocm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qffmuxbc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2bnhlncuf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fmtopptd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2czrsudqm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2riazuqxb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fgblcomy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ejziewpi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gfccksfq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2roguetob.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iewohzsn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2altysnno.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mdshmbpq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qndxcmbs.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2jlgpymhk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dmlvodvd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ncpefbly.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2voxwumhy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2locmoybt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xrzcgolf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bbyrgvrf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhurrfiv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nezdhrdz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wnrokoqi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xnzdzdyg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tggduzwp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dogfrvqs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jjrjeqhr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cczeqzok.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cwlwjiuk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2sblqqauy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sxuxnddd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tagsgkgl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jbxmkdlb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2caupotqt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zepikfli.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ljlemmsb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2cgilsolj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mtijcbew.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ubbkegin.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tlbhkpnn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ctynbokt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhlaoofz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qzbdolek.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hdhsuugo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2znmjmfnu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ffbcogtu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rieihlsg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2soqnfhvv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nzfyjrkd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gvcqpfks.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2fjexedzt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uvyvvtvr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pztiqeqb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vnjbkkpx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ybktchzp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vbnfvylf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qyumldqh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jnowfpgf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jzouaqwy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2awitxdgo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2sfmfexut.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tuiczxzq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2uhrckgpi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mzrrburd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bprytsoy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2whxcbrka.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2iuimtezu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rsgatjhm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mgoqedna.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jaortjiu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fvdhgvth.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fjjtxvaa.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jzmlfpei.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ypqqpkcr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2msdelycl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2kzmypdtn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2lhqcudpb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ngquixuq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ljnhzihq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rqebzhpp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2toqbfibf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kzmmoxoe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xspqqskp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ateocfba.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2rpbevhjn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2cvpwyogr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2rloqxune.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ttaikdnk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ttpqrdpc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2qwixqptt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kipeikga.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qozyizfk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wsgvdrhz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mckckuub.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vhfkaadg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrvgejiv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qsbnyqdz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsayrdkj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rymmlcfb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wqrxrbtb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fyginxdi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sqshweab.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ufcdlnog.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mqdjahtl.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hmpdatvk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2lxvmuzmx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uywaipvt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kaetwtnc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ustmlbkw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zdilroej.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2peokcdcb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2znkoiaut.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2fojdshem.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2elmugyvx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cjazjwfh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xrkrgpoe.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2buwatwld.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vpcadfio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rraiunof.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uvptpnzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdmndwje.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wjwjpynx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2usunjssm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2zhanxspa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qkwetetn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fpqcadph.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2pgsgtgtl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2kxzfojza.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2rewmkpet.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xpxktmii.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lukuqnrg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2tbndyysp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vsjcjzqx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2szdhwexe.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2eeiicdsw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2niieoyvd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mrvhiize.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2odoabtyz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2uaiwnaso.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2mpymijfr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jjagfqnf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dmskzdqh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tfwvzzzq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ldcojntu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2nxremeqa.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2oognnxba.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jchrverh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zihubwig.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2couneism.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xrfbdhuh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rkcjcfhj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ptjnkvmc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tuftmpwd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2htkergsw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2rulxhekc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nhrqsbde.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jhqxvliq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2dfelwfnw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtauyoqq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2phatcnnt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2htlogarw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2szqynzrx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dyrybdyb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fbxsszyl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2laqswysg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmdummrd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pdiqjxfj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qocoqgzl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kwttyqfd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2cifngcic.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2adojdjze.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2cgqeyfhg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2uamyjgqu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2fncdmxga.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2azvasqca.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2teamesuo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tflyjmor.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tbjmkvpq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jewvqmsh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lblikzab.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgwszgc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2dmpkyjlg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2dctjytei.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tooxheda.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wtmjklrr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2atjdivra.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ulskkulw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ecofrfkv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ccsdexxn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gqvnybiu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqmwapg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uskawecb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mjwdolpb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ddkbgogg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kzdledbs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2mvifjobg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vkhxzfdb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2bkgatybf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nwwqzyhk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2fhxhosns.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsidelzp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2pxicgiax.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2szxtuujy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xltkcnfd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2naftrawd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vjmuuije.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2obwbgwxy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2kdttayhb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2djpglggp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jtrxasbb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aujubxip.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vjjcleeq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jrioxgwm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wtukooiz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2avbbwqvz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fsmaepkw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrlwjdbz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ytgiwktl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ioygizme.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uebltmay.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cquhbxgg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cdspwcos.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zcoxtfhm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uwbasdfr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2srkzflsu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xxcizpzt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jplbrkdd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ndkiyuzu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vjtnkdyw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zjsrdgyg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hlzthsiq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgrclatt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqynxroz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gugnoula.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqejzglm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2sxxzecjs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2szydrqim.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2fbmiqtgk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jvdjcefo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bilknytr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2yosapwqx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2dehnywqm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mdvwagzq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2xznhqink.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ukwaoise.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2epqfxorf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ycymfarf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mpvkwumo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xevxwgis.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2romtqdll.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pckbwwhu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2dntfylig.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2schtejss.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2rigpcgkf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2tdpohkhh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ljxonxvu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ggajgopa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dslsgmkv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fabkncft.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2cyepnpus.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2etqkktiv.html


<!-- 参考信息 -->