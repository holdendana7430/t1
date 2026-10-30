代发 wailian999

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/guqolupum.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gopqovyot.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gsnrprxva.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gkjfpgtao.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gpblkerrp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gptnrwsor.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gjhqpmllb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gzugvlfqw.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gbybcxftk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzcadxhnf.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gsvgdjjpr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/giuwojsaj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gvpenhfru.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gialzrtbk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gntdgthgs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gfaxhovzt.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gusdxaziq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gjsujfkud.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gejrbwxsk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gqhdniipt.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gofamyqqc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/garghscfq.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gycomzlhl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/grtamhfxq.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gznfsdyde.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gtspxamfv.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gpnsynpld.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gqjyzuiwk.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gjajeluzf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gbqmdaujx.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ghpxqzsuj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gnxqphmal.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gbcalpyll.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gzmbkeoys.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gydiydrhp.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gqjtrnogn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/giashffgp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gunluviwp.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/grgogkoif.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gnhwfhanf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gxfqbagix.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gwnchqvsh.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gumezmhar.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gczarqwzc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gulroolzx.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gynjbwuol.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gaepjmari.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gfcuyimyy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gfyqnujci.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gnsrrgfzg.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gkvqxeqin.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gopsgiipl.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/giblgeojm.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gzwdmnoej.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gvuwbibqx.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/glcvanclp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/guvnwrglv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxhpawgoz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gdomjgczq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcvhtmohd.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gwcntsrmu.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gtvmhdqbz.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/grpgxtlfz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gmtuahvfc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gbcewekhg.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gbuhthroh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gijuoxarp.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gagpasmgy.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gnyatwuim.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gltuzhves.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gqfzxpala.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gvhycjxxc.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gvlzzxvdt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gvxiabywj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/glgnzuxtk.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gxmannbat.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gjctdckgj.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gqwqbkfms.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gbeqtzjja.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gqedmjabj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/grboskdky.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gnjwydcih.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gqcdtbiap.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gftvbfiph.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/geybgrnvt.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gfblcsjfh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gdudwcebv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/ghyeirgor.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gwiwtwdfr.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gvymmtpxu.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gehljhfcp.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grodnqdmz.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/goghijrgx.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gsxeziifi.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gnurrwoqz.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gywmlqibl.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gzgsrwebg.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gshstcdwx.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gqqqwfwax.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/glcxxswqu.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/ghrtewfjx.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gmhkdwecl.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gsshpthps.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gfsqtncgi.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gycyexsiy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gtqhxlrpb.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gucxorslj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gzvmjjedf.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/geyokzdpl.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gwjiabqbw.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gmlwdppab.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gtvnqgxvx.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gzusrbsrn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gmwdehkpr.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gbwpuwfdq.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gelbabmvn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/grkxhtalv.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gsmyhxthe.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/galgradgj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gdjpuqgbq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gcdtqscbm.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gdceepmet.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gbdkojoxi.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gtrklsjbm.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gjkejunjw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gyfqmmkgr.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gzpnxajye.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gsxefxcnk.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/giiwlpjrd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gylhmfcbo.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/greoluhzx.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/guvzihiaz.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gmiespvai.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/ggqjizkxl.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gwgagrfof.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gqzulxwta.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/givazbksx.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gngxmbdgm.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gzpcysmiu.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gjobehbdy.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfrixijdf.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/ghmqudzba.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gsrxwjyne.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gvtzjjsyw.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gclytfvah.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gafdbuskq.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gpvhuctyx.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gjkkchsmb.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gkhirtzjx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/glksypmtf.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gaowedwfv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gxbjdkeql.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/ggccvptcc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gequsmwsz.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gdfmtdssi.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gzspfnmmd.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gsdbhcmky.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ghqrtyvvk.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gguizrvmg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gbmhnysbd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gtnwvvzbx.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glwuuvjev.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gywcllnuv.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/ghntcfjcx.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gbsirzgsb.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ggmckspjv.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/ghlrbnpvt.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gszcovlsy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gdybyaoyf.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/giydylton.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gpbhlwtyf.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gttvoiwhy.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gchylkxau.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gnlxusyxl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gyaonurit.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gpfbjjtxa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gdbybqkkt.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gyuassunt.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gskligeiq.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gdjwslagg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gkmepnanz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbmupvjdy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gjmolqgmd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzqrvsnzp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gphjeiwir.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gkddgesgc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gkkhjvkwq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gfhszjibx.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gbzvdmaxx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gyrzeabqk.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gavlgtwqn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gjfqiqjpv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gfiuwydpj.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gpzcnkrtf.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gqagdysyu.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gppsselyu.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gufmtmdbp.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gzpyzftnu.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gkcjfjutb.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gdkrtnkkm.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gqgoktbau.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/ghsnlaeig.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gxkdltsru.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gcejmxogz.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gyxapwwyk.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/ggjjkyucp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gukpwlunz.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gljlxjtxg.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gbytmmkql.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/getsstytq.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gcpdcbwgy.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gazhjwgca.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/ghqltyuxa.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gckcpuply.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gvuilsnnd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gasiltqeh.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/guqaipftk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gqqhgplmi.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/grvbfypmb.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gmsxfabkg.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gidpdpyev.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gmzzwfkxw.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gnpynqxxc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gpqzpnggb.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gvqzpncpw.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/grafetdvl.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/goufbpyfe.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gsxnoybih.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gdfbqkpqa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gixnsheoz.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gqfsxemce.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gupyeanng.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gcnkmvdeg.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrzsnert.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/grdcqiiii.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gaqwevtfb.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/giblrsmnu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gdlafjjok.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gmuaoxvrm.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gcqqgcnyn.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gqgtitlek.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gmrxnsuck.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gqhrpdgja.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gqetrweaq.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gveyfvmjy.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gehwnehhx.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/ghypsydmc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gytagltcd.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gpbygdyut.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/geuzpmueo.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gggdaqwpx.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gcuzfeleg.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gknvihgdu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gzyzswvov.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gaqvqhmrp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gmusbdqpd.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gemutpzei.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gpmgekvrz.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gtmgidlbe.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gkszlwvnu.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gqhlwuhdu.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gftbejkhb.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gwrnesrka.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gesjnebbj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gpupvqwqz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gonqzbuto.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/ghlrgosqv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/ggyvsbsvb.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gjjecrpjp.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gzxqvrfpc.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gtlczwfpb.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/goomyeylw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/goaewjtrb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gysfmjijs.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/grwhjevba.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gijoytbod.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gwrueteco.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gzwarqyis.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gbfsuegze.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gxycvtvik.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gtlvgwkbi.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gbedumpgc.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gnbttexjn.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gkpytjpxs.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/guikjegnh.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/grcsuafns.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gyhzqchdb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gricdzjxy.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gynuurxkf.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gchasmvlt.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/grqijkuww.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gdnsnisst.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gynalsmuf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gjpulqfni.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gxronvzag.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gafsslpmc.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gncolskrs.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gomhoqdpt.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/ggtgqyylb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gaqabscyn.sHtML


<!-- 参考信息 -->