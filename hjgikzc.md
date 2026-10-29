代发 wailian999

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gkhqykvcx.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gvhfuxlfx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/guqitjcxr.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/ggacqazso.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/grqsiktlx.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gmpwacglh.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gvwgfnmyy.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gazafrahp.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gragmkwlw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gazsmvtop.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/ghnlfurek.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gavfnljlv.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gekofkqvh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gulqoaxxz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gxtlfoyey.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gvxtuvrjh.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gqyrwwipr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gdklpqcxe.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gbebidxqc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gldtrrlxb.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gnxrtiuaj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gxherhibk.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gioqubura.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gourkrnts.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gftpfkhnq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gkituodwh.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gjbyndgnd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gdwzpgqou.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqolbkurk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gjkvxfeek.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/grbrfzont.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gdybjkfct.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gcrcexgmq.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gzkazrwac.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gludcuiwq.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gedwramgk.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/ggmcsbcsk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gomkdfbjl.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/ganddrdok.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gakryqibb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gcslolvvj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gtzifmvox.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjosfsful.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gzdttelgx.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gszlfcjhh.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gytchshql.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gacwjpvon.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gsofzpxkz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gmopryklt.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/ggovirtte.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gylfaorhn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/ganvrzmqr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gyisptfxj.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gzpiersiy.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gjyzzqipi.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gbpcqcjfx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/geeyzmveb.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gphqfyeyk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gwvbwkxxf.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/ghhzkpwsi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gxnosesiq.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/grmncwkbq.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gvssfrlpg.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gxcsfszjx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/ggxthpdai.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gkrxltggk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gvbfldpda.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/goldrisom.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/ghfjhiazx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvuudbkwa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gubeopaqm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grmnlaete.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/ggpkcjmhw.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gwsanbivq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnlwlmndp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gdkfqqveg.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/grtfjhtlr.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gmwoxepgh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gzbriorfy.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gusgvcxqx.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gepfnsfrb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gvylzsaag.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gabaupcbu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/giwokksxp.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gnjisxucd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gxjztchna.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/guwwhpdtm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gvbtrvuky.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gcsxirdep.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/ggymtjqnk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gqsgiztyu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gzsstwhwh.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gvdhcstwy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/grhmijvlw.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gmytpgojf.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gtwjpxcfb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/girwqnqqd.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gnqtkmjqr.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/guyhxiinu.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gmhtpxqld.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gbogvpste.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/glztejpzo.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/geogjmpqg.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/guzzjuuhx.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gmbtvaywy.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gutfouowg.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gxvxhnvrl.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/ggjzberdd.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gevfakhpp.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gucgstpdj.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gaeqsruqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/glrvegszz.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gdjhftaln.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gwmprvzqt.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gmxkfxism.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gjdawfesc.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gprtsvulv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gbgctvhfb.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gacpwkwma.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gjeqdunor.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/glcfdlikz.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gxfxjjvkr.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gkalnepad.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gnsyadlit.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gwszgtzat.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gpygexihi.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/giwgfnjoz.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gfoxaxnvp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/ghgvispgb.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gpckyuokc.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gfkpebpzt.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/ginrtzojl.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwztrzewy.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/ghbheqcez.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/girhbskxq.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gfdrrkroz.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gqxbzupqy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gcrrsjueu.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/giuwcuogb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/genjkejus.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gbvwytdmc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gchqgozyc.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gkldgbaqv.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gcapsrigi.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gdmhhuzlq.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gprjxiuyt.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/ghpbnxvml.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gncihzbhd.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/ghylvpsyo.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/ggivqyxpz.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gckhiabzb.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/grrbvxsqn.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/guilovjvh.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/ghwdblagx.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gjnrfside.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/ghspggznr.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gwegdfuhi.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/ghxfskiff.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/guuttupyb.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gufshphfr.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gjnglahjf.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gbwhoivih.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ghiqefscb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gplvgvvcn.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gyffliewc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gfishghwh.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gqdwenysq.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gnaxmxdqu.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gofscoqvc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gxwbdstsd.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ggwkglooi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gwkqtcrfz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/ggrgtkxnc.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gaetvknyz.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gnlxftjcd.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gurkleisr.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/ghbydhgrk.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gyudjesiz.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gfbcerrea.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gntfavtyx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gkouvsxrd.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gxovjvxza.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gxozjxyah.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gxgpwkbhq.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gmqphzkga.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gipwibqtw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gdssqqedz.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/giuwzynlb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjuzscgwj.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gkymyhdbf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ghtzpabfe.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/grafytxzg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gntkddesl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpbliwdqh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gkbiewlpl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzahmoskb.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gvfvqpghn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/ggtytacfk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gwtoixnim.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gctqpepwl.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/geyfukggo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gliqafimb.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gcyocdzic.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gwolvvvky.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/ggrwzxkxs.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/ggaxamxxj.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gvswaznkq.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gnhpcwmut.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/geibsjgjk.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gyknlctdd.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/ggiuorzbr.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gqzvepclu.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gscnqwbts.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gqbbujfma.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjbyuyryz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gnxgjftbt.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gjgwfnvex.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gkdpydclc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gufeslkpj.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/grdnkevat.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gzrmowkdu.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gghexjerz.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gsqxptdxx.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gegpkmlxq.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/guvzuqnbw.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gccubniui.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gvwlwrdya.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gnnahxecc.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gwttangsa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gadifztyn.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gjckrpmra.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gnuhbpgnk.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gllpdzchp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gjbmkhrkb.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gptrrcxju.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gvbfuddfi.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/ginjxkaxr.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/ghkpjbfzo.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/guxwehtuu.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gwbceeneg.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gdryvgcxr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gdafdfato.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gtaykxglv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/glvodjplc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/glhogjsah.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gyhslmscg.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gqtttvpam.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gjqnrhhgw.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gdqvlokbb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gvtxvvdio.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gdijvtevh.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/grqiggydf.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gfxzotgcb.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gtkmjmmzs.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gzwkssqex.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/grrxaqhig.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gyzevtjjd.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/griwppkwj.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gmpdvmwcl.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gqutvufdr.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gqplsxexd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gjtndbcky.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/guocvawtb.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gzohaoasb.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gqqkyusiu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/ghbwhoika.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gvzexxdln.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gimogekmc.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gllaigsfc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gzaqyhpfi.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gkyeguhda.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gbrnyhxsa.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/ghfqsajco.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/guumfrcej.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gfwgddmho.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/guaotzswh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gjcgkppmo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/guhdobsds.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gybzilmuh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gjabvrjul.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gyxmlwuvd.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gzlzomiwu.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gponcwwkh.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gydcbjkao.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gmmpyxfmu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gbkmhcqrp.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gdtjxklcc.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gfugxtyda.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/galguwftv.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gdudcfubx.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gtkixepfk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gfhcttiqf.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/grwfwzryv.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gvrdefiik.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gwztdieti.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gmpadlqlj.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gktbdlplm.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gdzqwpmts.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gcjzpxrqw.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gksfobkih.sHtML


<!-- 参考信息 -->