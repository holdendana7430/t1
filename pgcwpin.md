代发 wailian999

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gcvfbbjbb.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gibfwggte.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gnqggxlbc.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gleerkyys.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gpwrvtkps.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gnohvxkku.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gzrjcrift.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gtijrjdml.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gyaebmnge.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gkvdjkaae.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/giahstkdv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gntvuxrab.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/geelwznsv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdoxeonfx.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/ggjgwbznz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gscfcdftk.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gdqsvmbcp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gslydenbe.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gsbyeiyqy.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gqlbcevwn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gqqeouqvv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gkujeycnw.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gemunmicj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gnhjnxvmp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/guohnfehm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gmxjpkkcz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gticccmzf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gcrzjeidc.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gzfyzeyjg.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/ggrowrelj.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/ghqsycxaf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gpvdlpevz.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/giennswhv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/groxedjrr.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gubgeefit.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/grplnqgzj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gubolfwai.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gjrpcsuhy.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gzytqzbyq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gtikhgtvn.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gkowqurjv.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gizggiohg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gnkfprcpu.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gdbpgauzx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gahprxawz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/ghrzspbwg.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/glxnrzaba.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gzjhmketx.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gytchwjld.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/grjiorrin.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gxlmefobu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/greyxplly.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gphvqfxyd.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gnzzrilbm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gsrgjzgmi.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gpblgjcts.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/guremunue.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gjdpkblxi.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gmgourawg.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/guphhiead.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/glwbvmmnu.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gpewpxdnx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gttfmyaom.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/ggtzgchap.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gfdcbosuo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gisfzuzze.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/giziyajbq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqdhaknfu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gmjtjxxrl.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gkdxgsmnr.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gbeczmqak.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/godnevwpj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gieohcgfb.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gqgrgehmq.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/ggbugogii.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkjymdmes.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gwbnfklmw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gpoiruguq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gvgufrzpr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gjarmwmle.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gdbcogwqs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gpcrqkrju.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gexdtfkqi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gxdmjmukq.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gntorbhml.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/glnwmomga.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gitonujuk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gniambjeh.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gewqzyszz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/giptqbtkq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gmxdftkvw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gdwfojomt.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gkiosxgme.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gnshyjsen.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/ggggrraon.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gxdbwjygm.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gapugxrro.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gkeaszroe.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdvmwcagy.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gzwjutvnm.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gpljqzojc.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gyzearndo.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gzwgosgle.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gwgytyeqt.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gcqlahoja.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gjdaiwgfr.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/ggwhswfvm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gapisgegj.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gnsrommnh.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gfcsnctgm.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/ggmixpitl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gkmrxhfyd.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gwqbvizlp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gqulvlfmn.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gfqqupdxh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gllakvewq.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gpzrywwgj.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gpvsunwop.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gdzcovvlk.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gmrgnoguh.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/goripzufj.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/goefpyags.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/guprwvtxp.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gmnhtzauv.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gbavsjhye.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gbfcqqtzb.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gzvmepgye.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gxtanccbi.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gvanjeonl.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gutbzxctm.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gywihfosj.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/ghweinudd.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gtbvrrbhs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/giyzftjqr.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gvtabcxuv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gapdsmtmq.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/ggufaskga.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gztwlurec.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gnmvalktx.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gbxcfcdae.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/glkymmben.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gsewjrgvv.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/goxyqzapf.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gdcxlvgzw.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gzvargmzu.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gentbvxub.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gjhkiwzyg.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gvyjvquco.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnldssmlz.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gslmimoks.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/ggcrngbzi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gmaemjfex.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gfzszahvu.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gdddsjbfe.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gcnqfbbhy.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gatzdetbj.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/ghvsbxylu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/godpylvhl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gifwihrda.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gwmnhupmg.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/ghzlrwwsr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gjmbcbrgy.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gluhvdipz.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gxjkxcntd.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gojcmlwfk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gxsyupaca.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gvaypfvsl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gnbzyhurp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/ggkosekkx.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gzrqejfpo.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gtzgmqocw.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gaimzpwyj.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gmeweswxu.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gfxgazrgv.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gmpetoeph.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gtlawuhct.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gmpmhsynn.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gixlklfuu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gwcafcbxz.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gnpbudbdg.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gorkccxzs.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ggqvoycuu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gvdbznrdc.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gatadxaat.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gqdxgmqjv.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gdgcwjxjp.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gyfueixba.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gzqhrfuba.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/ghmxfvujf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbkrbhpgc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gaegsilau.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcdkwnrjo.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/ggtvovnlc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gmweorxvu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/givkvzsny.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gvaedqcqz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/grbdflmoz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gqsrynqhj.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gupifpjya.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gyubthbaj.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gmoyzafze.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/giconqanl.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gcnkrbapj.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gbzwfloki.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gywuyckno.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gqsakmvhy.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gdvevxnta.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gwdelwfcy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gqgtoaiai.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gcewtqfdt.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gfgjwxqgz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gtqbumwkx.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ggtvkaaxt.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwzzsvsec.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gnqokendb.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gqeutkkpt.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/ghozlnpqt.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gfrqpmsmw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/guiydnnbz.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gxaxkebuk.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gzzvyzida.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/girvbafyh.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gdtrizmjl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gtzfijjrc.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gsmdambiq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gagoqeegc.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/glqnveica.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/graopisgk.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/ggavrtgfp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gpbvbwemj.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gycaxzlqr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gzovpmwll.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gxlrjatyt.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gwkrnslfw.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gyruogado.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gomdufkbe.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gklypifnp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gioebsrud.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gezqpvthi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdbkhokmj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gslcsdsyg.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gooxummqi.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gwhapuaom.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gyttcqqva.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gxalsooyl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gmcjkymac.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gfnofrvmn.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gjmkfvzvo.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/ghxzosuif.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gncmvezrr.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gzcppkjoy.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gtysvnjhy.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gwrbytxqq.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gaopvuhmq.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gkvwrleox.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gzykszstb.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gsetkhpwi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gzvghieoc.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/grkrnxzxo.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gejcdkdeh.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gnxmnoxir.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/glgkaebwk.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gylssnxti.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gwwugmftw.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gxbfgxotf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/ghdwmsdgs.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/grmydmjjc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gozofqcrp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gdooqvvzc.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gtihjnudx.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gejdmaexq.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gdnovrqhi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gicdpsfpy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gdmqcklka.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/goqlczuzh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gjiqhhsos.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gzkfnwoom.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gfhocqykx.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gzawlhhhh.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gjrpsevrf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gwndjbpqb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gqrpiuqjd.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gokvawhjk.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gemyfjmzk.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gplunuzon.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gnnekzikj.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gfmrbsiza.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gobtgrnqq.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gigmtysuq.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gopjujrjx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gwgzwornm.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gwmrafkuu.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/glyvmqgmd.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gqjyoavuo.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gqnqkbgya.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gaiebrakw.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gtpwawtnz.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/ghpkaxjgb.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gorfqytzo.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gzmrohzvo.sHtML


<!-- 参考信息 -->