代发 wailian999

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wlqhkend.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3yenklasq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qlcdrmpd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pteevvrr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ciligjmf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hfkdwbfk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sjqcsnzm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3unsgvpxl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ihovuijz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qzrgpsbz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hgggxfue.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecwekvvy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jqlzxyvt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3evsbyvwi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kykrcqzy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bvptgtyp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3igsmmxcq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mcqydmbx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ytswgibw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3yivjivon.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rmucazhy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3nhwudfib.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ilacedys.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rstdrqpn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3snhseytp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3teirjiac.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3uuwafcpu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wolmuuzh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3sxppxzpb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zlfqgkaj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xoyunasn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3roanmgrn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xhalkpsy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qjughpqa.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jgdnaynt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3horkxgmo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vknfcnwy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rxihmlvp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zioocbdt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ocouxxrx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mvsqarhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egofqucz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pmjukymh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cccowfvr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hlhqruay.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ioarjlav.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dzcppxbf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3danuygpe.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xxjcmimw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vpiaavao.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ohqkyfyt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3izfwzgnv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xxhgyuyj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pivhbszy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mcxppqye.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3huqaakzy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gnbgeqic.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dtvhvozg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pwbnectt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dopvofuu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3puefhiiz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3uhppeghk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dzjdfoqz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ecztbpse.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dhrpxsef.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zdwneuoi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dawjhxdz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jelsyguw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bqnbpezo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldevwewv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kgcdqwvh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rsdvrtmf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3lxhwopem.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wiodwvmf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ipjovgoo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3niqkflij.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vsheajwk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3skewofqr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ptptjntz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hqqdzczb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3otbtjkzt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kblgvffg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3eenjvdxv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3paahzuko.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3emhuqueh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3okmkzxsn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dtbfxpzt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bwlonecg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfrqhxrb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lusaeabl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3trdmjcod.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gpgjwlyw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pkuqniqn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3svkepbww.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zlgigawf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mebwhuqz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3lgyqonxv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3uoxhcwyj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zlqvbmeb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3kijcdlpe.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3kctunfxg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3thrkheki.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3slffymvs.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3aaizovth.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ghhlbpbl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pdredgpd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lgzvbdnd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wewlqzen.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jvueibpx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zmqtppfo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mxzpvcgx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3fvcaxhbc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xpsdueom.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3mavlnvaz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3immaowta.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3agwmvdrl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vdtyuxvm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3woyaiczn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3brjpnvtz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bbmjexyz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vncgfmtn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nkmnzafp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ybqiilqs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zbvnwxgw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3acpebide.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3afvjkusd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3uznaydoh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3giulqnpt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qxehfeqn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qdsujfad.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3exlxciny.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pbdsbzdb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lpjjyzna.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnuudsra.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dpkkndpn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3efadhozo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xargefha.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mykmkdkt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tljbwrvn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cycslgxc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iokzxevt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3spixclxt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qxenfjmq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pbzozqvv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhhwfuhn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3beghobae.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hogbqigl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3nakfilhv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vtioaybj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fbqnhyil.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ksufjtvt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yeoncqqc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ljvckwis.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fuhmaeiy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkhjbfsh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nqtiyxjd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uacmgvls.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rhiwggke.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3znnacjim.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3olpbenlx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ontucmul.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmotfvdg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3htkegrlv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3nkqmmton.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lffapgqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbjjsyfi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jpecwtqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqljcnme.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3blvdkbgq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ndzeomrx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3treazhen.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3njsolyqx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3yafbddry.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3seopldjm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jmcwwbmi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mnrxoasj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bkwizkyc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tdilsggf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yvktrijc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wkvnrrtp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3geaatken.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wvvyvutj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lcgkxckk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3csacvvqo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3iugkrrej.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3sguihhqs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tfbaxzeh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tltviwdo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fcfyhvda.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qqswpsab.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3sgkwvjbl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3roccsila.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3lbxzskdq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fueddhft.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kdhjuico.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwheexz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3rpbiiauy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3dnuhmqiq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gnusykaa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wbyogeew.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3jknhaivf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3opvvbpjj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3kcochand.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ypucwyws.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tcmdgqzc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3qfkfpsvh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3czlkpxqn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qeatcxor.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bfgnwdxx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pklpztow.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3yxveykwp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xyihodbw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tocpvoge.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hntcizpt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ptujrxwg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jtahluft.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ccxyhbjz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3etexgswk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3wpvduprf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ozuuncwf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3siuikmmq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3yhdhebzz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3shpbjjef.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fkdvxhlr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3trldtgly.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bxradjnw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mdayzhhu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xbvtzlqm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3hkzlsmce.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3hwmaales.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3izzgeugy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lqtaqrqh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3odfaffhb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3quuvjpkn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3brndloqz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3lgexlbds.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wffoxvar.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3iliaentp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dzykhool.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3adqspxsi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ksrnxyhn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gmclxrom.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3icyjvupw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mmyyawav.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3zmlhtyau.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bdncbmym.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3iuknlspn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3whvpvtxu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vpjamcfv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mnzinedy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3lgslzolg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3cboyudkd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gdtqmicc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3iylrkurx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3byztueqd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3gazwaiju.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3zneomhmf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3twcunopl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tpodijtp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qyvvghsd.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3yxztnpjj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3mobpuuvy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ggzxizzy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydkfyeuk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ekgvsizv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mfzgqfta.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3zzvtffyb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3spdpcmyc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pngoelmu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ntgpnnur.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3saxihqng.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pghrevcp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qndfenje.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ywytrkoi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lfgowbwl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3bmmbrsyn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cpkkdsfq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3syduzxvx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ujchegnc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iaaespwp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3loglxamh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3letawphh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lmwmyhem.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hhvadqrs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zwmwkqxt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yigmvwhq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3lcjiyfjq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mmnzfdxf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vadmcxpz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jlwqtood.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3inkwhqpk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3bwaxpvfv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nkawbnya.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3vdhoeqkt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sjoqranr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3lkrxelwp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3cyognrxa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3khuaiwun.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3mayhvwer.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ivttxhcq.html


<!-- 参考信息 -->