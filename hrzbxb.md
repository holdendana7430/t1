代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ofwauwts.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kdaeapvc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fpmknlfr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ujocxmtf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2abbsqdul.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gdwkulae.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vsxiggdb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qfwhgtdh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lhftlznd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2wnbwxhzv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iobpljzk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zpxcfvix.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2phwyzwxd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fcxnowyg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2bbcjqxvx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2iguwufrf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wjlepxcf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2sywmzfmq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2uhznfuha.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uxuemfwo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wxdwogox.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsnptejx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rvdspklw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rxourulm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2csksfnme.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fwbbxwcd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2anxwerio.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkqtqqsv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ufopxyfx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xblxpqwk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wvydciuc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yhmgzofe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vqprdrbk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2smzjysgd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2feasknbe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sglxcqxt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ueqytcxu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2riecqniz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2loeklhzf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dnxelibd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ycxpotrc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rzgpmzcz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qkbyhoek.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nswhofet.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jqpawslm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2zbmnhkdi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bprheqwb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2nqpfoing.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uypdupme.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fgghrdvv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jaeqfpdb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdoaliig.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kqekifen.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmbqgopr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2arggrfzf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2foqobefb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2rnlmakje.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2eyrxjljl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zmnwqupj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kkbcbapg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tcmijgpi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kjizzzow.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uvsnwden.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xzeztldy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2porjoksc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bioltxjg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yvjiwgjv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lfxzrudx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2srhppkyi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kydvnmyp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zeigvshw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2crarlkld.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2skytaikg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2iitulibw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2atroxmnv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hmcqpcdx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2grtvhqfr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mwckuzdv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kaxnmakt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ntwmjjhk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2twwwajpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vupffwzl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sphecest.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkaolrtc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tojvvlkc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ezlqowmm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fxacexnz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2witnpoov.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wbxwppfh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nhkmrtuh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2uujzjngh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2bzuhvfuc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jyoyqkqv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2yvhwjtgb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dnmjfwjd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2csmpubwx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yihdzhsq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2beopvjxd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lspyonrm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pbkkkbdq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ajzkpkwp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2srtqvhkl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wwxpcrvh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2wknmcszh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2iunsqnpa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qnhhkcjv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2sjssdiut.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hehclkqo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lgkwoxxj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2tjjjkchs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2psqjdqny.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jexaluqu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rplxtktz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kdavdkmb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mulpgsxy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kfqngvsh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lkcrtybm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qbxfrltu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2suxfhyfe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pnhopjxa.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rrqcyjhu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ricefqoz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ykkrzmbq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bmeoyfxa.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ruhlbsbx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2lzwmxalr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2prnoybgc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mzimqekq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2luubzedh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gnarpeha.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2aimxwhnn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2trdkjrvq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yarpzgsk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qjgypxiv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vprybkmk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2unoxersw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2szzrilll.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2oqfvlllj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vnoerkkc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ygmzslfs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kjdvjonz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2sjjehbmx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2epzrzozh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jpytascj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2elzwbhxv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ssbolhyt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nsrhkkcm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2khzxbqqy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ofkngzkc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bdokhyci.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2bofactkr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cgfiajon.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gbkpejvx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kscjfhgt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnlpfjrh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jeaigwcz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cfnfmmdc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ztcrtsql.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2kaytsfkj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vgecapke.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wagfnmgv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ofgsfgac.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2aqqsjfye.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nernojek.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lfqkmuli.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rrxybtwi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mjrephxm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gnqfhurb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hwhvxwxt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ixewvypr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mlstfrda.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ritxdnmp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2yuyvfuai.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2intvslkd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mekzarec.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xscmklwn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2aqhjrwea.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2vyhfbgep.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qkaeiakw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2atabqjvj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2egtmxxct.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnjrwczo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gcdgwcnc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fmqgizay.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qzhtpukh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yhyikvnm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hrnhfqfx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ofzrhybo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ziedjcbi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dflsdpyr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2txaqghfy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fsaacotc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fcmhtgyo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gvntddma.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmkwenve.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ntvbpsfn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uhkqpajk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uxaaozgw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oqjzxshz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hfesmmnz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2npqigtkv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yqhwbwxj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zdammdjv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2rtnpiyfn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rswaglyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owzhlqoc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yhgsqynb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keovisjy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2oemfrtiw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2sbyssirw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tcdbpnak.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2kddphwye.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2svsyanxf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2mxfflnap.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rgdydkvs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ihiqcvja.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vfprpwrq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fnnrsenh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fonexvef.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2viikoneb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uzitnuuy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lilqacnj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jzxkdufn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rpdcvfne.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jtehlkrc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zebfgygd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2pticrcdp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ceeryamv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zoovsoch.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jknstksk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2vppduwdm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2weqbnojy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2lfdicspm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2kbcteatw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jkknznqz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ouxhftcv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dwurgwqr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gydebeth.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2zakacirb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tlureywa.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ldivamwp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2iicgcvuo.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2gbwzwdvm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2awsxiahf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2owzvlurq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2buykoecb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wnkzbtoj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxvwnnk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2psbdjwjd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2nkgmfrlb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2pggrbdli.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ulcwmjxx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lfeylbtn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2cgqryykn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2acekiwud.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2taqqajfa.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kfadmqog.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2trfaaudo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2kokvdmia.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2afxwugxv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bujlxred.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hklcngzf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2cnszekjv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dhbzbhjj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2gkazqtii.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yncfjjgs.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zfcwlcqy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lvmvanmc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2maboqyvs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2bqadqhgh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gpdykjqs.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tvpvrmdo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ciiugqio.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2sdghorwt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rudjshlu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gzctlkjd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nshfehxu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2chpsmrka.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2eunsfusk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2knzrgrcs.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2snnyzlha.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2botwmexk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xqyftjqd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2bsjhfkvo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2rvhfalvd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bsxulmur.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2prwbgaio.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fawkjicq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lfgxjhse.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2expresho.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fngwttyj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2lxjuruba.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jmxxzuyy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ghofpmky.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fusygyzp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2nivtcpwz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vcxsuvvd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwuzoeoa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2inzyukaq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2yaktdchn.html


<!-- 参考信息 -->