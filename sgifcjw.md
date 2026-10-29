代发 wailian999

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gqmggqjpo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gcflkmwqj.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gfmyoqpyw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gojytotno.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gwqvlsjvw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gjeejmbrf.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gudibanhb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gugiemdam.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gtpamfrra.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gxmutuqsv.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gpnewimbc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gnorzydaf.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gbzyqkfil.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/guprfeljz.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/glgdzlklc.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gidtnsflj.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gxkuloptc.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gxpautcpw.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gtromnldu.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gnwoxrhep.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/ghlryzvgi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gmaogefeq.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gqvfhymie.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gykpupphl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gcaiiayxv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gcrqcsoyb.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gnldxvqpc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gmsaexwqc.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/ginrggpwj.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gajookbua.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gmubgyjak.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/ggxbmwrsk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gzcvtapdf.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/giosbluob.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/ghvgxkrgp.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gdvhncpxt.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gocshlsuo.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gvbkmlewd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/guruwsldf.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/guxbysdtc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gaoyujefq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gxhaxnmql.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gfxivuglx.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/ggbvtqskb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gmkpsacyj.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/ggrmjsypr.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gblfxkqly.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gbimiuseo.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gmmmlpcef.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gglhhlfbl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/ghierlkko.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gqtqdllfa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/ggmruyyvn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnsrwhzdw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gkqneubkv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsavfcbol.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxynwgnhr.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gffogpdqh.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/ggilhheti.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gqdkbiwvv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gyjrgzovo.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/ggsovqrhh.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/ggnqkinnk.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gzgfebfkh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gmygdwpsm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/glnayqoyj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gdjvswkus.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/glbwrqdjt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gwgrlghfe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gorcprmbw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/ggnrqhezd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/goldqfplq.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gkgrqihov.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/ggkuuqcrk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gwnqrzkbj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/geewmlzjz.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gvpqjylwf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gkimksxpy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gtahapttq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gmhmwfojb.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gvzxtievm.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gfeivahlx.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/giumvvwuj.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gdfmdikkj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gianbsbso.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gvrgcxfxk.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gsyhljeiq.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/grurnpeqc.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/ggmkqfxqg.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gtpwerzwm.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gbjtkagom.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/ghvkgfzkm.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gcjigkuom.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gvxcelbnq.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/guzctgnpy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gpgefcfuc.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/ggcehwtpv.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/ggtibhaat.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gcgzcicxo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gtibdqnkd.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gtbbbaufg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gitigmjnt.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gcxknbcoz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gfgwqbxnz.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gtrnmmidg.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/ggibpdfbo.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gvtunabke.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gbqxznotp.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/geqdgjzxm.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gsvmanbts.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gfkjwzops.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gmyfzhols.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gcaonahve.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gimrxkbqc.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gryeoytvp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gmscidxww.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gsyommbux.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gqubqcwkr.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/grnggkvcp.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/ggqmwqpep.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gavusnclj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gxktjgeso.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gcnagmujb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gvpwlnkfo.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gavrhdwat.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gfzxnjynf.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gmwwulbwn.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gyjvenrgz.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gfhsbyrpa.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gukbwzdae.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gvsmmfsbt.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gcwycydjq.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gynvlqhlv.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gvacrayqz.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gepwcotxp.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gfmzrdxlj.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/ggzkpnwjj.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gqqxwrtpi.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/govcmnljs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gemcboavz.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ggurpdciv.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gmfurrmtr.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gjxdueflr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/ghpqgamiw.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/giahjvpuz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/glsduwjwj.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gqweigpsw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gcxenprbg.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gvhqaviee.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gyjdcrojq.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/glqvlpyvb.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gtglxjacm.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gwzqmrxst.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gduhutizl.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gqgyzduwa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gspvgpffm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gfkvtiknq.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwodylkgx.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gzuoumrdw.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gsiyputmh.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gapnxisir.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gqkavdaea.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gbjuxapxc.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gygiczkph.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gpaqazbqt.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gleetjjkz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gyadigkex.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gvwprmtwn.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gvmzshpdy.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gstjhmtbi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gvapjusur.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gohrgmhfy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gouzxqwgt.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gsgknazmz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/grkjsgrin.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/geyzixzwm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gkefjewwd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpetlxyvu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyygdppdm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggbrwcbhm.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gxexylqym.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gthxdovvl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gbtsdixrz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gokiijdmt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gwnjemwok.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gfmkgldpi.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gvnhpfnis.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gztlvvydi.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/goeyyebzl.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gakzhfocc.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/getgeabsq.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gqopmqzum.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gywnzogya.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gvyfryzln.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gletmynox.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gcqosvauk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gopgurrwr.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gduvboarw.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gcnpiiyrj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gcbpacssk.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gxtgbprga.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gdrykexzs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gbboeseoc.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gluvgbedk.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gordbqgjj.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/glxmduyzr.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gafmatsmf.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzluzsfh.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gayfqgdsz.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gohfykbur.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gxajswoef.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/grpozpiwy.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gqyrowcld.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/ghoewmvvg.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gopkdkwub.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/genpixvmt.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gpmgvvmhk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gbqaxbsmy.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gmmsyqzts.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/ghruarxpb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gdtezlxyi.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/ghrnmiyli.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gfdlvwgug.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gxudzxvqo.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gxuqovybu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gwsmdhjpk.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gvtfgtoyb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gdlzmqnfi.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gmxrggenl.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gmrxqgfvu.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gdvmfjqbn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gfoocowvv.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/ggjxqdxju.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gyrreuowk.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gbhvuacgv.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/glddqjrao.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gexmiqtfe.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gpgfxquky.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gsbezudhj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gdatvwlbh.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gccykvznj.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/govrwjeuf.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gurcjxghj.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gdgvthiyx.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/giygzduhj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gkhbjrpbr.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gcooqbsmr.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gnqtpfcoc.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/greoesulg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gtoaahwea.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gmnjkbmea.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gycehmykp.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/goobenjzl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gajsttysv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gjkhlrysk.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gvsxoifas.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gkvbynbuk.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gevyjyoic.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/giqyucrnq.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnpeeleg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/glifmcykr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gmmvlotrg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gposhjazz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gfwxiywfc.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gtnritttu.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gibixbmvn.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gufoeujiw.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gutsbpnsf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gcrgogwcc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gwmeapuyx.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gzvjtbpks.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gavgyfuup.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gcznxlkib.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gnkdhsmdx.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gnfzrauga.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwbbaqmxn.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/guybxdkar.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gzduvdzfg.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gsoiomqap.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gzrvlntht.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/ghxpeljfl.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gnhnglnti.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gjvnqycgz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gqoqhucqg.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gasndjshl.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/glnltbfwb.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/glylsgfgt.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gmxwxukom.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gxmaecbbk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gyomhjqia.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gvxxnmcws.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gijvogywm.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/grpebbvzl.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/guowbdbub.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gofjssvxz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/ggbkirmgd.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gmohveqfq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gjevahxbq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gibjhdste.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gaohahjwc.sHtML


<!-- 参考信息 -->