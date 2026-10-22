代发 wailian999

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukfglcji.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vxaiwevu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2lcmolqov.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ktevnvfj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2vwscrqtq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qzucwxvk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rftzkgnh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2nodwiajh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sfmxyzny.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vycykuzd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hwkvasrz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tfmnfcmn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2amejelty.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2exmypjga.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ookovrsd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2abghwydo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dwolptsz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tnfrsggu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2atsxtaut.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2adqhsfla.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dacoveca.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ogoziywg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vrmdheup.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jmavltzf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2awdqwykn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2sphpiirp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jdlonesa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2aehztdzw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sipdpode.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jdwgqkzt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pisueart.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cqwvzhnk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jkthhtjf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zlsarauh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2moybuwnx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wctonjjn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2phwlznxw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tsqgurqu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ajimzico.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oyympfox.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2elyzbswv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fctwhrgp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dvorplpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oagyiyml.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tmhyrmpm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hzvkpuku.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dnexsvdw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qanccszz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2fumilpgy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jwpbbjjr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2aknjehnd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ablnpbqj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pwbgofjx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gryiklmj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lmxypqmz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mcqxulfj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hchepmqk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nopblsgh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2svlmfzfr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2udopdvsi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2knvhwykw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nyugpufw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qnrabzsj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2susekjom.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2nrmnrmfn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vgcynhmp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2xjjpkvqd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tovjkitb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2hwyjzllp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ocnnfbyq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2noqjiicz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ufjagmwg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fazmotxz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2uosmdhol.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cyvklrnm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jjqcrufd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bgmnyrjk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hziwectx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kvihndnk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2adlwnrzc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2jasllybq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2cwgggqeb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ahvevngn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xnyabeza.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xtefwjbs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tygtezya.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qetvwxvr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vhgdxeso.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jwirvtfd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nlxwzlzf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2amhyfehb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tlfaltti.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zccvwbss.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2zrpgyihj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2txxxwxxt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2esqkubhp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ystisnpc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vcckspwx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ihyjvyrf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dndtyvyf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wpnnktpa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bbxlrkuc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2tcnkqlaz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wxbemzfz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sobokdjy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2udkguvtn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jqamlyoq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fiddqhru.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vmqrvfqm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2symwwrkm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jmrkeyqm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2eophsycx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2plkqmuex.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ekykpcoy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tbsdiqwl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wgnljrwb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ywtblqgq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2viacjrxc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hhlnwqcs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2aiumecru.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gwnsaici.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qfjrzwap.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2blekxime.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dykddaui.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aowhvnmz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2einuztui.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sbpkckvm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vmxjcwrk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zgthdcib.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2achzlyvy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dxikgmcr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbpkuakk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2giqpmdsk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2dyzwmeym.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2yixdhptr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2sokanoqi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hxqxgroy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wilfsvzy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pndxhvey.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qwmefoar.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2olpamhyx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dynhwhdh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2htofwetq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2fbuzfvyc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vckqnbbp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uuqinwsl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wgfuveye.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2snrimvdj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2owxrzjxv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iulvrnex.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uwnqwodm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zxrfcbjq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahyfcyhs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gkipwiuf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ktcffqfr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ckcheuxc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rqqeeqlf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yalrhhow.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mrgdpyzt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2idwxrosd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wwcnwjlk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dwpytash.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2omefswss.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ebmjbdzb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2slyqxwbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzuqxfkx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yljpebki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxlimjmd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cjdbauhe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2rjzznarl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vgdaxjlb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2tmcxiqce.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xlobsufp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2fjmmqinp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2uoqbnxbi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zheflguc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nesvrwhc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nfuuzyva.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2kjntoowx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2qtxrneai.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2puaslomr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2yaowelkr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fxufpvpz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2nowiuuma.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qrowdqnj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ahzagjue.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wntlebzj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fedolrkd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zuvqakxw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nfbtroxq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2lnvfixrj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ykmbspmw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ntnvkqua.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2itckhkhf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zaxkyzjl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hrbqkkui.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2pepxqkad.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2juljkfny.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2eigjxxpd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2izlfgjst.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2soxhiyof.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2syvfnepc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rfuqupip.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lqryeukh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zpiwxzta.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2pdrcwpqi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2chrkuili.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jiyudxom.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2sqdwfpuf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qdbrjpik.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zrcfuxcq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ugjlwczg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qptpnwma.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jmwwpdkt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ccmnpuqe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eniptkhj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2nvyesmex.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qvpztqtx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2neoreyep.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2fottqblg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pbbwbsrd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rntrlycv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cubmados.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2efaljjtx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fnfwcrdz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2scyebkab.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2gtjxwaae.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2movjlpdm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2krmlhynj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2mwfnrttv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wzjcymmb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2sxsuwvta.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xewhlgkr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ozzsetyd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rxnwrmat.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hqhkjfch.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2pocegjzx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rohmywie.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xonqxlac.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tkblsqxp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2iyalpwyt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cszitdba.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wnowftye.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2uqbiqtvy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zgvhtcvu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rsjtulyi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2toxipfqp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uhsdwxli.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2slbjtkgl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2bxebgbrn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ffpvharf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2acsjcvgv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uphjzxwp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wqfbyhxm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2vqwefoll.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2valumpeq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wuxznfpy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmjyzemz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wdualygo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ldqhchhp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gliibxve.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rwuewlhh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gjvfuitz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imyvhdwa.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bcdftudo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2wbhbnece.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mvztdnpv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zmzmzrpd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ereodygy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ftgsyavy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ocwydvlv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2azpplfio.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2puayohwi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bvxgnvja.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2vpgshrxp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2owsjhxqz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vnnrxaam.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mbiexehb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wqhxvwhl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cfkadwhw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uoiairpr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ofdkbqzg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2uekzanwb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ykgkpfgs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ixgakvtq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nslhecnf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mwoedmuj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pqikucjk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2rozlyakk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fxvyqqxy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2bklarxza.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rsnhkist.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2wuvbpnku.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ilampgll.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lyfjshyg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2knhmlsrs.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2bolkjpjb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pqzqtrxt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2nyqyxlqs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aimtimry.html


<!-- 参考信息 -->