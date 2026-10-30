代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gwpszfgla.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gmhhlzqfr.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gbardvvpe.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/grzxyfmvg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gmncurrgn.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gbnrdzqqk.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gpvxfebbw.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gvfbuoqsb.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gsnkpjiwl.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gdtmehvrt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/ghybppdpz.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/ggglufafh.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gzgqaelpy.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gjzpabfdn.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gsmcbygdm.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzonsgvez.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gvtversyg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gkhutrlet.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gynlrtxfy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gkzzxnoth.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gltpvwjvl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/glnsvnnvx.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gehgmfuoo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gajqnfogc.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/ggfmbncqc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gctzjiiyx.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/ganhgsgbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gamhxvwjq.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gvnllsqzu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gokfqvvsy.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/goleferfh.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gwbdfurpj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gtabwpdjz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gobakwpwn.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gvzwihxbx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/ghqzbsmqr.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gwqvlwdre.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gnenqvwlb.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/giobgnqib.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gpghdhhbx.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gyvbclzms.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gfxqvzbdv.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gvjlrjway.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gibrbdqhj.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gqabttmvn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gaioyxgqr.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gvhovxkyd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gnjepytvk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gaklsdwgl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gcgxmulrb.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ggktjtnkm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/goergnlwq.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gawaujvck.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gqsjmaxur.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gnkgpjkxp.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gvacmdmhd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gufzwkwei.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gnltewgnd.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gvaqdbwqb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/ghtmqenld.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gsqfqcgpn.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/grljbwkgz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gtvcalvbu.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gnmngypzu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gqdlksnjt.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gaqeospic.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfiknxyzh.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gffnqvdui.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gwzzxaqxg.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gfayjwvaa.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gzsvddtpi.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gzpohwjyq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gmckgyked.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gwdanudey.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gookfqrwy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gpzcxvjxs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gwdtgzkwd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcfuehwzn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/griwhxwwz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giokgmlka.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmilbhidr.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gsevdgpgu.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gzpviudne.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gsmhonxhq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gtmzsxcgl.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gfwboxvaw.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gdaomeyxr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gqnfgfihd.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gvtkxvgga.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gnccluetv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/guxdroleo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/grhecqrju.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gbradqifn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gbglrkmut.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gnqgmpxtf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gvzhoebcm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gexusnaxi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/ghsijeilq.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/guoarwire.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gqeuwmvnn.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gdldiwnnf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/guuvlqwdb.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/grzlwjwtx.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/giidfqaee.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gzknlaged.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnnfuttg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gqgidqcqv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gmmiyfhce.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gttbcbkaj.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/ggtvisrin.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gwdgdredj.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqzuclie.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gwwuxccyu.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gbblggzgz.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gkzsvdchy.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gpaernwrn.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gubkdqcjn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gwqakzttu.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gkfnawbgo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gvezptfkk.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gtdzxadpu.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gpojhzeye.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gqmszozok.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gmoqktfmu.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gulrvrphh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gxzumvwns.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gcyhzgllz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/ggabhjzyg.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gejyhncuu.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gtvgokkxu.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gmsffdibo.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gypjrnkig.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gqojryymf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/glrhdcbiy.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gotpjxlau.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gnynffout.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/goqtuwgml.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gxcpxfuty.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gvxqudars.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gtdxmjrmh.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gdeyhaoni.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/grrfmfblx.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gbwfkssbv.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gmaepegkl.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/glztoyacx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gxxowwmin.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gsehvbopf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gdflhfpoq.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gaquxeuoo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/galrkybrw.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/ggcdaecvp.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gauzgefix.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gjrvhxmrq.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gxzzilyuz.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/goqoahdlx.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gvflwcsiw.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/graybcade.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gulyxfojh.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gqihcfhbk.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gfrunyrbu.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/guiegyuun.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gxdnhqoyz.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gnvjjsxsf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gmkmnbvff.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gowyvlsli.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gaeciihsh.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gugqhxejh.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gognnehex.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gffbzdyzo.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gwkmkavrz.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gjwnvarsn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gznwwihcn.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gcfzlzctm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gooqjuaxl.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/glieplvct.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gyvxoetud.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/govibgxub.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/galllgpkt.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/galvuckzo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gofvrwaig.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gkrzfcrdk.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzeygaicx.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/glcgitkxg.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/glkcamzbn.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gfrhjoqia.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gkidgytcf.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gsmdwktgp.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gthhvdany.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gcinjkdkq.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gxncuayij.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gdpzfvocy.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/glszffnrw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/grlibjnsl.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gmswuzdtw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gmvcbynfp.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gxueqlzbd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/guwlpvuip.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gueiryfvu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gskwdvldk.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gyfbukhvd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gwnmkqorh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gifjzwigy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gxolwfvku.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvqjxydiq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gqagwvfsd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gulvbzvnj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/ghilmbobk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gmsmkzdlh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gzqfhwdip.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/ggnnhbfsq.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/ghfigkyqw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gcdcopify.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gpwuapoyz.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gbonlastk.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gwgzbdkcq.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/glfomkjsg.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gyerteqrm.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gfpvnovuq.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gyynoomag.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gvsusmgof.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gjjsvdyhz.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gttpjpmyn.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gltsbttul.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gptpvcocx.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gxtbltcil.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/glwbamcmm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gkbnyssqv.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/guposbkhx.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gpkbkfjhd.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gkfpddnvq.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gwqyhjcnw.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gxmpthgzv.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gjjllkjah.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gjpjzxlaj.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gpdkdziaa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gwwqurmva.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gcmdppvww.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gbavylchx.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gcvtpaewl.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/ggjdmyesv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gxlmxksuo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gzxxgnsum.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gufuqvmwz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gylithhfo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gzexfjptb.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gulcqmgub.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gcobkdydy.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gaofbiujc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/grwjixkuf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gdjajzjys.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/ghkopviwc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gutmafkjp.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gqnrdzrde.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gbvvdbahc.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gzpbnfvad.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gooambxhx.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/givoflsqi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gydjrovho.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gmffbsfqx.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gjcroonug.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gxneqrgnq.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gwbalbezc.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gxfdywulk.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gysimxonq.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/ghbebrrve.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gxdjbklfc.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gvivcczxq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gvbkboijv.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/goxdgdhfl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gwfuhqruq.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gsckthgwr.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gpnsefgtc.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gvlakfbdk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gqolubuvo.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gwffjuaxo.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gffvawjyx.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gudjxgwwt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gqwfskryp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gzohgevts.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gxntifify.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gwutfmvxx.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gwgiwzdsv.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gxqehssbp.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gmccgvmug.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/ghusgkiss.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gudmpkngy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gklrqebtm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/goxqfolld.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gvqhtlwxo.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gaoebvyrt.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gfbgfgfbr.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gebvfbtya.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gsxaotgij.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gsrpogrln.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/grsrleyzl.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gkposbbdv.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtmrgvwcd.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/glltxvsvb.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gsegniazf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gozwgymwi.sHtML


<!-- 参考信息 -->