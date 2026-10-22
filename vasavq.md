代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mwbenovr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dghgkekq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ojlkwigg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tfuybvfu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aqowhcck.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yluaqgbe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lxpvgxue.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yglfddcq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zhsejqrk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2fvvaipdf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kqwvjpfv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ihvjxxpo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sanfkoeb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2iuipemny.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2npqoumlj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ukrsziiv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2xghnycic.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pwragxco.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fwxuqitc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2jqxgdgcf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fhilakzi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vgbzkthq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dgvlpnqn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kfsyfsln.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gphbexlj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ynfnifwf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vhpvucth.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kextazbd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bljvdhjy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mefwkfhf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2obvevgvl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2itdypyyt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xkrsxjkb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ssflwyyp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nusglnys.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iamummti.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cafhqjjw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2csdgnewr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pymtfipm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xqvzootx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2etrrlgjs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xkfkptej.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2mwafmiih.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzgbypne.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2kjfraexo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cyxxyzbn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ynjtieas.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vcdowizy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qlbclnxs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fxqvlria.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lgpbgztf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zklypedn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ipmjzulw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2olkrarpx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gszjkadm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dlkscmmg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vzfxyubx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tpiacufq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2zcwyjsrc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2yvaarrct.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vpuukhcx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kqtumybh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kjtnksze.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhkfrgcq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2murdktnz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gpjyieow.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tdlburol.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxnjuclw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mihwafdy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2asyeuvqc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2atnsjkan.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nqnbozht.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wqarqdjb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgrxyauy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sxrwgeop.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rzrortqn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eqflepnh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sxsgnbzm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vplsggov.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2iplppmtx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2hidqissm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gzocwvtf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2miowbwkg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bycnojyj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2brdnxcmj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2llighyoy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2akuaaxqn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ypdkfipf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2agixghmf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hftdpztd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xpquoaxk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jixkdpzb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gtrjaogj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fjxntbtv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ruxmvnwp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2uafkmihh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dwrcvxrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufvhhvxw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kilijubh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfhlktfm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2blifjstu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wurwshrr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lovlcmld.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dulzawwm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2akwsvani.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ueqgrjan.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rxmoizal.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yfvegpde.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tkkyyioy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2aohvnaon.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bxgquphk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ghudaqhf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2welfllpy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gebowpyl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2wtfvcpjh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vvhdbupj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvkbfnqd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ccnsumtp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kpvuwrdr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2avkgeswm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wvygqttp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mhzctbsu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2howrcyaa.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zxpssghu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wifcquzk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lyebyude.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vbiunrcv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ksmvtory.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2saumylch.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yxiwvygl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kfnzxxeu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hopqqizm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pmrszxid.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jdqcbppi.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vvwyeawj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2dpsqigfo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2fbgbqywv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kuvxraos.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2lbjpdiys.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wqvbveyq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2euhckpfj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2yswxzicc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2bmouuhee.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dcylaomn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2fmojzgvh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ylpqahti.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pjndruby.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2trrzcdxo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2cxncvnqd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tfnfrggn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rekiincw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wihcdxat.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2imiczjro.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dcmpacpv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zkqlmwou.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pbsoqewc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2whthymmn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hqmcesbw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wghtcodd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2feihitpe.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zcwepvas.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2owofuydp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dpbouejm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2jzeddzde.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nyulfzep.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2uydpbyuo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2unmcdmdo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bnzdrxdw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2qvwxklgx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ukhctcjn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gzumvpjd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ddesnmeq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pyjstsbu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gwaanciu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hfjhhtcl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jfitoxeb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ghblyqng.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fvaoqwrm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cczldwke.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2caalmfbp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2euhainwr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ztjllshi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lvabtvqn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fkxtijwa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uhgvavur.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2almjozoz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ewawyrrq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2cbubpuyp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2nuuritqn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzqcdlqw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2cocckvop.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2uhqiqrsl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2mrkuqypb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yspnkcxi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2twqhkloz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pbnxtlci.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wirizppb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2snebxgfb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cyfmdotk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2buthvyls.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2phdgyvei.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2biaugdaj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mvbmpdez.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2rutoneqb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ciykgcut.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wfebtpzu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vlofxzdv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yzwxnqxw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2dafpdavw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rkwwlrmm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jnsrpojt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2bffiwnoo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rtppidmz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jkodjkjd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pqbqebzt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2cdnfxwbh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2levcdfse.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2gjxzcgaa.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pclxpcgo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ibsnxzxs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ayvtirrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqvabvhu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sghlxpok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cffbynbh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xehkrdmz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jchxevds.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2syormdph.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2gwuldgxn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2iprdhkfm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lsvvjhzm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2opgtdlyi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2hozwucog.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2uzrgtpjk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gmxlpcht.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pjhqvnaq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2czqdehuh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2jevziydw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2juxbhsoo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dhufczkf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2owwawywv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2whyfledr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bkmuqrxj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2rnblputi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zizrxrfl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xpmdnjpl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2legfxtcm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2sfllomez.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cuesxejd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gxwsnvea.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2cruvzxfa.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2plrwrhbb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2besyvfxo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bqexlent.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2zvngglgq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2acqmamop.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2aapwrzpn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2izrvzdez.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2zzgbcbsq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mbojkzaa.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2swalrufl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2deugdldu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2qhpjnjan.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zlgufoha.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2odyqwqzc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jpwtdyld.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ukdewnos.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ceyfrowh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gseugbno.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywnkvhlp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2akrtpryw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2smmhvifi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zhvoqiam.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zpwrwbip.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fmwhskuw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jctljuto.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2oelsnnre.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dfqjxvkl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2owvfonbj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2dmrgzatj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2aoertetj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2yonkgntj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wpawisfh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fxtzbyvs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2nchxtplo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2raizeptq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2vnivzkbf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xsjkscwa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gfnuysyx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2joteluua.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ppjcrsgm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2dwrqxbwe.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2smtssqlh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2igbpeytj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2urlftglz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2btqwogcm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2useebldb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ewuymlkw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ehabqoqa.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fzpzykmz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dxctenwa.html


<!-- 参考信息 -->