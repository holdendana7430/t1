代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gscajmugm.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/ggkafnowm.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gzzaknruy.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/grchqulsh.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gqknbscip.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gmdjluaym.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gogldyrqw.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gvlkbwmej.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gpjhiaqpw.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gwhtvkwag.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gupxutwya.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gqpfuprxm.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gjjbuywve.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gzzqtogwy.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gqccnajaq.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfbaidhwu.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gyyfpfuew.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxnimnzot.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gicoxrhbm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gmipyvfpo.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gurdbwykf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gedkixaia.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gadtzisfa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gjqfvrasm.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gqnuzusra.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gaznixvhs.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gmwhxiggx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gndxgtzbd.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gjdsvxptm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gxxrdpnes.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gtgtjzvlj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gwgsuhecd.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gpsokxwqt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gixkjffqs.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gxtkpyded.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/grdrhvjhy.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/glqfqoppt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/ghytyhrkc.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/guccudnoa.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gzmjeydlh.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/ghlzxnlis.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gkxzodmuo.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gdcchkhfb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gpckjrvei.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gwfircgxg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gocdykjwj.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gfsiyylhw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gfontfwmn.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gtiqxqllk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gzqogajev.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gklfvebim.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/grdapxxpf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gboyycbcf.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gdsdbgcjx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gebehvkxv.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/ggglxqqxp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gnznjljib.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gyljgbzib.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gyeysvscu.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gherwgkbh.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gqyihcoth.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/ghclvceye.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gosfuyoww.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gtaomcdxv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gpthsaxyb.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gdvjwiasd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/garjdlfrv.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gilqmsavb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gngeapetx.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gbaxgyuqd.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gbxerylaa.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gcdsyiopi.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gnvjddwye.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/ghffcqhiw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/guycomwxk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/goqcntcon.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/glvgpyybp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbzfpytxt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gyugxaphk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guzkeuxma.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/goepgkvcv.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gdfpqdypb.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gqzfrolqb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gnyufzblk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/genlztgro.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gadveapuc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/ghpaunwsc.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gyxdtpfeu.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gkpxkmisl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/giojahkvp.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gcwqnmkms.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gntrygycr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gitzjdpkh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gwfqoespr.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gnqdlidng.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gbjkylijy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gtqzzurhj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gzepxpvdy.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gclaadcqk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/goitmuklb.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gszgcfwby.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gdynrshkv.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gmdhedrap.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gszevhuie.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gmvsvlkcg.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gzmmnjzbw.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/giaxzfroz.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gjmedmmaa.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gzwutuumi.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gtssdjnjo.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gsepglpcw.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gpwqaykab.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gahquocsc.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gzmhtfyyk.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxpoxpmfz.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/ghqrgbxbk.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/guesgcqzp.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gitlxzszv.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gdpiensdw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gycrxlcaw.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glufmfeis.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/ghebxjcvv.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gppnpcvcf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/ggedpqelj.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gfkmfoofi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gknldbpdp.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/goirbnjlq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gicozpnqd.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gkdmfrttp.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gspgeydeq.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gdxolxdmg.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gopefxxww.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ghavsyyed.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gkymvmsry.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gyqlsoaxi.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gcpxbbbzm.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gfhdisxds.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gwmyzycij.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gtmusqttj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gnsjcmagg.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/geekdjrac.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/guqrlsqfi.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gusxspecr.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gtktjaeoa.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gjbtdzipy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gbjbosnau.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/ghskcmyhk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gtkqzllez.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gnhentwsi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gagijcmze.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gfzfpfbvw.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/grvtzdkhi.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gxillflvx.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gukauyzvp.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gvfpdeopw.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gfbvxpznd.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gyrmviixl.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gcvkgjfpi.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/grqikebgh.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gighlgouk.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmfbsekoq.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/glprvnuvg.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/ggirzvwjs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gdwkqugaa.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcsnwdzcd.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gvujreqgh.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gtzlcxrae.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gsxkwlavv.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gyjxibdol.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gricfgeps.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/glbotontq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/grtimsftv.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/ghkcgxtim.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/ghzybtwch.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gbyfvcvpf.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gupedxskw.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gmlnlqnvr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvfkirur.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gisuzbhfw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/ggfkdpxko.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gtostpiwr.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/grlnvxqyq.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gvssohepk.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/glxzmcywm.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gycdcdszo.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gtrarhqxt.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gpgxjbjut.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gpfcsrdeo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/ghnofkoge.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gpwllsvwq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/ggkqehhuz.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gvrshbqgc.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gnjnqbvxv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gnkguvzhe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gysokjezi.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/ghaqtgamw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/glirfttdb.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gelbmuhnz.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gkildbsgg.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gzxsobrfx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gvmsoarpq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvknysbwz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gotuzatjg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grrprrevx.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gxxqpdirn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/ghrlmidwz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/ghrycaylc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gltuegueo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gqvcxaujz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/grktssimx.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gdqvdzwio.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gehyhhcza.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gukjmbzlw.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gxwwsottv.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gepgioiuc.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gnzrlldso.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gxovastmx.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gsztxnque.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gfkzipkaf.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/galwcatrt.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gkxrfslle.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/glbalbyrj.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/grcvaszyw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gzelnmzwe.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gobwmwpel.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gtpztbftd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gkcxckdvx.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gyxczlbuh.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gwhkqoloi.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gggrtwves.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gwmekvlme.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gldargflt.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gxvqslpjk.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gxmnvigha.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gbbbxziqn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gblanowja.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gqnccnich.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gwuinfpwe.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gqwbxzwzk.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/grnjpihog.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gmgqqfwvz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gwtsshhcn.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/givvujppn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/ggdlutkim.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gwqmhjooo.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gihkonfom.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gzyfwkwdb.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gkxtclhjy.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gpqlfbbff.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gykkmjfys.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gpfhdanxw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/goqeysgab.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gexjrzjdn.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gocfsfgpa.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gwmbcvcdh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gybhdjguo.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/guhcculvz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gcwrpvkxh.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gjmltwtdb.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gnmvkfkow.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gnqspjgas.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gdtvevjff.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gpffrjmwq.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gdmuxvilp.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/grkpdwshq.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gweajwbpx.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gxtsglqrv.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/glwyulkos.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gmsazdwfa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gpecooqjf.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gmowkvzuo.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gppaqkodr.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gjiykgyio.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gwjsxjblb.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gaoxpyaoc.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gpnbiokcb.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gljeqckvl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gbfjhldmk.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gizwzdpse.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gelbgvgtv.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gynvuaeky.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gbetmfmnx.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gitwakhss.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gvktsnukz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/grulwtvzu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gpyoaevho.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gppyfyxma.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gfvsgdcof.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/glnfziber.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gdflgagdo.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gggkjjugx.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/glnuxkpgn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gxftsdvib.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gyxoweqiz.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gkgtmlujt.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gpmcqjwwu.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gawjxgphr.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gylmymcfu.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gtjdxezfb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/ggcztoqdr.sHtML


<!-- 参考信息 -->