代发 wailian999

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3weklmnko.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpwovcnq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mvnxkism.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3necprugf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ryrjtpwk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hmdqfgyp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cunblaai.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nnirfgwl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bgtewveg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vdiwcdbx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jjyybryx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rzhtxjcz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zfcsdlsi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eulbaluj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3fephvyke.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sxalxjox.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tafvjnda.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zfoyjccr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cyiupvks.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bwulfsju.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rotzvhet.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3aukaipgy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3npwohasi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bsqnsxjd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zbnrdtgp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ianszcwy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ifcjcaid.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3oyaskpja.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xoxengmy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3uczqumvc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vqashylc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjdxebqs.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zhvwfrgg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ktaedasp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oapfcshx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lriexvju.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rgmojfxq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3weurjnpa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kdjdoppd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fpguoleq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jbqlomew.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3clluhzox.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3zwggqaav.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pgccvqmt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3molrjcnn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xdvqrgfk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3dsmizece.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ngpneqpo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zaxsohox.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yvvydxav.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ppzhollb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uekfsylg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3paonlibs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dzhkbqth.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3uejvhjgb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ddufiqia.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3sxsjgpst.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ggorbjue.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ryuhrzff.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3effiotzz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dghjvrcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqibtadf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3blyysayw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqlunprs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gegtecrm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3enadtflq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vifvemra.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ybecyvba.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3trtpsrib.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pwpgmzyh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dzcugbuy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ufmjkxiw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bbaodwwo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ygowilvr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wfuuxhtm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eiusvddq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ykdgmexc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3macpcxli.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3trrtbwiw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zssgyzkd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ifvqilhd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hqdeoqhe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3skndfhsp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yalprnpy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3avfkfxdf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jeymxeuc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3mckwtnae.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aprukdcp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3brdfiwcm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhgbtmeq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3loddpsqb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uytturxj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wgcrtxmu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mjmzcchb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xruugxud.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lcbjvcjh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jbikohrz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wscumhik.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3buzyxdek.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fihkttzj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gjlxoksx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3whmmapxx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jyjvozem.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yzteshiz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uwvcdksq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hngrbjwf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mxqlryhu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zpzzzxcx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3kkbhgtwj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3roqzizde.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3trukxzzr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3caoynkok.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3qvbnnpjw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jhdfreki.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3cjteqglf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ivxpddpq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wkyxfdxd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gppbmwwr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3qboyjubn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3eofyphtc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3iaywierq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mqmltrhm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3jaqsnihq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xyydadkz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wicbrtvr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xvktozdf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3fsgyuxmk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nvrurumx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ysxryfsn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rooeacne.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gycplerd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3cafvyugk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ukofevfo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3inrolsab.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3neoudeak.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pwvcvgrc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nteqbhsv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3txqyumnl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3aznwgnnf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3iwyplmko.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3iuuynyio.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rmkpfras.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ztvzpyaj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xqhxcavt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sexjnvqv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uloalayi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xcojsatv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ugxpprdd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uidaxdgm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ltdxmbqj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3expxbbxx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ddodygat.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wpripjmq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zskoekao.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3eomswgtj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nbweigvg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3uyutgnri.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iayexude.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3llvmbhni.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qchyyohf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ynycvugp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nnywiuwg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zrdaernk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3sxmofgee.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xegyystr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3owckczji.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pqmcjxeb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3aqhngoif.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xnztavqs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3apzjdwnf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lmoqdwvg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eagrqeap.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kaatelvh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fdzuiqzw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppnrmwks.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3prrjdqwe.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ndzamkie.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ibfacbkk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mmyuiind.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dcllubvb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uxobbnaj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ywszoeea.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ujeplnuw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ntvzbxpb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3npyjkyqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykrrqavz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lxsszmrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxwfnvti.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qvbycpnk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rtwngvun.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mjupvuee.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fmhpyeya.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3rblwhzzw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hybrgadx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zhokkwvb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vlhlblvf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sivqkibf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xmfozuib.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wxxkkzjt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dgblcpfy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3iiqxhewl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3whxwnpnf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3iardpnir.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hxirgdvp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3smhpjiwc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vfvvhxwy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3oayzpwnh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xjuxjfhw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3trswqdnz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzaqckzy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3oeyobrap.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhohcol.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3emefhmue.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3lqxeixst.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ycfcqerc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cuzpjlcw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3hdoxefnu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3rmfyvvkb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3angzyjaw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gzzrviis.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ygnwlhts.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3szryimxe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3oiuvdsex.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dtsalswt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zbdfroge.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgshmpyp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3juhtncal.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tfcjhpdh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ffooydxg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pibilphy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ttrzcfjn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ongcgyco.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sypqrekl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3erreisri.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wztjilnd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3brsihyzy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3stvrhwyw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgnwztm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hxzgmgtl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3lvhvqrie.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3vixejdmj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dalmdhxs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vealhyxq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bggqqitf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wjoxcyuf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mhsidhzy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3qkboryro.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zxrhzngb.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wuctwaeg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qaitmquo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mcotcivc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3kmipejvz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3kgdwmxuu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3yhfxtulw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3mjdlrbpn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3rfnjkyjq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zcziwdtt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3mplvlftq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kczdomxf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3uizwkhcp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3alfolfke.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pvlahmet.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zopqarfn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qenbudeb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3uvmcvzgm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3fhsfdgyq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qdiplsnh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtahwto.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gftmckqk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hgnarxiu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3inrurqia.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wxpdxqrm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yrnuijiu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ehrestge.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nnhsfxgh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dnvlbhtp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3lccnpezb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmgubihj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3eoxrqpzk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cvowwmhg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3mtjqkecc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3oykzipfw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hlrjwzjq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btbwamrn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3mrcpybzt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3nlkkkihz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mblraezt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3skxrqpqb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3thhnztee.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3zwaduvvj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbteplsn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cpfzzwtk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3doorkpfz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3josxhqwb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3wajglfop.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3cysvpvwc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xbiatncw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3sitmbjte.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3skytofzj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ytchwcpb.html


<!-- 参考信息 -->