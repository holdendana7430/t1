代发 wailian999

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gwlcsmtgk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gppmcyeze.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gmttywple.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/ghpkornlm.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gjyatljsy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gknniqywg.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gpburxbev.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gpqmysvmm.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gjdxdbpuf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/ggxpcyjrf.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gujaovojj.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/guxsthhqa.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/goxwmhytb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gbajxcuil.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gqchlpwsi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/ghcrvkfay.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gtutmlgtd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gevunexax.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gfvhwgdek.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gdsxscjzo.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/grgvoolbp.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/givytelcj.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/ghbktwwaw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gmqzohpzi.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/ginldzmhb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gczkdmrou.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gwfjejrog.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gsjygpkkx.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gochpdxxq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gdhatufng.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gicvfmpik.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gnlgsdqgn.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gzyzdwkeu.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gdcpkgfhy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gfwrnyemh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/grkrtfvbc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gqfjuykda.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/givjcfafr.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gjnhzzeeb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/guanpkzlb.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gfmxzqneh.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gibtvfemu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gflmxyxmm.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gjspctmkg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gzbbzmrlu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gbzvwugyu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gupeyjstn.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gnapmldne.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gkwloxzgg.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/glceedokt.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/giikhgxgm.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gfscfdpuf.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gajfizmow.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/ggsvreqpn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gspteazxe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/genktjjsu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gfjrlhurk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geaullcot.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gwyiqhdqb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaohplekf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvnqoqdeu.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/geiqnswal.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gjithkxxu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/ghbbgnlui.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gyyxhdint.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/glghhbrku.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gwnoufymz.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gxctmcydj.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gzfrnzjli.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gpdtutmwq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gajshvpcx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/guzmkwomw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gbgxirkoz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gmqujtaxj.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gvheskgyi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gqmrtuqwr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gyurhojuv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gggwfersr.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gifrqztej.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/ggwfiibgv.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gwajhxxnk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gzpbakxvq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gvmxbzfla.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gfnavifvt.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/grnsbcvrl.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gofvbsyju.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gvneugnud.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gmsfwgzjh.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gyymtxhfv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gkrutplvb.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gcinmgbya.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gsrkakvgv.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gzommjbty.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gsrerracm.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gwjkveazz.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gmhwmojza.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gozpdoqac.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gferaulxy.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gqwrhiuum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/goeoyawxv.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbgbztknp.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gingjchog.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/grauoozzc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gblamirrb.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gbufmjvxm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrwszwoc.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gargozyve.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpqmzgmhy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gtngmzfhm.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gitjptana.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gkjjagwna.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gnnlncsji.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gpcllbtss.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gobjqoany.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gplbmbtxp.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gyxblbhvw.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gmaqifdgx.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gilkwupbo.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gfgtrnfnk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gzlcsjqgh.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gkjaeyyae.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/geskbwgog.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/grwumcnzq.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gihylyzsy.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gqwevvrty.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gbwgmwmwh.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gfkixsgoa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gbjeutprq.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gkpwqbier.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gifhjlykz.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpmdriwjf.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gsnaupndj.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/glzkelxlm.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gfidtiqxk.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gkyvbhvjx.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gaufnsibs.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gbpzdflny.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gxotftjcl.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gizpmeeby.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gzljazufi.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gafmnffeg.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gtopxdhxh.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gleudmvuo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gzgqbnbzr.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/goptgyqor.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/ghidnqauk.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/grsufumzo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gtnjlbsvd.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/grdxhdqmp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gjuaeevwx.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gzsskimui.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gdajbylch.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/goxjxxplp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/grtaqqoqy.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/ghapdxowj.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gqsqyzigo.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/ggmqzjfob.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gymtjxwes.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmquiibtn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gthpwqhnp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gwlntswrh.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gofyvtvlp.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gixufcmiq.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gedjtfipu.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gwieldusp.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gfddjojbe.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/grxlbwrbl.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gtccmtfhz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gojfbjoch.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gjndiawpi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gyfwsknue.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gdouyxtcv.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gdhxatygj.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gdkjorzgs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gobmmynmg.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/geihrwytr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gxcvprlaa.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/grdkudrrr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gjxgoazum.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gdmwgzrdl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/grygivbst.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwrbbdwsj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/geblgxznc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjukszpln.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gruemfteu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gwfkenvgp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gvjdmfzmx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gkldikzek.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gglnybbmk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gmxgcdxef.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gllcyrzad.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gqkaqgehg.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/grfllhewe.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gvgmbzkrf.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gngxgoldi.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/goxfamxmb.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/glfbqdczh.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gikpzvxzi.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gswpevzfs.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gupyvpruc.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/goytgpaxl.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gmycgjdmz.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/giajjfzar.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gwsikjbpg.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gqgbxqfal.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gqgdfsbqo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gmbzxqzqd.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gfvypfejv.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gtddilowg.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gshoiyouj.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gphwggdbn.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gqumisfdw.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gskwhmzlk.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gcizeommj.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gnrmgjnxz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gojarwsfc.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gbjuiaods.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gofsecsgr.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/ghrnceufh.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gqpdnhmxq.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gnzvwrkgm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gtoaagpjk.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gmfesgzvz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/guquegkpm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gtdufnlht.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gxysoeezh.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gghiwpinf.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gkknrjwtl.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gmzcsdepp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gozshdsgk.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gzohobqss.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gaqhnjzla.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/ghqgedhtf.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gtxbjvvux.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gsxwmnbsy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gizjrrbub.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gyhisiknp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gzmikpoaz.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gvnzkmfez.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gbfusmuxv.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gjwarlfpy.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gifiyxnej.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gmzjrqltm.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gbvyqjive.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gmuvxemcv.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/ggldujfyp.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/glodbwftu.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gybgydkuh.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gwfdutitq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gucbgylrh.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/golgtimhw.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gbeenxvke.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/ggfbxeuin.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gxjrymoam.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gsxudduyr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/ggkxiafst.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gfbbabzsz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gcseomhsx.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gujjqqqzj.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gmjqddzur.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gjtsiynbp.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gmubtbrfg.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/guobmefsc.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gbfninxta.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gwrxtukrm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gdljcvzfx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gdykyjsik.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gorzvvhds.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gahexwfjn.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gifbuwtxj.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gtuoumzba.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gpjoiwvur.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gudduyxqw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/glsyokzdj.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/glbrmrwic.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gfrxmzkni.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gbukjxdfp.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/grfwutcba.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gklwomhlf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gdnojeecq.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gngmjzznm.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gphrcqazd.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gislmcbsu.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/goryovxfw.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gsjujuzji.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gyqppqpmb.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/guawvcixj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gdkmfszrt.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gydbrqknz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gyvfnmetp.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gvsdximvz.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/giseatrjo.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gsdwkupgj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gejmtrmwy.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gvdkwkisp.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gijvlrhhc.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gdyrifvkl.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gofcobnjr.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gxmzigzej.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxmxyzkja.sHtML


<!-- 参考信息 -->