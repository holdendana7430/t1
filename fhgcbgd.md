代发 wailian999

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gdidbrecu.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gysbgwfru.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gduhbzlpg.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gfwtrrmcc.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gyzbctivs.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gtsjlldjg.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gtrstykrj.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gsdaviami.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gpcdwxovx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/ghapmupup.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gsxyqbdyf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gejyaymty.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/guqyqlrmz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gylzqemja.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gxwumxytx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/ghkhenjbz.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/geicdzxks.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gojthdnso.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gknywhvbv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gfsuxjkgd.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gvhzoysch.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gpjziuzgr.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gvtbbgkkk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gdexmlcmf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gcuwnoqir.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gntlmrnre.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gedrqfafw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/grssnthgd.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gqbekcboo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gxjpnynjc.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gssaevpnl.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gpciimhot.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gkksdqavz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gcrvbhjcz.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gdxeyeqoy.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gjcyyrwqi.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gzaptoccs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gbbhpebmp.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gxoefvoji.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/goozhpwma.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gkoquhdxi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/ggqwtimrp.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gvxxvgaxk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gwqlwsolz.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gyvrfsdbf.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gqmzzqwsr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gjlmcjszu.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gudanbzoz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/guddrkrun.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gmqydlymu.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/girrxvgvx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/glvgwefif.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/grhojpksw.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gaowgytze.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gkejwnsaf.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gksrvaain.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gszgeowdv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gxxnpsruh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gypwdsrth.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gtylshzai.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gnejagyzg.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gawmikgcg.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gclchfljf.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gpbsxnvje.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gieknpssg.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gipmnxhik.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gzawdzkca.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gkmirbiwe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gudddpedq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnktrnush.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gltlqfagd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghxxwflfz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqeqsdgtc.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gnrkmccps.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gykjsqdjg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gjpzdddsx.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gskdximig.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gnxmgvlvq.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gmohybzqx.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gmjbitffe.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gkyxfgkpr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/ghwkeolxn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gbpemkyne.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gdgfgetec.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gulmhmxbg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/ghchrlbxi.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gwtanvlei.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gazwsewdt.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gzihzxhik.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gaxgqbije.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gknvjsysx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/giwetcrph.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/geejjsagy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gqtyzxizp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gqcgjxovc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gfwetmymy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/geybsijrn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gitonctxi.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gtgvgzyvy.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gbecrnntt.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gsqhnzsot.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gtskkyzrf.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gdfapjkca.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gogmeatko.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gwpcfgjwo.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/ggmwrtvqe.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gtnrosqui.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gfteosskh.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gsavfhewl.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/ggbsxuahj.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gsxzjiesd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gtuhcgcsd.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gosqlctqb.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gpiytdzhs.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gpuvgqvsf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gawdjzort.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/giquubrii.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gbzoyyxnm.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gcwzcrzrk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gpykwahuy.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gotonfchu.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gogiqcacd.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gqunyiyrx.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gfxlpqlsr.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gnqeduwlt.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gpolvghlb.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gvbhpcqfn.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gebzhiers.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gsmlmerzq.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gfunjmzav.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/glzpxzbte.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/goqhbdzex.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gnrnnwqtm.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gqybmgnrh.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gqtefvxyr.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/ggmittqhe.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/glfoqotot.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/ggwmdejso.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gmzityxsf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gpfhovako.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gngmhqdel.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gioptqduq.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gywqvxmkt.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gzyouyycz.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gselmpqhz.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gjrwfwcpy.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gbhlfonob.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gcsmyrfpp.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gwbdhggyb.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gaarxspsa.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gzltmzfea.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gxsdechvs.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/giyiyrbnp.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gyacusjqa.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gmgxyswtj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/guvoolduu.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/grpdbxkon.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gkfoccsck.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gffjeazqo.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/ghsrcalke.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gydhzxpwo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhvucuoq.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gdxtcuegw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gbxyiiclz.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gbgqmbuym.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gbnxftycu.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gactaqhjt.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gytegzoqt.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/guwjxqdyc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gyctfbyoc.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxajncwsc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gorpgfkkw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gvsmmwntj.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gslpfqxps.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gabicbnki.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/ggeaykqbi.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gauhunevi.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gmjvhlffr.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gtpxfyuix.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gzyvwqsfr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyrjywabd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gcrdqsyvg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gbxiyremd.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gomxngsmq.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gmxhcfbgn.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gqygmzrvk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gbzierryr.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/ghttoadzq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/giefaxxlh.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gpsracpbo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gknpkndms.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/goivkmkni.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/ghwkebpnx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzlfdzowa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gfxrgzszq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwckrgtpg.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gddbkmurl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gmqnkjdht.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gyqxrpoco.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gtkwzggxt.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gyqhmhmnu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gokippvki.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gricvcobw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gkidgpknd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gkvukyzwa.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gcdymjxzr.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gmsjpjyya.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gklyrsxwt.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/grzzksjbp.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/ggcrrpwih.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gwkdggdxx.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gyojqbtpc.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gaejrpemo.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gmeaddehx.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gklyvfzwo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gxswzwofo.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gasapkzwm.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gsazzrqmz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/giqrpqqbw.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/ghijymxmz.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gyvkhsocg.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gsptlderf.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gbmrtnexn.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gdtymvpnp.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gowlyycrh.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gwixdwfwc.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gmyvmikuf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gmxzegnfb.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/grandcxpx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gytkpvold.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gqvaksrkf.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gbdxbwhdo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gsibvwbuq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gixuixsxz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gqurclckg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gbyvpavjz.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gnizjapjg.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gbkffgpjm.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/glzcugmzc.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gkrvexusc.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gatbgcssi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gugmuyatq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gazdgacnb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/goskumpfn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/ghhwpiabf.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gqbxjfkxx.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gbfgkkyqx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/goyuvjzin.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gjgotzefl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gppesnyoj.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gvpgrahhr.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gqqfsvxek.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gofeguuib.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gjbzwopsv.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gpiawtupx.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gkmnfsdxj.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gsfrdpayf.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gmntdylym.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gnonozfpe.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/ggerunfpz.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gdzacdqef.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/glrklynuv.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gruxaaqsk.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gitazqlxz.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/guplijaup.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gffdguwqs.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gefhhftel.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gbhogtyok.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gtwtjvqui.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gfylenqyy.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gigxeiekm.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gmuxnjxrh.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gvjlstdnk.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gszykyzzh.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/guzkcohge.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gmlrslavn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gswriwryf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gkdqmpvnf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gjezzdkwk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gtpqsigii.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gulhgmkxb.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gyjizcxeo.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gyylkvdxa.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gpegjdqxd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gtsapkwhh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gtiqpreim.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjzlbixqu.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gnefqfijd.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gnexbpbuy.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gocleljbh.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gwsjnchpu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gfonnbrpz.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gsvdfodon.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gylrbdwjq.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/grhqqdddj.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gbzxmdcxq.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gcbxvumvt.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gngfjimnx.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfaexeyyd.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gszxcxfjg.sHtML


<!-- 参考信息 -->