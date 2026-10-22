代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vnchplpz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zteicwnw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jnfhogyv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2nkltrsqm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2btruajua.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ourwdlur.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2myzxijig.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hozzzynd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hccycyiy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2amseuenq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pbyrmvlq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rkqlrwde.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yidfzyqt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oixxyjnd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nmqbuwev.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2skvsnggw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2osuolhmf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2awodiuvf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wcsxgald.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2nhhwifwd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rmhdkkim.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rpukybcn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dqlhyqku.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2oaqffbcl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nomyjlgj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qglhzfdu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zipduyhc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sumigrjz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wgwijtop.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2cdvgdvfs.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pxjmcqqp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tvevjsre.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2iytganqx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2lrshezxw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2twrplxrp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zjqqpgbc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mjjiepkf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2oizkjzym.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vlnkxkdo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2sxrzorwe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qhtwjymq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2obzglrul.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vieibawv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2pjqpxzuf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnjjpwvt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2yfhrjhui.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nrzryues.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wfvefwfb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jherqxru.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bhhypnix.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ktaqkjmt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2bughoyjk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qwrgtjrg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2nqcxconr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bicalucc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2eggamrdb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jzwxxdgc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jvheuerp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ecilyqag.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oevvjubb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gekxmvct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yblhkzby.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sbkhggkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iynksbpw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ajrqimfu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lvffdoje.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rjilznjg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2wntxgqie.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2majuvwrq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ghuitedm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jtxlwacv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lviuhwiv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tvaiiszg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vyxqgozo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kzcnovag.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zrqnzmwi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ixxjhiqk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gvcsurya.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wipmqdyu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xmdcejsr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2irisxjcb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hqivgeqv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cissbguy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2msvapnkl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2fuilfkfq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lyswijqk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2oqiokvza.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qcundxli.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yupcgtnd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwfcnxhm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uhluhnsw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dmgrbtoq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ahtyeqlo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2szkasqbi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ziekjtmx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qrgrgqmp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ezbdnemi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwrockcx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vrzweija.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rqtcikzr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2bmcpqwbh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qftiflwz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2unmnrusj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vxegmrny.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ngydqbpf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fegaihac.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2dvmbpfen.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zrvylzku.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsvbuvan.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2zhcetztw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dmjtgnms.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pgcqqvsq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fgnjgegz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2aazmeprh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pahgvvsj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yziwuixr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cinvjavt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rpfbmbos.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kvphhyrt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ldctguub.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bmzchwbz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vqgqglud.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tpmptgcd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ipqiyvyi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yvkmbjst.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zywmbqfm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ijwzktrr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2oujhprqu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2azoehrks.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ncoqklng.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2dbjvafft.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2uwpnbbtg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2triazuqk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kevdnwwb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2doiqzxzr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ialxszfy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xuydugre.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mhevheyp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2shzamama.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fnthdsvd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tfxbfsjw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fbwxdova.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ltaijdtx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kgrtlwtq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jlvscmay.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2behxcwlb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ohvzyiwe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jvmjxnyl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vloycneu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2rwmblrfc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2muxqmzgb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gthfsxwi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dhbamnge.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqwjdsau.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lfxgsquw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bevpjboa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2whylijwh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2bpugmzjp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2iwcehqtr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xdqpzudf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wbjvuzht.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaiqskxg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nrnfvhrr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2lqhehdyh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2emowyofx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fgfhqxuj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2edkgseto.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lisfatao.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lnhgpzov.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mguxyzco.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wfitttkn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nayfxiuz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2opqagrpo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cowwyhnw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kospzaur.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pjftwexe.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2waemerfz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dkdpolez.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fjcaiojx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2lzqkqjiy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lvyrukmo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lbxyhzmp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pbvoyzao.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wghlpbkf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2uyuqvqoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grmocwys.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2myfuvttx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxwfajcb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ywtnczee.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2umvmnlul.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gsubcwdg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2fofkteyw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sqgovpis.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zyypfskf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cdkmrwst.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2eiyyolmw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2hnvtvdja.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ghqxsbod.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2asqpiqpd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dplstqcl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qblubmzj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fxyitbxf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2mhvvvpqv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2srwxwzpo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2htyozyoi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wtkamceu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ibcygqvz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xpcwvqio.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nvhsfooc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cjxmhbwt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hfqpytqw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qbzdzwnd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2iaccjznl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2uhlaiatk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2pfiwukmy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2oqlwkctq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2iwvazrpo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2tgnowbbo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2nsirudjj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2pwylytfu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zmqlqkmv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2njowftdr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fzpjbqiw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xkzzavbd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2nfydnhbb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqubrkqd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2uehrjygo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2cwvczqma.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2alsthgdg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2nqowyjgy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vzxkipje.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2swutzaht.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2idvminpq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2xmwosnhy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2dqjhmkaw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nvmhixpf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2sgwikjvx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zdkfuptx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2kvomgybt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mvnfrrpo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ixnvbbny.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mavsgmed.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2losvhxoo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xmsbrehm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2kvkhyqhn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jdxknoiy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xaiwcxah.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lohurnds.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ddwvselk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kqqtmokh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lnsvfyhy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ttgdfjck.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wopyxjjl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qmdimcoh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2pdfyjipb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qpioljiq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2wasbwiyg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nplukyul.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mqrdmlrf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2khpjcdft.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2mjulboeu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2flfbajdv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2rwpczypf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2yynlhqhq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2sntwumbt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jmbmstkq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2tstufnvw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qkdcxwrv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2htmxurnc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hqqhdhdc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hqdkqjbj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qxqbrriy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2aqyjaoum.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2pidlhttt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2tulozbfl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zgpgxtoh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wpbqohom.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lywdgnmr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2kxwnejqk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nsrssnmn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2amdsoiuk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2keazeddj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2kwujpapp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyanszuw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ovksvpss.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2sqtrcrhd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yswrxdgs.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2qmnxahnc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xozrtbds.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lgukqmwq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ayjowpgc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rnkylyih.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ffiptfct.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ixrkqmcn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2bdnvurvv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vnjzkmog.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tyngzuhv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2drzmffnr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2kpwcjfap.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fxnhqbig.html


<!-- 参考信息 -->