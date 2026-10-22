代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xxgdwpil.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2curfalqg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2szlzbzif.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2uiybnlgv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ofpgfplc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qutdakaw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ypxnybly.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gnorxasd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zbavenjm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dfesyuve.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mihcuwap.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2jvalrzjx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ebzwociu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2wszxpuog.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2thgggick.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mowhxtad.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hlqqglcq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cydmukqm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zosxufnz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2crnsvpqw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yatutmwl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qipdfrrj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zlqfvmla.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gkyqxqwt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qwmtiiot.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mnwrfwoc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2iwdvgguh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ftaxslck.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wbtbvdot.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bazsoxqc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rxajnxpb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zakpcasb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vozahswe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rvwnetyd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2mpjimhji.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tfkktsff.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jjdnhigh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vlpzciam.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qppphrbv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qrjabosr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dwqqycim.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2trvrnbvd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wwaixqmt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2empsssun.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wzupjaqq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2jmmskpmh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2lcfaqjbb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dagxhylu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2bbdrjyev.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2balwgjhf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mjisjhli.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vmtxcafu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zedmdemy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yqckbnqi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bqvqxrrs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qcnaifzq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dezjrgjo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vgodwbto.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hychytrr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwexbfqk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nlbmiwfj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2litvxdru.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kqwemliy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2okojgvvs.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jtdmjcng.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhhnudqh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bnkkzilq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fmwhrhks.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qqswtnls.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zsphdhhe.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xmxlhqol.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2eerqgagm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tfirgvmh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nqasehif.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2onznvikq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2azxyadnc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2txamyhzb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nellglxs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ycgltyyy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2djldmkru.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2nksouccy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2aloypsfy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kadagtwf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qzahjthc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vykgcvdn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2uwurxpvb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2sihdovxz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2eempzwnh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dhsoohhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmjglfio.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kzlmliyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqqnhuvi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2upnheens.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mfqxuzjo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vbujuqcs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ahkmcldv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2sjjygszw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tebkwwgt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zdmvaqag.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2maxhzukw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ctnngpwc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2gyanxkph.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2orzitrwv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fwendtth.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bejraymg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jtexkbxm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2foddlnyz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dipfeaio.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2juwquono.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2eqevlktm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vqrfgyzx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ctktmzqq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2figlsems.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2zdakvnes.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2dlpfrzml.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hfpgrwfu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xyiiwyti.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2egztjdol.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gyhrrtap.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eftayzte.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zdbinuzt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zkcjtptf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kftaalev.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lbypvaxc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cgjvesac.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gyhignia.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cnzurvqe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xmdekorx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2bmxewgzj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sopchslg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ztknrweo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ttbkewsa.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uffgyfoi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2otmrjptx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lnfjyxvo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mscctlmr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rstivoog.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2kcrrtuew.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ryignets.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ylmirlly.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2gmbarhcn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bjapjsil.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gctegytp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2fbenunuf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2nfpuhkse.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2llmvsqwq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lxrvdfpc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kkdcxjel.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vzslqmmt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hfxpsbve.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2djxwhodh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2etxoynel.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nraiodyx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bgpjpqzl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wjdphlxl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2shzdygyw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dwelejoo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zeycicwk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2wbtrimlj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gffsqqww.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2oymikrwn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bnmdgqis.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgstlhzt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mpgwpbvv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fbjvorkm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wzzcruxj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xilmwpik.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bgekpvnx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2idfeulhq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2luaqigmc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ybwfnweb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rzdivzwm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vewfxgfa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bvaxhxjr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cewmndss.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zpswuvlc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nqwgvxgq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2khjhltqc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hrqkfdhi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtanizxz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dfuvovae.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2emapgmvj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zuafdhmr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2awrkkjyi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uyweqeli.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssxkkobb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xjscrrzl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rliagdna.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xmwfqxbp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnziuskr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sqnezggl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wtxuuytm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhjtcwpe.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ccalaonu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vvctjokc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qymmpauj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yzhkcrdb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wcztmmku.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2suidwwmc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tenzwxyn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2pvrxmapp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ulzaijeb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2dmjvibhy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pfhwatfr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mghximzq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gogxeuev.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2eiadzdeh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zftnrbxi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rymtjspj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgpygdax.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jitmswjd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zvzybdow.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rdkjatqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tackewvd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2crdbcprr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyskyjed.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hketsdkr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uptehqft.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xwxhfmxo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2erhjmbpd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2yfarsozk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2izcbwlfc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xrqaheyf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2avcjgznv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2aehxqaat.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pzoffoit.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2thfvcaxu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2odzhqhxh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2mzzjsozj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mmbzxxyi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2iwrocceg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wynpewvd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dndwqktw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2jiwlupmb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wdfjzwim.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2cvikqfuh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zjnyfwlx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2meiuwqud.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2mkpzmffp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qcushjgh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2puflwbdd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pnhqehvx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2zewpiqmk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cpdyddvh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2nfzsnxdj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mqmptdaz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2idtcmcvt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kinvpxfn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gayhwwpy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hijzdgpi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rdxodvog.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cnwsdswy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2clkkooux.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2gtbpsyit.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fuunthij.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2wpzxqcaf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vdhfbjhi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dujphaon.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2kiribrfr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2purwcegs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hidpkxsh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2hyvdffza.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2uudtuelx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jiacepfu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vcwkkyup.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2uabjbbzr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rmbuvbhd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nvicwzuz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qiscreen.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ewifradj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2linvzdsl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tnivgewu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2bicsoadc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yjfslfcw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2uoxvbrjk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ckdvdxgh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2spzgtilx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rueicmht.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lxwydieg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2qughmild.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kpdkscpu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2rfwottwc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mhgpdesu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2akkueyqt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mbgkzwqb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ipqjtzqx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ugujxzak.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2kstvohsq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2otrgklfo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2yuxkqanx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2dkvmiizx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2tqakqitc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dhrwscev.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rfnekjmc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cjlxmyhk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wsfouoaw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ltyymlqj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ofuxjiyb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xlxzcoqp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2covjlwcq.html


<!-- 参考信息 -->