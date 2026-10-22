代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yfpsbigx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kbcglryx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ulkcnijn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fdhzpdbq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fiyuyfzy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2dgqqewvq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ahwmtbei.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jnvdfupf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2smbsichi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hfrpvfmu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2gvumdiqs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bvzdnswo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cvbzhjsd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gkahvvvv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2enjffjbt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zuzzyisj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2usjmaexn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmyafnsb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vranvrpc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2igtbhwvu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ojetnufl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vpeicdau.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2euwcuhim.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vghwnvfj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2kgcewezp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2yrfykhlw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rwhitdcm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qgkqeifu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2brewmsxr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hzbtmvpd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2panlrrdw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jmvcokwj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hrwuooth.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jtuozamj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2nwabxfqe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2pwyzlidn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2aelklblb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2biqgqfuv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bqghbpgz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2loddfbpa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xpdxrogn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2svzfqpgw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2obkrcgau.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ofxiuhek.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zfotblro.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2nnkshddc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ncfcpxxp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ecbihkxj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2itsdnrzh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vpnuyarj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dhiidulq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mzyetrxi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2arozyqdm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2obciimmv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2czkfsxmk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hfcklgwq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cesvyioj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nqdcottv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tejsdgbp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2agidserl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hpzyarnh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2acblqdvt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pzkirege.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2wdmlmzcl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxkaotzu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2adprsvzw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vfbfsfkj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pjamfahg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kbqzfvhb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pxirikjn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ugjbvqzw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kwufhnsi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lcvxumvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahapatcv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hjoknoqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qufceblj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cvmjhizp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2haltanwr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lxkojsqa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nibkpash.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zdussnqh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wysvwryu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ffftkycq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2koirujhh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kndomfns.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gftxrbxc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hmnupqdq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rrcrkatm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zmlguxxn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sowylbgr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2evvxirjd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qpbzbyru.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2svybnqma.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rsegixyr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xdmetodv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2taypihzk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lmnofjxx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2uzcpewmk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2snobhrmj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2skzsftys.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2enyofrmm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgnahcxr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2oovxdmby.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ndamctod.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cwtmpnjq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2zwkgagpt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iiiqudto.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yarkvayl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pnclzcpg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vmafaldh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jyntxsfw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xnwaxqxj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cdmhunqu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zohymjzz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wcxpkuac.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qngdqzcz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2izhwzylj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2lgveufre.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2alglelzr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mgcqxhwt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2rlvbgoqv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rhhdbecv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oqzidjzg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vfsfnkmn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lqsiqtft.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mjcyfuhm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ehvdtebn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ticwkwbl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ymweuahb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cobaugny.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2rzoyhzij.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2espryabm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jsdxuloh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jnlaeahq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2hhkasrtq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2joenjhor.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2szjfjczn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vnolympi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2opuvcnhe.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2mgdwuhpw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nhxnbcvv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zrzfpjei.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sarhqnyd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2whgbbsvp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bsvquwsh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2htrcptoz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gktydqbm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wzylzipd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ptyiixvi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lqogpmvr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fypyijrj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dulvuxvs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dxkuzfde.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2bqkdazik.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mqbtrbrx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2rcytezkd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ihetsakb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xadtdgcz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kxmhsqlx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qjfojrdr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fygcastk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2gquhbqrw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jpqcuhcu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2uyvlvxnn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2snybclcp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2oszbowfc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nfdzgnmo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nazlpcuw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2shloergq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ndkamaib.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2nqxowxwi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wvjcuhsm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lirvdodr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mqywmirh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2phriqmlc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jfdgtyrx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uktxbmtu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hrbwsnpt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kmjbwsbb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2elrwzzcw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2mrrkrsir.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2javrpqah.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xeabktbm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ynicddlb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmskkome.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xitjjkth.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lowmjlip.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2iizdxpay.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bwehrvns.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ltvjqcdw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zkujewty.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2iwlzwcgx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2trbofazp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lmrmgkfe.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eycoieur.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tbiazkzp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hqjqzhgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byroixwa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kmdmqahg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guwawbct.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dxsbmivt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qqvkepml.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ivombqtc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2tonehnes.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2apzvozbw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xzhbzugn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ucncgqlv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2yyzjqkow.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2mbqpwgek.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2flpdgauu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ikffgsxh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kdpgybji.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ebanjbvg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mgboazjr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2bqvjpyeo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2orkhrgda.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xsvsvdkg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wrvwprxx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2gzkoxpca.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2aximugay.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pnwgnoky.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qnhdhsau.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gzyikjko.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2qkspchnb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ybsprshg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vcbrwysq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wiolhmab.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tpdfnnen.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2iprshety.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2rtnzwdkg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lwwxkdsb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2hmayffto.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gigzaiyx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ctcqryof.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qdbsrqog.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2azmnvvrl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ybpxvmdj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ugmndwfo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ndvtcwgq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ixdpmlfe.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2iurfcevt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ixidfthl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qysacsan.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bkpfrexc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hyerwgvj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2vlvsftsz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ebuyhsex.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2enpxucgu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kosylyuc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2siqaotxe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2tyggacsm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ofnbillj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xzaeefuh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2woezjfwt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2casevdml.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2aprvknbs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2kjxjdxmc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2eybxvcgw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2iqphsyuj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xazwkdxt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2urueevbq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gukeziuv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lhcfsxrc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nvlfdccp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ycifvple.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rktwgzzj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2wellqmxs.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wimybpli.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ekcgvtfo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kmgnbavb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ayzdeypv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ppbakzoa.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fuanomal.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mpyqbdbf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2vewnhbgn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2acljmeco.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2jkbctxya.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2qenjoonx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2bylwdaul.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnbpybiy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2eftmaoss.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lxyymbov.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2aaszslzx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qnwwxdis.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ywoezdtz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2upxlluwe.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xnqmsvoi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2xbvghxqp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gabhvktl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fqfyxtll.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2obnnbxtu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2rxirgiqc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bhfqmtey.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hxckevoo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2csdwyemh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrjhbzil.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2dvuswbfv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ukvafivn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2rlchvvpy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2eoejyqqt.html


<!-- 参考信息 -->