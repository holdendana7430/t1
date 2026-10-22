代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zrdhszzj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2suvqomkf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gjkzsyge.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wlbpkoaf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xoywrvcy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zsrzoksy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2alinvozw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dqbefycg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2uykruxxl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gkpwkshd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qavupfvs.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dhxfcqwy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lpefxbmh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sdtvomue.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2uyysirxf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2avufglfr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xvpcfqex.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hmumsmmg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rvghkfax.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2imuuliqz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2euomgilw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2trphpgvw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2sgckyspu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cbzspzao.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2juuykitj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nuxkngbg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xckbfhit.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ssnefayd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2tulkdofq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxbrgee.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2lqezydaq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qvousriv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vhlqlvxc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lmxcysrk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2imlstini.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmrejdmw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ecwlyrfj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jzbbaheu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2untxpyjo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wbznhntk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rqnzbora.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xgmeexrd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jhwtwmow.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kwktgyan.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2movhnfkx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2arqmswba.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bbxbqqgo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yiqhzlgr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2uutncpil.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ormljscj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wtjagfjr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rceoeutj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ezbvmikh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xpfiouzg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2uhqpikac.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibmxtdir.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nbsjszid.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xkvnndau.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zbuqddrv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2gjflietk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cduipios.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zujitssd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ecewtbkr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hirphzwy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2gbfmfjhc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rdtqokuo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2miiqpsco.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2phxjrmja.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ilelqipn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dfseqoyf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2njhxohen.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wnhfleoq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdiszlsn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gmxzqdoy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rudvbnxo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lrxjrjaz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zmtfzbwo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qhqfwuwg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2osvrdcxm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2weqxquqw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2nxloaihm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2xadglxdk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kxdpjkcb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fhnmlozj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ejywwvfp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2lirquthv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2myejzlpo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iojooxoo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lxjhhmnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzyhnhqd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qsjmmlls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbvbwgdv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hzbmxrok.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pvfysjad.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2czenyenz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2tiavfqzx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lpbnqpuf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xfccnoue.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2drdphqlc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2pdnuxglc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dcvdvyux.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uqbucjoz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mnfzfezz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2baiszmqa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uoqignjp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ndhzrkql.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vaoatqps.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2odeskkbn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2frugrpnq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nrkyayfn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2foekbunk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2avehyhga.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hiynccct.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zwzitgwi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2tyftjsvv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zccxpwda.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zwjtcpay.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2efrlvmeg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ywbytzrk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2twastobh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2srirmahr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lfpsezbd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tctrgdqw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2miyxbcpv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2dnpldoaq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ibqajoiz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yriolkaf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lqswjcqj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lbpmajez.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hxbrzqvp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hkbnwsvb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ipfxkfgq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ghmlvwga.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2cwosewyj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xgulkwll.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ncvfrcnw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2knbjgtfk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mqphymtf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2urxnnhmp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lupbfjdg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jmwxfjxv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2yzphmiyy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2axubncrw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2luyawpkd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dfwhqelq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2umiqboyj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vumfzpnh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2usjzzvkz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lqyymgfb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hecdzhso.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tqjbcqsc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pzvdezcb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ehurepnw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2blspyjoe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kbjesgwx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tllmpawz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2wnxkauwy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jbzjsxrn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2lyjgeyri.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cjmheuyg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wxtsuutr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zjlqzvar.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ptxcxubh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ejvecoga.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rmxbdtgp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2vdgelpxh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2uiggjyvi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2duvqxmrh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gdnghneh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2eliusajj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2degwibpj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xtmfyfyb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vcddoggd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xgmoznyg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bcwwzmsp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hgbgrpjk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ezkylvvd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2txpdygcm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ebfxnrvc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2knmmiogk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2tmscmran.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2grzxxwrs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2nbluqrnm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2unnbmxkz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2crkxnpwa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2eingdbqa.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kxdelqez.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2eomcfikb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxdgduoe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmvgbxvd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktrvcsyu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mjbaysko.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bknwwojh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ieupjaub.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sqtovtum.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jffcvusn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ovttulmj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2waxoqxia.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qrkndqmq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qdysxwin.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cusfytts.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qxrrttsh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2puqxajjf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hmahmbza.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kjbvgboy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ywdoxryp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yepwcdid.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2bbffpnln.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dwchzeul.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ymxhhtmv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yaqtktlw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2gzytecxv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zkrqjico.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flwzrfhi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ueyoivnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2attqtuet.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xckssqms.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2evfbhxfr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2siogghxr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vxwymvtb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rqjfkfjg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rcsvaluh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xrkdcmnx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2vddburch.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qvbnygpl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wesakqck.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2imlhduag.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ktfxthcn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2fjedfqfa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qembkmvz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bqwuykuw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qskviqmi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vnihhrar.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zkvsuejx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2iuxpiqmk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jecbbyrw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ehxzgsol.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2npynmcps.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dqjgiopo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rwizmuhg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wrqnrbyw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2rtlamfey.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ijirdwmp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2isepwatl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sfncuujs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vubyetcy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2gphiunvt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2imlimzbg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zebnbtqw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jendlkho.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2npebvojz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2alhmcagb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2uqlqvzkm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kesbuabd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2idmbvrad.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2wunecckl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2pqxqttjl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cilutavm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mwrjjzvx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jzzkxbcr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2xoyklaju.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2yfdyxwst.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2cokvfzhn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nhzuohnr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zkvspyfc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2dqnxhcza.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dcffcwrt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2dzzhdczi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2adzfqrew.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2uxsstejq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2rdupfhwz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ieionohz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cuzlqjes.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2svlkrhxq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2dtvidcou.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eihhtfxs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2woetcvll.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2skjygsvx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pzqfaggs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2chdyekkt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ehnijbmi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cwftcvkg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rtbcbmfu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2tpwhzahu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2blwegltz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2gjpmjrll.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jbvnfqci.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2sdphqupr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2yjfievmw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2cihfqnwb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2bkymehyj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2lpfhoboa.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2hzeuqyri.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2euxurzho.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rtluptol.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rgmdkxnh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ahzdjxma.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2axqxhuyk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hqmimudr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2idsfjrjd.html


<!-- 参考信息 -->