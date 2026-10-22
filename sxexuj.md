代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wfnzyhxc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2khpokrmj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tbejemih.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wxlguope.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dwqsghwo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fzbjzkpy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vgjkduai.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qrdktpje.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ztkmheik.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pgzqvmck.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uhciezeg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2eyaxuzli.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pqcwkpbd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lzacwmjy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qlqdjpdm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2akungdes.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2slbypbaq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yrkasshv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ajesnbof.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zaiulrcj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2aptzricb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ytqkiwrg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2frovlxmr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nnjdpiwi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2awqhypnn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fgfjsyjn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zbjoyfvm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vjxbdadq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hhtacwjl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ropahrbl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xebegfze.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wakofqah.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2wqjbaeqc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fjcxxett.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vdeyqhlq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2rlvojkyw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2isflujvh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vmtvfwcv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2bqmwmpek.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ebextqnx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xfwdevmf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2yezkhzfj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ivovuzxt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wyfjmixp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rpetmqxg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bponecyq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oaskhqnr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2spriblwi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dwelgxor.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2eteigwrc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xvsnybie.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jfkxlfcb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2udxbdjun.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gksutbky.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pgxizjwr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lckmclhc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bgdgvsvo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wnoifwoh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lxzqredh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jevwekut.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujptnwlx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2psmnaxdf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lrttrgup.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wiaqvdwb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qfysfeoy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ofjujryy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rtsrzdhh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hijhbiph.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2htlwppib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvewfonq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fxldbjce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htnojndx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ksbpdryq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2itkrejtg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pffdeitm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2yedsxohr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2swlorngw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2snfziybo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2sooynzpa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2daojfgvz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2unvvflpn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tdwsfpsr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hiadyygw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cslfynkl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2otparywk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2oseaarou.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ntbxrtoz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2asbxnoti.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojsnrguc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2acyabiob.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dquwjoex.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2atlmssup.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2mpjkdorv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2omfcgxxe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2tmlkiafs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2snjsfgae.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qtsoznse.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2thutbiap.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2acodmxwv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dvmcvmux.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2txxzwbos.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mzpcjpvh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bkzlzlxw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ckytfeih.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ogcuxnow.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qmnphsze.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mhegovzc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kpjpqtzu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2utilsjkt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jobsatmd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mjqzlqks.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwpsqga.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qwslmrxn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2inzbcziv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2bpgnlqqh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2weaasekv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wudmlxzs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lucswwps.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ppnpgkhd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kpgvifgd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2zcmhrczf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tmtymxrt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bagubpwz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jnzmzkkl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mfxcumij.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2cmtshrhx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yltfquqi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2diywxrkz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mdnaycnv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rkqrjdta.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2lbiheety.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cykwompo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uyhecfxo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cxzqghtp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jettddda.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qhtssdcm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bxtzoncj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2xksytoeg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nhgxxkfy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zfqixamd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ajhfoknl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2erzyftvm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2vqxdkmgw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bahwujfz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pdvumboe.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2zzzicigz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2btawjgrf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tftqmcsu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sddssxjg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fgzqhslq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qnzaqmub.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2bfehhgrc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mqtvshfj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aopvpmtg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jbzeobss.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xfnoqffj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2duecdhrk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wcacqbyg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gxkgkbty.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjddatwf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rcsvwmol.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahwdpwjn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2opiqdegv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2kmpmdvrf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xodlqwfc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wnttlqgo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gvzeancf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kllsuwzd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymukodgs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2siwkxgfy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vhteking.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mlugwqgg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2getjtqab.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hxlzvtvj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fgeazifj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2sczfxloq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2eserahhp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2swdtwlib.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tpxosujw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2isuemdhv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ksckuzdn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tnwxumso.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxcofgrm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lxeyyzbs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fgllynet.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2auxcfruz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bgmornls.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2leodowcm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ljdcbqnk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gzqmhwto.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hljxsdyp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hjvdeegx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ltawjgko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uujvsrih.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jfeklrbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2loezyvls.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jngctjme.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uyxbjlsh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2zkwhkddf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qkfpuauh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2taenvnrg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nltabiap.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2stwvaqkr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2eowdxpnz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ujqkiysn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gpuewfbr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wofvcnki.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lghcdxkk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pdlywhxf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2khnusglg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jveaqwdf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2sgkbkcxh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2bybpoqqt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ehcotcxg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jczussxu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xqluicez.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bdcmtpqv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2zatspfxv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wdnphlsx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gizcpcwx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wnrjdzrr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2gbchjsjd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2adkwkvwv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2bytgqxcf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2khapozim.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2endddmxt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2npebjapd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ghvxkgpr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2vkevquqr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fgytgklt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2qoxmzpxs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ndjujoib.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2yubgvymo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwssfqvx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2okhvhrpr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ovxrtugs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hyceumzq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mzgwwozr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rjoqzevm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2yhjzrmcd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cttwkbpu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2svbxifik.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tgixaxux.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wzocwvns.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2tohukfpc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2tpoljfey.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2gmnsiite.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2kbordkdc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ojrqdmje.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fekdqffe.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2oosbqgkd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2rsieioon.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vdltmzxw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2uzjxuukp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2puwgtvdt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lkfxkxwv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hgpiedrj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2veonasrc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2leyluzot.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ogpsffgu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2czecoxrt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xssgyruq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ecjmsbqx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vwnwcfbk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kciywgcx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kkwycjud.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qogtgqou.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2sypabqdq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zcizjepn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ydhjqdkd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fswikhht.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2nkcofegt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qmvhxmje.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vsppommd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rmawbcqo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2knvanyxv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2toejmpeh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2pppyuzxx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2svdkzgen.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fowsfnau.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pfbqwcon.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2dtrgdicg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2howatbhk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2gcptvaoe.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zwqpeceb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzoktsdo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bgspcqmv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2uhaknolb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2nvtrzqyd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ppfosveb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fxbnktov.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vjiqvncn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xquwfwdq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2uklpkodq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kopxqtma.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqewvxyi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2knemyqmo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2vurxrmcu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cuqlqscy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gmjeygut.html


<!-- 参考信息 -->