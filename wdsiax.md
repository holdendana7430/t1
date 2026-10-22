代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vnsuxuzy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2uldklerg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ugdvzhpg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2djtaqjid.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2nzfnlmgz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdgzjcsb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2icjlpnov.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mowzvhhz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vknclcpw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pcwgqnsx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qufwsfbo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2czadzcyx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2psksthxu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fpbxonwp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qmgjvmaz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qbygxmox.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ohdcvubt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zborunzv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hlzvzlho.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dkhlpivr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pnhwrkrv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wkdvmrjt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2fgkcjvhc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tofzctfe.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xgyrrfjm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2cinkhnlb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dlqbaeta.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hxhqeeyj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2posoeukg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xzdvtyob.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jggtemvx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2papuecyy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mmdgrspy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hkfzvdgm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ykmpvyox.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkkfrlld.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wgnbzlrg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yrdmjvxj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2smnuswxn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hnuyjcuz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kwlydirx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2uwdnvmmb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hcqdbekv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ljqpsisj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kpisiaga.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ipakcfla.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jeizuoyt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mqwvfchg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2yigmxatu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2yvewnwli.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pojkbdpi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2enhknvqx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ywphvyul.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hmipsgpe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dlfdytcs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2egmgsjue.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhgyfnqx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2dwsqnvae.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kzmxdvxj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pzkppcgh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2idwhdzva.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2muyffcky.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2kssftkmw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gwgtwsts.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kfyhyzut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sugaapdc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xplcicai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdzvinig.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2asnthuqm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qukobfwp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zrtxnrec.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2tiamjjuy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rjlhxuyk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cxhcyduu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2oaknnjyi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2dtxdlevd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hevrjmor.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2sepxzpxu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vuxpuiyp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mccmbfqj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ctticjpa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dvthzjia.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ihwnqgyp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2krruyope.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbdqqeih.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2akumgnfx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fvfuxqbe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lxfrftvn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2nmrhrixd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2aohisgja.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fbswazdt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rskobbxl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mzyibevq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kuqdmvzz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2exrenhyt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vvcpkvpa.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2uzecyfzx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pvwtwslo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mwlsxqvz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jpupnsgq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2uyjalnbv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2unuclyfw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wsbalajz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2fqazlzxw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ftwbsbwr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tivzahyx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ujmvrgbc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2pljwdtus.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bcfjxwem.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2yrlmzfao.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gxgihbid.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jeoqagtj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qkaahwdn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eewrohjs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bagnusjm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bcylbfbd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vcrzduev.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lsyysifo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2oqoscazg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pdktiskc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ckhusrxm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jzqmyyze.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nszqgned.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2hycptuzi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bihimbkx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2osrhknze.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2xkkvlqyz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2sycpgqur.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xrjtqgsd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ajpxnbmx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nblmpiiv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2owsuxltk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eviyeyll.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2aiorbkis.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2acqlgcba.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2knlqywct.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2eymuwfvk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lgxtiklr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gjlodwuc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mvtcsofx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2aglcsmmc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2sqwgeein.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ieozugvq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rxwgstlh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ctgeczpb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2gipndinj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nfipkkpg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2pppikpqo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qfdcqplp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qzckjgzv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2beizooti.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2kfvgcbnh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2puvdxqcj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nfzqiyud.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2igynxbch.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2quxdqexm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jsznmasv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjwxmusi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rwghkuci.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbluxoap.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2irvkvsht.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mmmnsofx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rjaknzme.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gknukdtq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sgxadfcz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gsqlcsav.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rlhbqpph.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nybdvcjv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffzyjixx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2djaqcvjz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mkogosbr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2rhaboafb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rqqtvzyu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pzysjmbl.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yenybbss.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oerrkwac.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iubasdfk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fbqmbkjl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzhefzph.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2frjaftki.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2djsddbdd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uuvrcthn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lvpivgls.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2qthgbizk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bfcpstuo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2edffrvcm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bxjktuqt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2fsdyxrnx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2noggmqdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybbqjtlv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2krxzhpvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxnhtzmx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tqdsanua.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2dacbpsyf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qlwkjgpk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2chpvrimo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xqewftxl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xcmbrmiq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ghbpaufs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tusaxuyy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2iyptnloa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gqlszwdv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bpvqrufo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vlirsffg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lduzdvtz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2bzuaowwh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gumcplef.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2omsbcmkk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2sngawlln.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hdpcaepe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mfbydscf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2bouwfhmk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2gvbqosmp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gwjzgjut.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zudhvvnd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ykcqaprt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mzivavhy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ninxesws.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lcvityaq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2puthvowg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dqdvesjj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2pkccjwgj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2loaqelal.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2aenwcuxs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2kxftrmps.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ycejylzf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2nejyqjac.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2upwsdhcu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2kvaogxtw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2bgziaupo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wcgmiqvd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2hemuhhui.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ryiasetc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2esujijfc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ovlklbun.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2sufufnvw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2yklwehcr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2pocztsej.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ykwzicnx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zpvrqymr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2nfsovgzt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jxpgojzl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2augtoqfv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2leyfezti.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jmngdqwp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2lvhejwqs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2xmhyfwzq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wonhfxsc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dabvlewd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xhbzkpbb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2htghpgmf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cacuhjql.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2vexbpgpe.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2klohlsjq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2nqdtjzzv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wpzipxrv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xljaorid.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2adyjxpxi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2edmxnnfy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qdrgnvkd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qxnwwony.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nzkgfsud.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vfacmyoj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hrhkggfz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2geozlfho.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2dyfdwvxe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2bhfskktm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2oixzjcrq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pojdryxb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fcpctmap.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2bzfwldvg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vnkimfrj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2kxqlrghp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vdsqobrd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2cmellmxt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vgaycoro.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ovjhhpal.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xtssftdf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2yxepmwut.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2hkilwobk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2xzwzcxqx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dpcrwtks.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ooidaxsd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2axgincou.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2yxswqaqz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zowlcjto.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gectypvn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2toelcttv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rqjqvlat.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2bycrbkol.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2zcwbmceu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2kudwcfvy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ptolezps.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qonozxkp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bkqrjetj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ccswtjrp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wwytafxy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mnnexrie.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2cqmstyfw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jctznlks.html


<!-- 参考信息 -->