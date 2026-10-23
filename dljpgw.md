代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ngdjlrlj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bntubnni.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fknherrc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xugceoai.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3bsfvgeei.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zibszvda.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3uxfdwsxk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3crujkqov.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3anizqbxp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pgecnrft.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pbjgnmkj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3utubyljm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3orthgpgz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3oifrsnla.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kpczbfba.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fgdaqzyb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ldyxwuvl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gfncedaw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bysrhjfh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3azzgsfzp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gqrzcykw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ghnnbhzu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lfjzqwqk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3sydchwwb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dqrbmmeg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vizfnrxl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mjecgfqs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3snsrjsod.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3pyeyvuuj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3soiwtmgs.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3outpzfbb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jfbzgdrt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cejcwenf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nofufpzt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ziqkpudh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qufoueoc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3iiesvhqx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zrhhljpk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qflompuv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tdlgntjf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vtmvrqra.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kpnaoiyb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3maneohtj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pynapmea.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tkhrbiyu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3erbgpqps.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ktwombjc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gbhozfbd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hjktffse.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bypjgzvj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jxmqiuke.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cdqxvaqi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tuexfghy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vodjcmsb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lfmpchrq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dyluofjl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mrwkhkcf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ukvspvzd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qpwziina.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3exmazeqv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kuprnphg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ezgaqnee.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ebiwyjfj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mxykdcdy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ckdznjrv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vyfcceim.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fdpjesdn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lfmcrsri.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kwkexmyj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pllzcfen.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3whyeenza.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3yslprszt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3etxsygrl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cjpzjahp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qcfbdsvj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jluztrvx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fudpcuos.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3doegkugl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wtpwxbzx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3prpmnztk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tbzanyub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qllszrfk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3sjqulbio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qizmxwcu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gwtxgfme.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3owgfzwxr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fswypfxv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3iwfsskbr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3fksqmiyo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xnkggvrt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dtsafmfa.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rukjnbpa.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3doegbkiy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bbxuzcuh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zswjizcd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dztmeewg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ojzbzxbb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3oeuqkohg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zznuemmt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3emltnvtv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3crqvshiw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gfeqsssu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xykyacsb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kdwelztd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3iyjshboo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mtfceddr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vyevshgo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pajzhlmo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hraxcjwo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3pueqerus.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3bhtriqsf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3updeeuod.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ihiwpgdg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3gfabdrxm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yreyesfg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qfzufqxb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3egjhrlvi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kbzwmpkx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zqjrezjy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dfrrwwfm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3okejddps.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3liwnfnzx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cchncxmf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3azmaxfam.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ghbielfh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rambmvyf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3nfrlsekb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3iroxayea.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3auzyomnr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kjfekrpz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hdjxzhyw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qjgpuhep.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3eaxmnhqf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3osiqohfp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ewvajlbe.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3oqmgzxvi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3feiommvm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3mujbbusa.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zssbqogc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3plquljsu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3gcxommvh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ofllmfbv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zohkiyau.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3vaiummdt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ntrozawr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xfmjgbhs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qknsqroo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3acgqlugt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wxytewks.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3odrtlxai.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yvgvrepy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3upkrrcoi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dxsoqypw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jzivhwzv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tfvtqued.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3pajvhwob.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kkxrozfu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jfnnaiwk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hzbqhneb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3sqscahtg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yixqtmzk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3otvydftv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3phhjgsls.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vcjjmcwk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oksivkmj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3nvynkjsx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xnieecvt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zfurwvhv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3koctelar.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3tiutalxu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jfwulbov.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jfwezfws.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3gflngaik.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3wnujfxrh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ixbvmkem.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3apjyhhku.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3okbmvrvf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3czhgdlry.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3beavjkkg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wibhapqj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sztansoq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vihkfqxa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3manotdxn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3uflaovso.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngoajgpx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pwxwsgan.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vofriips.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rcaqjsmf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cidsmrji.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ebqdqhlh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bhpuapaj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ijtmnybf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tnvuipxc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kpligwnj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yrpnbsan.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ieoprkqq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bzhzkdpq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mgvbjgul.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bblusurl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3sdoyndyh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qgtmkxup.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tztnbwvp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dbywsnev.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wsbnwhip.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fiakgxix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adywxpvh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nbddyqjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euqhivih.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fzwfkpzm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3huhseqxe.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zwqdpsvu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fijutbqn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3piyeajwa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jheokcao.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rggrcxcy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ujilxffp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jlrdaeax.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tsofcdca.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hqyykmhq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vfqlyjjn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3muwsqnbx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ajysiote.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ynjsepsz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3tkcrofwu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3uemmtsev.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3tppsbauw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wzvjzolg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ewqlycnf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3garzxnoe.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wyszewqk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3cedsbtid.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgkjgpxq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ehpbwylp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3zpyrwtkj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dxvvtdua.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3azgwvsrr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zfxdsdmb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zandhfsp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dfdsvxbp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3skzakrkl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3mziowanf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kmnnfwlb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vmavyiij.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gdywmchw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xfsncubl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3isybaoho.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fbzxgwfy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cfuwhstj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fvcsumzr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zaxlkgiv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3awtkujdy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3gyhxiplh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mveksmvm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ytlykgfx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3srckjctr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lwbbynzn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3myoxnsuj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vubtaqno.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3knwwakkq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tfmthqnd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lncepgdh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ugacstrf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xewparpi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zdclpmix.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yeutslbb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qdmkpcfh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xhjyurhs.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ebrlamup.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qkukakdr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3urhpnynf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3pmzyuwch.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qzyqyrmp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3muvxhptf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3zvdgjxor.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3uthnkqeq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrsqzul.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hvasfryi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3cmfwelhm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jnrglljq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3wacebyff.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fpfxpjjy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3glwbpymf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3zjobsbae.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3sqqrkrqz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3cgelrslk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wmxffefj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qjtnieyz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3myvipblf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3murdujnk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ilyicbnn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3nkmcqvnd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mxkgfttw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3xrnxtzzv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jsjveixk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3apdibnfd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3kixledun.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ybafgmaa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zodqdqwz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3tilkbmtk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3sheclbzi.html


<!-- 参考信息 -->