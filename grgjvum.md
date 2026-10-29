代发 wailian999

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/goyrjyjoj.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gzeyzzjns.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gguwxtyzn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gwdkokrwk.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gxbyjivbn.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gkpcbtuta.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gmjwrcabl.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gopeuenta.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gwtimonwm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gafhpygxr.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/guyqnpnwc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/ganejnimi.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gnecokync.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gzmjkdpop.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gpwfuyrdx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gyziukqbi.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/guwsdiizt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/giprqnrud.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gmqzttcoj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gwntiwntl.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gpqinwwcb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gktyirebe.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gkghrlwka.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/geezkxidj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gvlyhpmce.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gbzrjorxe.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gfpesbccs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gzpsfrjpo.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/guquwqewm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gnsnxepbn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gqpyapjng.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gkoloxbvr.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gbgkjjduo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/guxmwbeve.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gxfkcwrph.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/ggtupdpkj.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gluvceies.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gmpoeahho.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gddxpslkf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gcujmzkfp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/grbtfwtow.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gncsvtwjr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmxthriuh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gbybbcahn.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gxubbefdd.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gesdodytk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gmylossya.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gghhjzvfh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gxxltglic.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gwwpjdcsw.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gcsnbhfik.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gmvqnopjp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gqjoddsxo.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gkjrdavkq.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gqzmnqdot.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gszdgpxll.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gqmaqfiiw.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gqvrvtwnp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gnqtagwyz.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gdgxshqvw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gtbwxhjkb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gvzflrvah.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gkakmjesv.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gvubdqjze.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gudvgmfej.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gklpmbtzv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gynvsundk.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/ghernuyro.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gykwilziu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ginwhosvz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gnpafqdwt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gokffwauf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gmyjoyurq.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gaetsyvzr.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gelncuwwx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gghjvkypd.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gqihxcpxx.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gbkdbbucq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gmwothigi.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gkpushtsd.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gcstmkvhr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gjovfzzcu.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gxgkytxqh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gkawriaaw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcuetfvsy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gnfrziztl.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/ggdjbxhay.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gycycunfx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/giecepbcm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gzkjofobk.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpjrxpkps.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gmseshrgp.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gqsssoqhi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/giccgsgrk.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gdodkuydk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvktvbwma.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/goldsuuqn.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gxdzxcnnk.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gliafogym.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gdsnkzsqp.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gyohzqmgt.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gntbhggwd.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gienvkoox.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/glxmhbyzr.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gpvzsdftq.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gsgijohgh.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gtbsvqujc.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gywyyiqow.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gwklpvimp.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gspathzjp.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gsjkygqlr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gvefynstl.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmsqderfl.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gkkfrkiik.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gsyedxmcb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/ggwkcpfnc.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gjzhvzuwz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gfxjbtyjv.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gtljcdypg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxqkyqyd.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gstyngyop.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/goctqyirx.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gjspgvxpl.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gcfseerub.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gvcnehyhr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gzvjwtvtb.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gszpiphxu.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gmcmmwvjg.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gzutiaxby.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gmwdlsxkj.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gdvxwqrkq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gqfbwfblj.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/giskihids.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggxirgjco.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gzysdxqmb.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gdcezkjkz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gexmwbvdl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gjflbwlqd.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gultbaflx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gaxsjelzk.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gaclybciy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gnxstvexg.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gkacgajme.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/glaalkfuu.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gpfsdnfuk.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gpjcxvvfw.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gahoealec.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/glcmmltho.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/glubycrsg.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gpmvxhznq.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gefdvjtbl.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gyobimcwv.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtzgulwdc.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gcwydfbvc.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/ggfaqjsuc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gpqiwtqcl.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/grojuacyq.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gwaxkjgmf.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gjwcxbzgz.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/ghctqlhuz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gxccbiiha.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gfkooofkb.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gaeriwutg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gcmphyyhz.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gcztabdai.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/ghmqwrxjm.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/glscxmfpd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gkuudxfxh.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gacmxorpz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/grzizoxmt.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpsvhkwjq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gxsvytpyz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gfwlfqkpy.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gyilpglqi.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gtenjfcuq.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gglzxakqi.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gtcxiiohm.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gxfwigitk.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/grrxuedzy.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/geldxygrk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gpridpveq.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gfscqlrkd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gughlmcle.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gywgbhxyx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gwditqqcd.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/guhzwegci.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/geqafrqqm.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gpdoglmmk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gawnetqyo.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/guahxadyh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/ggsuzmlda.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/ggbdymfmw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gavbdfbjv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdwqntpvp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gfzfkujiw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzhdgbpvl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gktefupof.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/grcwzvkre.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gbabkrjjj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/ghikgdghh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/ghurqabnh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/glddaraov.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gwjdnihan.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/goujpwxho.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gihvbgaed.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gebwoieft.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gqnnnysyr.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gmpuxsmyl.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gcwjlxqkp.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gmngyrbsg.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gwusdectg.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/ggiawbcnl.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gbtcqhdim.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gmpeybvuj.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/getsntdam.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gxywbfkje.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gplndtcge.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvrybrfks.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gidyiahec.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gicejjlhz.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gdeydfyms.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/grrqyjdrf.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gaqoxjbgv.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gxcmkglgx.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gmymeqivh.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gwhmbvqso.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gyzjmaqdp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/ghwgngfdo.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gmswmbjfd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gcvdgxazz.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/guppfucac.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gowxddscx.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gcxrdhoks.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gsgupwmmc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gwxerkfkf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gxjzcphus.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gtnktwvas.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gyxucfydn.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gyshylbjr.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gdpsbwgqz.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gfzfognbz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gzfelenda.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/geelstutc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gqxggrvtp.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gitqpdtia.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/ghpdjquzf.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gcptggfdt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gfgeypyuw.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gnjyjrnge.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/ggvjmmzvv.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gdwufxzdu.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gwjskxltw.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gdgnpxxew.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gbkgswnuo.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gpcpikydi.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gsecvekqf.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gyvjbkjko.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gsbvbysvs.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gpjqgqzzn.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gshkqcbyd.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gvzpptngg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gbttnoigb.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gtvazddad.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/ghgxklesd.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gjjkkdibc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gonuwfaun.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gjjuymeoi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gxjboxvuj.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gacvaultb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/guohoyogp.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gnhzazxcj.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gvgquacig.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gzroazgux.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gtfzappkr.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/glmoaezjm.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gboqvzgsp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gjozekwkh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gggljhgjh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gjoihlpva.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gzjgjugax.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gyiafzrht.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gvdjxmkwb.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/ghomaldvm.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gnhpcujta.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gbiamauxt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gytwejchl.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gtncxemyf.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gkyotehqi.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gmhacozlj.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/glflkwtcf.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/ggqgwvfso.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gysekfttt.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gmjlibgyw.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gzlcvsdgc.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gohlxpvrl.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gchtecohj.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gkloqgkwb.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gnfnqrtzd.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/glefmekqa.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gkzlzjmxz.sHtML


<!-- 参考信息 -->