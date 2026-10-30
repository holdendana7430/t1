代发 wailian999

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gvdyxoyiu.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gmgspzcil.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gtzcefuan.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsrvzmkgh.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/goryhvweq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gejwueosa.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gvqylkudb.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gdvtcdudf.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gwhfjxcpy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/glbqmmoqg.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gzayseeyl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gyngvpwfh.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gtzofpjxw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/grndpzeic.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gautarzgj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gbrjpetvw.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gatjqiyil.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gtqtjhmqs.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/genvirysz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gugqtnlhu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gjhqedfqd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gqqlvvlmz.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/goleokwym.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gfbimlgcx.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/guvjyrwtv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/grgtavovo.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gbfymamnz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gxokuzwmr.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gvkzheaux.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gcagnxrjs.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gjlpsxuwf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gzufjjbis.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gjnvlusqi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gmcgmedys.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gvvtbzzin.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/giepuqcos.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/giuqqjkfh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gbwjffxgo.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gsaiviamz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/giuwhchsu.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gzehkocll.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gdenddymz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gihpiftgx.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gbfdhjcmb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ghruyoizn.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gibjcrxlw.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gxbjgekyd.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gqufraeuv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/glgqpxkqp.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gtcbzzdhc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gleksmrlg.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/ggibrdglt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gsxaeepwi.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gvkotxlos.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gtgelunec.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gehdhrgip.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/goumnlbap.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gqwywyasg.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/guheisvpq.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gssiwjqzk.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/ghilejorq.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gbwnfrnrf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gduntazoy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gfttwbrzs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gcozwvfhm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxtimphex.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gnwqihrfl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxjljmuzu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/ghvheegfe.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/geuoozwho.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gumlcxzri.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gulsboper.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gsgwuwkue.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/grkoqrnjs.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gbmadzjgq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gjosktypy.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gwwbmlhsg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gbxhafday.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gmjhphmvf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gvwyoehhe.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gcizppjit.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gujlbmrzv.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gkxjrazxs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gxdknueai.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gxwftntyz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gnkfivlzt.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gvepjpvvs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gnxnvvwsl.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gemlpzqit.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gvdlgljzq.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/ghjbpdpgg.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gpvqxcjsn.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gydgledhs.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gnuwhhvow.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gcethhoqf.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/grxekiwve.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gzxojrdlx.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gsvzlftnz.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gmzqdabrz.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gsadqagah.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gwgjifqzv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gogursgbc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gwlwtrpre.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gajmojebp.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gtksnorml.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/guvyvydtm.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gnsijabwy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/glwtqcxxh.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/ggrawanbp.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/geblsmyqh.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gxyafzacy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gspeywkmu.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/grhcqjeih.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gugdrzeyc.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/ghgiursov.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gwnzsaapq.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/glpfaouus.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gbfyoskae.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gcoipuzoy.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/glwqyhxsq.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/ggonafdbc.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gwbsrvmwx.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gahyvfgic.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gpxmueodc.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gkiteahoq.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gyylphron.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gosjbwliv.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gftiuladn.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggwcbtwau.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gywfludpe.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/giylidrmx.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gemyxmiyd.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gsuasejim.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gihnvkdtd.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/ghxuthydk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gmorccjij.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gjsatevde.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gmrquytar.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/grgccbhic.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gtpnxmoiu.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gwnkwrjuc.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gbfzyizea.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gafllbkzl.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gpigfsqiv.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gcyvpwmuw.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/glwlwhddr.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gwndmkayn.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gsiynplmq.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtkbfhyou.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/goptzkoae.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gjckktzns.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gtpuwwoia.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ghkjxqhcc.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gortqqbxd.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gqyzzkemk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gepbkbwio.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gvyabzyfj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/glmbbicet.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gzhvqibez.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gzbxlimvh.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gywsptjat.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gotlinpnr.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gbbnqlurr.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/glncjcgfw.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/guqzyfnho.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gpwycnxnu.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gmiakvwha.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/guatsgnxt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gytllkvrd.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gjfqygjbb.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/ganefzehl.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gqpswiani.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gcxwoplhn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxybgqjuv.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gopfohezd.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gsufzfgrt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gewykwlmu.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gwkaolzuk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/ghrlawfsi.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/ghlpwpnrr.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gmspyjzov.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gewtduojw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gbihyvrzq.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gjpunhbcl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gkaxfdgil.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/goxathlns.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/geszrghhg.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gyvjcazab.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gjxogrvaa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goydkugcz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gakwlhtpx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfradrfkf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gcbuozbkm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gdfxmnfxx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gipshyzye.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gqjykayqg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gjocsixaz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gmqghfrao.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gunizgetp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gidvzflfo.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gerkljipl.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/ggdsjbdci.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gycffznyz.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gbnpjlewq.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gfssatzun.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gljpqsvzw.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/ggkotanez.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gvaqkpwtk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gampuejew.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gafmofcfo.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gmirxarkw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gkxzdqreu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gikczextt.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gyoedhprv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gigxloush.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/ghaokzeyq.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/glixpmwjm.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gzliufmlj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gfnwpfpdw.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gipbzzupe.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gusvggnuq.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gicnyysyv.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gyeumxkck.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gnenxtpos.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gwerxumuj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gbconxiyo.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gnmnfyerh.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gbfviudzt.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/guuoyhqmx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gxbnfctwv.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/geiizbtkj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gvawzcaye.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gvlbemxwk.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gxqnyibxs.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gskiybrfg.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gceyoxeuf.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gpgtokpaw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/ggcymxvdt.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gndyznujt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gixzzaywt.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gpmqhlawx.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/grzahzxgs.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gxaxvneuq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gotigwrxi.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/guxvgbzsi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gmdyhcmne.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gsooghtda.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gehfwpvyb.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gljoremcb.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gcsssecbc.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gbbmbfxjh.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gjxmlcevl.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/guoposqju.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gugcasuwf.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gokbmywwq.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gaznwgvou.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/ghvxqiucg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gwbhnagiu.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gyhzjqava.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gtoaekwik.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gwkbybioj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gxufpkbjq.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gigmyjusx.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gavtjnvfb.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/ggamyorwf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gmfkdpbvz.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gubsxheil.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gpiccqjcb.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gkxalyzra.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/glbiodquh.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gawuemecm.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gbddfzywo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gcclmdlrb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/glhaanmgb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gpqhpeayl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/giazsfzcg.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/givmafull.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gacqiooek.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gkovrpuqt.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gyiuiibye.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gidzdraop.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gdjwrcgyk.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/ggovntnuh.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/ghifpidej.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gikdimdmd.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/ggxvxfumm.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gwtmgjycl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gtdloxcgc.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gmiduqlxq.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gzypkzwty.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gazlrezys.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gjwihtrtq.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/giwrfgpdj.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gseecbtnc.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gydpziefo.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gtgcncnsg.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gjnghkfcp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gzrftpauv.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gyjnlkoly.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gzydxabmf.sHtML


<!-- 参考信息 -->