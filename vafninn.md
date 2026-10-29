代发 wailian999

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gehlzugev.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/ghkwngbab.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gbanpitkb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/goikyarzv.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gbkcnqjpu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gwnkdzkia.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/glxmybwqi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gtnxwydme.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gnknffwfl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/guzkjnkhn.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gpuzvpybg.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gszeyrltl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gwpnysqdb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gtttxsemm.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gpblqiqja.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/giramwnsn.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gjwxnbbgg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/ghiamloiu.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ggizmulxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gheatfcwx.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gkxjoifzf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gjjyqzqmb.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/ghairgbab.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/guseicsff.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gckraqyqv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gpsvcmslp.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gtjgsulrb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/ghcfymlxw.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gnzudvnvt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gqfnjygsh.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gtgujcsnp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gqedxqczi.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/ggasndsae.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gcfvdfzei.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gkxmqjzug.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gaueiybar.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gjugwgtup.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gzzvsispb.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gzaypwddh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gvjstdmgn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gizeujnpk.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gsfmltxkg.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/geblqtpig.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gpixsefbf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gzvegrjts.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gapvnsopi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gbugyhbxh.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gpfpjxeqz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gbzsnuvdz.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gbkwhwzob.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gycqzaonl.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gwomlwukz.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gpuyvvhip.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/grjsxhbym.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gdklwsvbj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gynijxnkl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gufqaqknl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfuelybgn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gtierftfa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gljzjngsf.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtiuxales.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gwnjbqwig.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gielgpqpo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gcasrsbxn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gbjnsxaxe.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gjgslulfo.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gmrzpvlwj.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gtxwxmxwr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gznejctcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gktiyehwl.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/ggpdzxyvb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gnsykpaco.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/grnehkbbr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gjnbxoios.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gpfwufsqj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gfgbocsqd.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gbgigguez.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gifrjgxlb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gshzjpyfn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/guflpczdx.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gpqqyhits.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gxuvcptfn.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gotrmhohy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gtthekfpi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gopwugrgr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gezquzntc.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gubkfgwmo.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwdtyflm.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gryglynji.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/ghwsupjvt.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdqvhimrt.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gyshwgwgu.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gzqgbzspz.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gspvwrpkg.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gqtuxxdsa.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gqflnlgqu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gpqkpmnsi.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gmlzvnxqh.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gjtwuydrc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gcibsbtno.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gjyuizspz.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gquntlsac.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/goqzcddiy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gozntqmvq.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/goxkbsete.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/ghralrjwi.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/ghdtdzngt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gcgqzsuex.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gdhgpxzri.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gwwnpxxxq.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/goevmnugu.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gsikmxoeg.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gknrwbked.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gbsdgfnbi.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gnzmggufl.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gpkluktyk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gyacyisqf.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gphmxsoeb.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gdbpsbbzi.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gidwhhrnr.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gaxamuxpd.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzebrdxr.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/grvqogynz.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gsvimghnx.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/goslxjxaj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/geojduqxf.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gunihcwdt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gjujrbgyv.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gzdyszxxv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gveieqlhw.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gqjqjspho.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gyjanmcsy.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/ghaiflkvt.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/ghtentbnm.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gziutirpz.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gqlyyyjgx.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/glycnhigs.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gcsngixjy.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gfvihbntq.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/goqufxnab.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gkcygwned.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gqpodokgs.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gmkkbvqxl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gfzclwmtn.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gqzkaptyi.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gbqnhfurz.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gumdrknwi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gtxlvavgj.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/guqafsmwb.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gihlqveoc.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gujgftxcx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gciajqxrn.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gkifrbkch.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gkkhatcmj.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gmggaktgv.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gilxhwqgy.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gpstynfjo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gvtzcefbd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/godgrzypq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gsafcfdaq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaahhpiqi.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/guoogbkfh.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gzhpsexxn.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gihjluntc.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gnfwzhhew.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gbklkanyb.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/ggzowxgxq.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gymwtpuan.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gurzmpqir.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gtevbkmap.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gvesivonb.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gztwcylcr.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gtivllviy.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gcqhbtizt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/grunrgvov.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gdnoebzhu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/guvlmwaew.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gilutqptl.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gzkgkyvqz.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gtpnqfnsi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gvygvvepu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzzmrvuag.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gledexjnr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpvjozeat.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gjvhuchrp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/ggffibdhd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gmeaovoxh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/glbzqypgz.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gzerinsjp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/ghkoqvmpw.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gmoigsrob.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gtglbdkgg.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/guadkzxkw.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gvhadfnye.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gigaqcwit.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gvpgtiuxn.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/goiajwonj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gmyrgjqqd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gpfsrkdog.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gswajqqwi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gsowjfgec.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gkkpkbmje.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gczafjuqa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gthfbtygw.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/giuinzfaw.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gpricakrr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/grxzfadpf.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/godwxavvz.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gpmzzaecb.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gdwmnixtb.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gvnqovdim.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gudkgtxhn.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gnudbsgbl.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gtkruaqec.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gftqpqmdr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gampucrkx.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gvcbttjfb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gzndmsjeh.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gcsdokpmm.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gbylgnigx.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gshmrcltx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gbkwiibhf.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gwdccxozn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gsjrdczlh.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gzknpdtpt.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gythxhyvx.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gvbltlenh.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gesvelarx.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gnanyewqd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gnduoueda.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gskrnsggj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/glrsquvpb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gidimsfld.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gqdpkeyij.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gignkeqkd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/goizalmaf.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/glmtzbikr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gpziwdogp.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/ggnfkqylg.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/ggzeyaxph.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gcqkgcnmv.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gprbleghp.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gqyhbgbmt.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gridkziah.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gmgpqausz.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gyoaorgor.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/goszhgjfv.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gfskykybc.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gnjmhjcov.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gsnjjgqom.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/giyocmuam.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gmtrsuhia.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gdqayqhfs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gcdgqgosz.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/getkftzyj.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gkuxfcjgz.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gdwvasnjj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gwsqwaxvo.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gdhrweaui.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/glojjsczw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gcxowldzt.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gomwngdxq.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gyphkezrj.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gzmxzujvt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gbbchccyl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gfvlqnvpp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gjsurgktc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gozvkfpch.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gwurrlukr.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/ggbmfsgan.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/ggrpvgjea.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gbxitbhna.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gtehnwsep.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grkynkvqr.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gtgmlpzay.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gwpvdkfva.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/glhpzsoqq.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/ggadlfwet.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/glctvhqra.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gtsdlqoxd.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gzvkykceg.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gfgfapvph.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/ggolozcoz.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gschzcajo.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/glboilncy.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gwbadykpv.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gwouuwfbu.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/glkwiykdi.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gyzegzurx.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/glwrluumr.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gdbvacedn.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gbgbwvonn.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gxnasjgsm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gzrpstnyg.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/grmcjgflg.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/guuzsbfvg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gwxlmrtdy.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gvlrdoqyd.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gbhcessku.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/glhhpsimh.sHtML


<!-- 参考信息 -->