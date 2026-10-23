代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3iioytweh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hdnlhngb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fgjoebog.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vyqvgtyt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3pbdglpjl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kcrpzhez.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gahmevws.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3agimrfcv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xronqujn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mhboglha.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3srdiyrcd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nxhsvsov.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rsbvfnzt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qcuzvbus.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3zfcnuqdc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ugnugbod.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dwcfkfgp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fgkffwzd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cmonhomr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3drsklsce.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wjikdbwl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ocwdnjti.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zgydwbww.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ddzwxgqz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3etgvppvz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tyojrzfb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mbdcrpjc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jsdydszz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qgsjpukm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dgybpbmq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3popcjpqk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pzuvidts.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wuhbcran.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhoqurpv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bqsfaaqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpcfgpgb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ezxwixcr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3faucgazr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uzdgizvl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vtfyplkl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3fwqivlir.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3epwxvevo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gyrwxmav.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3iqyfjsjg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3udczpuvo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3muwuqxnv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pzfhxbnl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3woapmgmn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wvrlwptp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3idtwycxl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ydzmhfyq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wgnxpttm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3odfbadve.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xgotqmhn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3znsoemnw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pzauohgc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ncitikmi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3phzptqsl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jmfvbsnj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qvbbhmlx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yeytxceb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3boitrhbk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vhklfxkv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ikxaiald.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gtmhwwub.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qyiyhxob.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ltlpfehg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ipkjaqut.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3sedkmtvw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3pooczjze.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ieptccur.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3akfhfnxk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3xdxokfcs.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ktzcudrn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kcpxifux.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mqiruuzn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nebqqtyt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3nlrymtua.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3idqqwdmu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ctunakza.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wswvspok.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rspsdcwp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hkpjxfum.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3updszsfw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kbnzhsvx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ebklrtwl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nbvbdogl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fhvyqamg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3uswbjsqm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ahmkvrji.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ewvfybll.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bwnrywlz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wsnjonqj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3prcuizxg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3gamlavmq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hudyftou.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3evitouzn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pluogmkr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mhqircbb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ctxywgxn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bnkemjie.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lyydfkbo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3vxpxorio.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3wgjlqmlt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ftxiwrix.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fcamxbci.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujhkokcv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3tmuvgsrp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bdfomhzo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3lkpsuqfw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kbzbycur.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zummramu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pobhlgcu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3rkkqgkhk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dmxrmras.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qafyxhbu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3snyfwvqb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wfvqasco.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3epkbcwhc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ouujruqd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uooebcoi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3eksjkwda.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wqillpjf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3yhgzhoda.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qbinkiks.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kasxallt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xjzqzrfq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nbxiktgn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hqulelhx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3vbzrzynr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ibuiklbl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3krgsoylr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nkzviswj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulbcvmuh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uwitruli.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mjlwqvcx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3czueurmt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ravykoht.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cqakbwrp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oiiqqixh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3twkpiccs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3msjpbrbo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eywuhdik.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cuplqcil.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrsrvnwg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mrvoflvp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3keywepqf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vxrtgtsn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xdekyyqo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tsmsagva.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ipljsail.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3qekwlzzt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mjszcjxs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3bhqtyfba.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ulsigcsc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3iswhzhqp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3jhlquwfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhppyumx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3alndkvjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yybmnngx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mqgqhwej.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3kjqejlnm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3gycghllj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3svmtsqal.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kbrqtaop.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qyszdrqs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3iugerwvz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3biryhunl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rowqfvhz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xeibivwb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vmomnxaa.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vkozvhyz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3yeczomvo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bjuphmdr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ruqnhqxc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3oyzyawod.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3uibkhgmk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3tvzefdzn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vdykmkji.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ayosjwft.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mhkxdclw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3znwojquk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3oafwlfww.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3frcapwnr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewvapbtr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ndphhfcu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ymrknszk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qyttkbeu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3piqaexbk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3smfptgmd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mzkullfx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3yplibvzu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bipnmdis.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3sohnnfih.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xsgdyupx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jhnmmhpy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zoskojgs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3yulbkmuy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3cvfhdnzl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3sjmvmxvz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fgrzoddc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3wewssmao.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zszggcof.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jpbjbhcu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xzzympgm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wdwztbyr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3npnryvtg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mmeqpjwl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ejyekfjt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ynwshbkb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fbmnvpen.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tgmrtayk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zvgmagyg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3msqskezk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3guuxpaew.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3leoziwnw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gwdlxhov.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qfcjbemj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3urdhhnsi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3wbwoxkcz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3btborkmj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lgojnjks.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zwzdvpdz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3jrgitlhb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kjudiklg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mfbpbtso.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3iilfdeqn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3bltmlitk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3grlxbcmi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3odtlnbdl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ztnehxax.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3glpipvvi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3dthqwdkt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3kdghfthf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zroiexxl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ratbobbv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tvlorhqd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wuajozwp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wgurihzt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3plddhgwr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3zcchtfjh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3yhcykcsj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mojoykuv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tcfegncx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3iwfoavyy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jznkdbfg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ugpozona.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mzmhcnct.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bkdibhef.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uditvdgu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ijcicmdu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qkduwcan.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3khtvuvcr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vyexposh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ymdduedl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsjjzcip.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3nofixzyz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vrppthpd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qvfaeypc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qshwcwjn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xhbsapww.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3usqnmxhk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvngihzs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qgehwwfn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3faeghnbh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3xoiqodph.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3iohkmrmg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qsbklzmr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3jxcsaytz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3icggackt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3truzliwm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihnmgdsf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3smhenfyb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dvxqcnwr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3fmgbqzqy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3pjsosuzp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3fpfzcnnl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iuuoahox.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dpyyctsl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tbdxuyyg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3wocpdbwt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3czhkobnn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3kzpcxtit.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nmpjmqvr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wdykvunx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jwcmlczd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rjbuuqqa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3cqkjlmed.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3enopomhl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3meycwehc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hcgzncoo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pahkifwb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3usdtnniz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3udpuuauf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ewkfatcq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3lzpzqbbf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rogpyoox.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zbwlzyum.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3usstejzq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sgszmxap.html


<!-- 参考信息 -->