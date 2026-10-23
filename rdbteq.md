代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jzbuveis.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vrdtjvuf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ngnatsmd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fcvzbzse.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fryfbwna.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3lwvyabbo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wafeqrre.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zsaxyunj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3icdxbfbk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3irblkcsz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iebmqilp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wrdcgxer.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ehwswcsa.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fommhhvt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bzgyngrd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3nrlrybvr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3coacmxva.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qdfnnhhb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dxjxlbsj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tiytnrfv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3avcrwwhm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xqiavqlc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jqgngxrg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cwxtefhv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nklbiqou.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3cwpvmrlu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bdhsoauf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qorffkvk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zbyidlha.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zrahkcmp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3dtnhofug.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qvxkpeqb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3astabnyb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bafufodi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jmnoajfz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oucewflz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hyrgauhr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fydyvvpx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3eaxwxvjc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jlphiyiw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xzzymalm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pomvjezj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmrqawbj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cvkpwewi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kshnmsyf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tfvieseh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rqwprjxy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aswjttzj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pkiodyvk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jllgkuvv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3srsqxokp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbmnnerw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jzjrtqjf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgwcnhfq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oajvbnzi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wytuvylu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ehtcvpvn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xclxfqor.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3unssyppk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tjlpwxnc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rogijwxa.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ucxfnzqn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3siwznhyx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3kwjecgoh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ghacvpfr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hozwtqfo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cjjferot.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3upmhcvgd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xefrjcja.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3omvucutd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ysvxfsqm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3joupolly.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tfguvirm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nysafyni.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pqklehnn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3lwtfvqmu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3goarkzgg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bxukfjds.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ctyvwdvi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ekmbnhwt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wixjyozb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fienieyc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tnjaelze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmokkpdv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tashvinp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3keqihwgc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xcmzoros.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3sigerjye.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kvmnjabs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3aigwoexn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ytfadvyy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zltjosxq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cqzlyspz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fbwxvoas.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lmmxuevw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gyxjvlqy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ptimaesc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzmarysz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fvqpgotl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gzcevtyu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cpaatbde.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ggsdplwt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jyorfgqr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3resfxusv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fuygmroo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3tfeekgsd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pnoutpqd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yguahpoc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fiemtref.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3szvfqfsf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qgjltzqb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhpveqg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3untturoj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hahiyzmj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mprlrkky.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tuaykhaf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tjjgaiph.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3cquarubs.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ynvrjhan.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3naaqfvdn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3olvfmruw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ocbsxyug.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qbonwxrw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gizjdobl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hekyykwo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cvthbivi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zwzsykfp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iaaazksx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rxfkjxxp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rwudiory.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3teccuhsl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bsoiabtb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3bfqmlgku.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qcokwjgv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ludqehqq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wpywxfts.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zyovlzii.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qwioetqm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rtqsmhac.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3igalzvsw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zlwzqnvy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3keipgvpb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ibmlvbdg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fjeduwpu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nnwuyebk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cuzmmudg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bbqrwabc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3syoparrp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3duvarzpt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jzynvgcf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vpciafqr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ggfvilby.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dtvsqhuv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jgtwhqme.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxjcjaot.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mzhcjdzm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vdzkaquf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3eentotij.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rdxhcvvu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3robvhynj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mntgmlgf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nlifjeda.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hyahvruf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ttjsujev.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kzyxxtfn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zgyafycl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3werjklef.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nusogird.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3aluzxpde.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dgedqzne.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3daogtujt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3svvffpal.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kwbgqank.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3rhytewjv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ktotqmcy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3etlgjbxb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3kxtivpel.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ogvgstew.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3pengrqin.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3cfhicgll.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rrkuqqjr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ssymyjmb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3twfvohil.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mjkrxfgl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3cozajyxl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xlvegplu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3srfdlzmu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qflvbwqd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ookectsf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tpeufydr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nryglsck.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xjspgiua.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fyuvbmjn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gtbtjvio.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3aufyfgoy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xeywxfiu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fiallskj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hnoouocf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3iyjogydm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3laecsgzv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3estbuxbc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nshyawwg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hvjtqqen.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mkxuruti.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3aywhfdka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfrathps.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iavcvlik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xezemdom.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3exsoqdfu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3djgqovag.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3drbfzayj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3snnrmzix.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3uekthhum.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3biqtxpvt.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3whzuvueo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3hipmpqqs.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3sxszizfq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lmakrowp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yxuyalmz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3itbfkzfv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zmtwmyjw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vevglilp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hiucamfq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3sivsgiuv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fowxvfmz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hpyucapl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3sljmvzil.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3atfmojnc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tuputmec.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gqeilihn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3codnyaxx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hkfunlum.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mottidxs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3fhlfuswt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jupkuybl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mdjxzniu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yanavfjn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3adqzwoar.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ebfdkrqz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xcmlrbkk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3meraonki.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3nzvwpiyf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3amymnoqn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3opfmslni.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3iyjyshdo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3oudqjupw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3msomvmpx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vagzemry.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rrkegxnn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3cfaoqfqb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qhhygmhi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wmpipusq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3kyrzuwjl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lgbijdpw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3damlbpok.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fiicuuuc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3irbgxipu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3whpzusay.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ghmhgtnl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ueyyierz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ayzirsqb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3fadyvazv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3aiadvyqx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qkxayhjc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jaaekyoa.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3lyllzkjv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xyiwrhxf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3iwflfycf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3sauizsjc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lnppeedi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3abtpgaxr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3joakgtnw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hgwwqcgo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3xkwhtglc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3uiukjvxv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jxkrgvmj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hsafympu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wxtlqenv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3orrzzhoi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kppypqpa.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3bwvyswet.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3npawfzrr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rrapkjor.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gsaoersh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3kxiqyidr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3fsbkqhrn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uwyvtsrj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3crpzdxqa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3maubocfm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3lohrqnxr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3cazrsefr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nvudnake.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fpdixnup.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ylnodgro.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zezdmfss.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xvuovdhj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vmnptffr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3foburvxn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3jkvsgdzk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ngggnwot.html


<!-- 参考信息 -->