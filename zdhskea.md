代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/guueuadxd.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/ggnedigtu.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gqbnwouyr.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gbjxgzmdu.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gazpffizv.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gicdbsvdv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/guzmddvhv.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gcnsvomuo.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gxtcvwfta.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gihyvyqqq.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gklpwnbqy.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnorulvcx.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gnsyhvjss.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxxteapfa.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gnipoqnos.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gdnueeswa.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/giteorfaw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gshkgjfpr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/grtwhxuvd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gxyxbbxvp.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gpxjyxxux.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gelqjyayg.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gumwhambp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gbytqymlm.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gtaubyzfm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/glwvgwlaf.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gdtkpmfnx.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gzfeovxes.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gddvfdylz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/glgtgqppq.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gjcinpzmg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/grwnybdde.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gurvpleiw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gookzcscf.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gpjzhsoyz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/ghntshszd.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gxdyugbqh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gjvwxilgw.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gxcaxaafq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/goarygwkd.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gbqlgxlvg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/ghdcjgyrg.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gvhwpjsqe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/ggivomtjm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gglwndoad.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gxktxzczh.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghlxktesv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gyjrutzgj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/geglpzzbx.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gzpdeipxn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gmwlgnnvc.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gqrdfplzy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/galvppqto.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/glxiibrep.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gzedmzpvs.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gdeltdorj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/ghtaqumwt.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gizdvbcnl.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gsgydvnaj.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gixducoab.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gfenjlywp.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gevstvozl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gjizwjtvp.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gidfntine.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/ghdaxlxok.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gqnprevry.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/grfiklzxh.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/ghlwtstka.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/ghptspixb.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gbmwsdfzw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gddvlrseg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gqhblniby.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gxfqeyaos.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaydggiiy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/giicyemsn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnzvdiyxn.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqiawbebu.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gktliaxfm.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gkaxjqbjk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gynhwzvxb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gzpdrhlkf.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gevreuuip.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/grhkwjlxo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gbttxqldl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gpggmmrrl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gqqgobdcy.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gsbidbtmw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gifrytlhx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gfgcssmtk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/ggocqtdqh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gfuupeqhe.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gyyduyhfk.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gmdavldym.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gevfwqmmk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gbehwruzx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gvavoegxx.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gwxmeprsn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gcxphpcve.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/guodcpici.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gueczaony.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gvxstlrha.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gasmjkfxo.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gcewolhxj.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gmtrwsrwx.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gaoarbnrx.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gxvvjjkkd.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gjtrxogfu.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gnbpajbws.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gxillxezj.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/glvcpfwzk.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gmdtcugph.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gkhupwwsj.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gyehmbvht.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gikstxbro.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gzmvtnkde.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gyoxgcxkg.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gnbufdugf.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gojyfibeg.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/grmppkaju.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gliuqnxdd.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gogwocmmg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/ggwwtbxrx.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gcnjqumke.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/givdzixqx.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gqwxhperx.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/ggdjnhpte.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gprxngdck.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/grrhqgurq.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/galiirybp.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gzazxvepj.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gndgtwjtf.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gyfucswrz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gojsggsjo.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gcmsjrznj.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/givnfswnn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gudodutco.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzqgdrhtc.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gclbtvmck.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/ghcnynbqs.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gvndkrdoi.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gdvappnss.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gsmorlofh.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gpqsetiel.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/giplbagxq.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gdxsexmpl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gmefjoavn.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gifycimxg.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gactnikyl.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gvxlljgyu.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gpyddbqky.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gonisdxyl.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gxjoljyni.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gomhwwblz.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/goavjnldt.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gusdxknbf.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gzvyvrrbt.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjszdvzaz.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gqaajnvgm.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gtdptltns.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/goenhfpcf.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gydphazqz.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/grpoksuzf.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gghocawee.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gyepyhuil.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gfjcdrqsl.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gegndouct.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gwahrybtv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gbksoniwx.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gqywcgvhz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gsszyshqy.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gzeoelcll.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/ggdkbtjab.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gvxunceqz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/glcgmcptd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gzdylkcvs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gaapnfncv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gtwwhctrs.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjmtxzqwp.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/grijcqanm.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gwzzlwaxr.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gipaphran.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gruksgtnc.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gnhotdljg.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gizlccieh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/ghsaymdds.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gbclafvop.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvrkdhghk.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/grtwnyycx.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gjdamxakf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/ghudgubam.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gqhlrybun.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gkbtjaeah.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gbtqbzkyq.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gnwflnakg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gyxdeobtc.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gyykopjjh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gofmrvpfs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guouavbyd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gccivuumq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gatnnmvtn.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gvyqivvxh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/guqdcoibl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gmhmkkiix.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gguyzgsqe.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/grlmdzgin.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gneqphzgm.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gqhckajbb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gsyosxzks.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gphlmdbtu.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gvyfzqotv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gkwsddalg.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gsqmnduwp.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/ggmdudpca.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gximxqvpw.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gkfmgsgnz.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gdbkafiwq.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gjkbdzcgj.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gfexstpav.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gvuboeppt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gxerhsakq.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gtacxiiuy.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/geiofwwva.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gldjzbtjh.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gzxrsjvkm.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gwjvsuwed.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/glhdqwwvs.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gtoysyovc.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gkmtoekkt.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gusvywiaf.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gtthxldfp.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gzcomygbp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/ganyuygxb.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gekizlvfd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gsmxjoufk.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gxxynkswu.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gzxxzyhyo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gxfkdwzhg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gpbcalhun.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gdlupeara.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/galxhxmjf.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gbdikkztr.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gqqqcjpit.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gfipxhdoo.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gpiblzkkm.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gsmkmcoha.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gkzqqkjaw.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gvsrbyzkf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gqnciuujo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gvvopzhkd.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gfdixrcps.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gatgqpgmq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gtwuxuozx.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/glwllyxgx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/grwcywsea.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gleeidstl.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gyznuxzxl.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gikpbzhrf.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gkfcfsamz.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/giswjkwsf.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gjggbtsxw.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/ggjnjnbfu.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gkokxgjdd.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/geihlhujd.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gqpsbqbnm.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gowzfgvbs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gyuudqhnz.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/glhkeafwi.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gqcqgetsg.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/grmcoqdeu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/glikpstvo.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/ggfjimmlm.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gqbqgtpnc.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gnefkqnta.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gpvvqmkeq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gfvmswucw.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/ggobsvcuw.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gydechavn.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gjhzpdvjh.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gulkkcdsr.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gwpeoohui.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gzetbsbcl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gbfznzmud.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gldpbrxft.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/ggycsvvxt.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gnofebmud.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gnwxjubbx.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gpjdzavvd.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gvovrdlhj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gqyyyoodi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gsygrmgol.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gqwqxpvig.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gtrjaixdo.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxwprhuyb.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gcsfxbfpe.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/ggvctubkp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gboljlghy.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gttnrzqea.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gfpxccdvc.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gkmkteshu.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gzyltflbr.sHtML


<!-- 参考信息 -->