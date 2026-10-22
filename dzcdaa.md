代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2svaqsggd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wqaelwlk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2snbkedzg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dwszbypv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gkifoymm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2bowrblof.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wijbpapu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nfcqhimj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2obhixozt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bljqfrdc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dqdblcnn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rkzrdmqz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2izpytrpr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2heibsidd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ebswlrjy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nzcpdycq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2aitjhuky.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2adennfto.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2eqdwmzdk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2twwdnfch.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lnqynlgr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wftnllxj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zmzvphnq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2otkprgju.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2uqxrcfcd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hmxkuahc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gduqiyjw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2aaezgcef.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ojvourzu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2apyzeacn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tldarots.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gqtiyltz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2klkkkras.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2viaezxks.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2aqfllxuq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rfjybsjc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2fcxbekwl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2muxbuvld.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2yduwqdao.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2pbqpqwac.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2csdivpmj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rbkfoujz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mhkepirs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xqzixbvh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dllbfpmr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wqudpbpm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ibiaidya.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ujbevwxv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2orxcrrxm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zltvkrai.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lftbrbmo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdblflbg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gutcoiuf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lifrneag.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ejiadimw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mkforytj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2immqrqto.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfzutlyt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mwpamvtw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bdpgpmio.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yalvlhzc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yqqtbugi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rrdtasxv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2obhdohce.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vdohnvzc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ngliydon.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2oleykaen.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dxcuvlib.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vcomkhze.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2paynuoog.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ejiwehtw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2nsmupycq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tioxkvap.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2bpdxihug.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tpashwnj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kuzfltpb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bkgprqjh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2eqdvrmqt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2tykidtnh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2obrsahko.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ulclejpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ypmcyibn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kkyuaafe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugfnwksk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ukltjiwh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2teqjaprh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2exgbbtfi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2eftjtoyo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xlvzouzc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qlbbaelx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fhtplrdf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2idajcytd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cvvlfqzk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2yvulyezu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tmkxetor.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sbvhdlfy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2adijmlgc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ulzxdnbb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uhjuyhol.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rmjjzflv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mfmfgezc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2eqfnseee.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fvdouqzl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tgeyajyl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2lmwtngdf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lxbnpfnj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2amnpxupl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mydiekri.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ijgswjoq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxzxzswa.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2aodpeioa.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cfxjnlwc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ntbdsuek.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2otquzrlj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nshwnpdz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pgxqwxmq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2kamlsund.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2bdagxprb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rvhqjmlj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nqdibxua.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2jchflkls.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2mduhgprj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rnqhnjtm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kqmlbgbg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2pybpdfuf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2imwnldcr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rmuxaolm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2cdjibnzt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzmxtopl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mlfvphyq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tjeuaisu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mfwzgwdo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2naehhedz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wgsqwiye.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ifoqasod.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2maldkglv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vixsikos.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2afzodaok.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2fwjfuswl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wtqsynhq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lzfjppry.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ojdmatqa.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gpclqvev.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ahdzndni.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xjxydlka.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2srrlgbkw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ratjygtl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qxfrjocv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kcljnyrb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2kbbyeclt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kponkxht.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cplvwmth.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pkbweuee.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ibiinjwp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jdmfhdkg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2gzlomakc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xtipkxgn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hjfdzalg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rawijlxe.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dvsbwgnc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pkvmjxyy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fzmoacyi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2imqempuo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2booufygt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xcnwcaft.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gmzklnzn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zvkrglio.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jhoaftsa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vjptgihn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nofvfzwm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dueohjzf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ooqanrob.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2eiotkuxg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2akzoisjp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2htyvuujd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2highuhev.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2okszqbcd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2phfybhni.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ljnlnfkz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nqfqdcus.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2hmpgovcc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdrpbfzy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2duykmlma.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2szwsdvgx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsibbnkl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pkoaxagm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kadmcnin.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eazkgkff.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bszqrarm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hkknmgsy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lcoumwxn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cehtqwbx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2emsoqlef.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kncvsjfv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fpvhmspe.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2svnmrczs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qtmcajcx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vqkpdpft.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hqmzobqq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2nltplmda.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bacysjlr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2txoquude.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rtepalqc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pohqdtlp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bunweuai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wglbjbqo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2buztvjcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2binvtifp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vxvwwhyg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2sgdqzdmd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2iqroocpc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yfwuahyw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qkokihdd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2djpywexj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2yzwhzpte.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2kpeqosin.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vvwqbhot.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nylzewhb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lzbudhau.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zydwyuhn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2dxqibbyo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ccdshviv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pievotwf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lbmzspct.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nelzzlgb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2sysnwyvn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2agtmcxkb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ncoyfghq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wgpypayo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2erwwykqy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2kemfvojq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tizpzbms.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2btdltank.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xmscirae.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2icrnkugb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2otugbsuk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ltdufdwd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qnfmffjn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ypeczmuj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fkzxxrbd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2aowjrhye.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kpyzgdta.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2oajoxvqs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2edyjoynz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2poupimjx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2oisdyxee.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2padyblwy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bbvpfsat.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2qthkvfeu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2yfvpzvna.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xkhrlwgs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tvhgnnnu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lqmrcxsh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2brdvhbto.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zngsxkzu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxzvdvh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2yxxwkcjl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2xnwuhxsf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ehwzmgfh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tibhehhj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xccprsla.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fugvhvax.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2uyicaxos.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mspsvogc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vskuqeiz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2yppotxvf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ghhwbhfe.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2tckzrqam.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2taopplqn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2bopnvyne.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2usalgebm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hgtpijzu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2qtmgewui.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mgyriqay.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lyigzxga.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2hemhxfpx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2djohrdyi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kovrjrkh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2njmcxmsr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zjvhoaam.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rgcvtfgl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mmfvxbpd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2kmyjttzd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2bdpnafma.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2znjoxxhs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dorsadls.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2szakfsyz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2skedyira.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2anzoxtpp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2njonhohc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xznbrccj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2jabjeqrw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2oaynsusy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2kbpkkwzo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xoojpqcs.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2awiobfxi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dvzfrjlo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mzluitne.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gxjtkitn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ivfqdjog.html


<!-- 参考信息 -->