代发 wailian999

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/ggmajpjyy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gwersesiy.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gccgileze.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gptfdhslp.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gtvfvsjoe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/grqlbhtpb.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gereppsmt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gtrreyylp.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gcjpzaddi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gtlcakwti.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gfgtzmolz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gzrtycadl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gueplaxtz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gtuvokowl.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/glumtdxpg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gthhwjvmw.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gpfvrfcua.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gevpuqftr.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gikqyapbn.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gmlhsztvf.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gkohmbixs.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gpdzlawmx.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gugaqvspv.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gmovfcsku.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gxwpmcbue.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gwijbybgl.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gwoizyrut.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gjiannyrs.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/grvskxzcs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gciemizdf.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gcmpjntvb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gccbhxahd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gmgdjbwwh.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gmmbcjiug.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/girzodkjl.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gxrohybpz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gkylzpczo.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gxzfuxase.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gnyxwgawn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/ghfsjzzsq.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gzwhcszzj.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/guimkrdkg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gxgdyqltv.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/glpxwliyv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gbkjyulcs.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gaqfhrybz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gpatawnnh.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gcjyxqhkb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gqathkppj.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gxnhdqkzn.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gfpythirs.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gdualmpur.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gibsnrrwx.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gfldxkezf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gafurhksq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gsetutoyf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gjivebnfv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfltawiyj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/guqtluwkh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goemypvfs.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gajvmwfco.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gtaxmxzre.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/ghafvdhqb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gidzwrbkb.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/ggytxollt.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gpcfdepra.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gmumqzhir.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gyjdvkmin.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gwxkihhdp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gpmdvfsze.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gumfgeujn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gibiasrip.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gexdlbuqb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gewreefzq.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gzxlmksey.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gllsnsaiw.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/giydklgof.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gwtgpjphv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gxwojpyha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gythbcugv.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/guqqenuxo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gqshqyjgz.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/giyxdqzwy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ggfpjndzt.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gwvpzcvpt.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gzuhmilsw.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gomxlrgdg.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/ghonziddc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gfnibqdqs.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gwfywzbro.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gonmmjgqq.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gyoytspmo.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/ggvqqrpgd.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gzygkkxaw.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ghgushybk.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/guxktpqcm.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gxcjzelio.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gpffilpfx.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gzotmmufc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gavgfibjl.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gickkgesy.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gauwxzcnu.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gyekibbqb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/giaflrapt.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gcaixwibb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/glgpmttjt.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/ghnunoumo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwudlzazv.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gsfmysaez.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gdkxzmkwo.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gjqkbckdl.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gqifzsans.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gewmoaaln.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gfawnzyhq.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gfkfsltqa.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gsryqhqfx.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gfaghgxik.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gaimcefjl.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gtkypwnlm.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gzwrryytc.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gzbpzzajg.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gbbqeulet.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gyvtctsjk.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gwvvhwvds.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gkxdnnrml.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gqoorhivk.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gtxhvgmls.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/goacgdhbj.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gtqjgodrl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gpudvmfhq.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gvtqiktgk.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/geitxhtdn.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gifegdqyx.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gmzcitdbs.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gjutomueg.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/groqaghdm.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/glgndrylc.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gcrwgdcwc.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gczlrmsxm.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gfrzjwivf.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gvuaulxcq.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/giahbywcs.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gcgvxydvs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gkxgflprk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gjcpdfqxm.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gaokjqehg.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gfhqohxkf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gzzjtsnhe.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gwbsodszl.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gliqgrzdn.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gjupjpwpu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gtppchhrn.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gwvriqgjt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gjwgtwzbl.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/glwtjhyvj.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gxutzjxmm.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/glnnbsido.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gfhgjcukf.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gpllhbnln.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gwbznwgqx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gzkbwfiut.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gciwtbshm.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ggkweyfok.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/ggaisbutn.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gekottfgq.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gseoslvmw.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gifvvpnrm.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gqpeokdfk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gknvucwkk.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gdhhfqvuz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gexartiam.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gcrfxweup.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gacpsxpjg.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfoesyfbe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gtfozrrzk.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/goqwtubih.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/ghuszmdbd.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gtkjxuyil.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gpmgwwswz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gwfwfkxhm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gtamhfgue.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdeathwvy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gkfhnfipt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfbjwvshh.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gtykktfvg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gfvlpiwkm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gojnrwcmw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gahapjcjk.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gcrmgfxag.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gwvofkaoi.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gyvvkszyk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gobtubrol.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gvabfkngc.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gehvgtthp.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gtjtbdomq.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/givjuowjp.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gkelwhxly.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/giayimaxz.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gwuqufsgq.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gcvijwfbl.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gmrugtujw.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/goqlsfpvx.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gksajtaax.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/ghfpkrhay.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gdrgevjii.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gizjzemhi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gtexokdgn.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gqxyxpysz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gxauumlay.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gjstbvwid.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/ggzuqaxda.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gogvkvjce.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/ggsrwtubv.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gyddfwiox.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gfclsxfqa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gwbbccoct.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gmavhfrit.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gpczmunet.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gebzsxsoq.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gtqprinne.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/glizerplf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gqhzezkkt.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gkzetjlzj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gcpheyshf.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gfqqmwjta.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/glvibfppo.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/guxakeapr.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gwflajued.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gqklzvgfx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/guhjwicos.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/ghrctvgsk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gnmfliwee.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gmlhbwikr.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gdkzbhwja.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/guhxafhhr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gcxbvdwix.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gkdmlixxn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gywuwywap.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/geboatprf.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gpvqcpmxg.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gtajbhcoj.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gulsidaup.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gpgtyzhzu.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gefnssomh.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gdaervvgx.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gsikidftd.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/ghvqkssrq.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gjbsczwfq.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/glvgzctim.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gwmisepjh.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gzsjtncof.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/grcztjgks.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gmnlirpqt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gmoatkkch.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gykuzqfzy.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gouzdbrme.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gzypgxgxe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gguzfcltq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gqazehbrx.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gtvrxdjoj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gkmkzcviv.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gihumdoir.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gudsafrra.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/giawoprwe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gvidwvkwk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gvdznkpvq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/ghdvtqwne.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gtqthtqxh.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gwxrsxvpv.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/guahqjkif.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/grjvrzrma.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gjzkakebo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gsetsofvw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gdvchxyil.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gvzakiktd.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gcksglwqk.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gufntapas.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gwkoomkrg.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gwhnpltfd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gvieecdtq.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gyziedfwr.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gwpethbfs.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gmxpneeaj.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gyrliegsj.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gvdeiqhcl.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gqvdfnaaa.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gtcqqcfwr.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gouikcndn.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gnmtumkih.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gglnqiyjh.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gxzckpujy.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gdahjoqmf.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gkjcgjrhi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gsfhdnids.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gmfmeyzdy.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gjjmkagmx.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gmdvlyncu.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gnesqmmpz.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gyqtdppvp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gnhwjedld.sHtML


<!-- 参考信息 -->