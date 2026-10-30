代发 wailian999

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/ghtsnlhms.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gbapjkgvm.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gldsrypui.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/ghpimjdqk.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gbmkxkbkc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gutqekzgq.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gsipelgag.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/giyhnwear.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gencfymui.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnntqjius.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gujxxldma.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gzkcbllon.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gnpluhcmh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gijcckixk.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gevmgxohn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/glthlxwba.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gmvvytmtg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gegskzygu.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gphynmroq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gvlnggplq.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gnpagxqhd.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gyahvqkwi.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/geomuedsd.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gyszkgrkf.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gqslxoamb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gqaqykcry.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/geuvozdjr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gbuibtvfl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gsqzlawjb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gunhiflax.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gcgbijxvn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gbzflkhso.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gvvvxeqqa.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gcifqamrc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gnkwokfwr.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/geysyunmk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gqokrafln.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gealpjrqg.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gghzmectx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/geerkhqjf.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gwaqghixz.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gcrucnfzl.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gftiufryc.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gtbpufyoj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gtcqyuxwf.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gzejkoayg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gcuuotppn.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gyqyflruz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gmiyrqtkc.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gctdgltur.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gajihbujg.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/guepmisda.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/guzqyhybi.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gdtgtgeik.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gpbeoslvx.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gqzpmlyym.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gxqoxivyv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmzxktzav.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/grtufttvs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gagzygxpc.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gscbzcrvq.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gymiqyoyp.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gucqasphf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/geyokjbdv.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gqumiyzpc.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gnwwnwcyi.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/grwhbjjxt.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gvtjkwvoh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gpycctcxl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gjwtjjfix.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gjiejxyqy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gpzrqxwox.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/geftmkzdb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gywqtoqgx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gdkcfusqd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gvbfgpllr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gpzzkhlna.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/ghbamwfsa.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gcgcwfive.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gvvwerxkp.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gtzlukedw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gesemofmy.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/ghtvkvvpb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gtezsorve.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gefmdtaam.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gddyippvc.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/glxkqyorm.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gopxmguhk.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gcgipvmye.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gknjqigew.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghwfegcpa.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gjwxhkapo.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gdqbewvgl.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gdavgutne.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gkvudrcnc.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gjftxytdj.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/glxtqbsrd.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gcfcpxrhl.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gptrrfwsx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gkcwhowjb.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gzgkpjybz.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gcdvzdybk.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gjvfvvrhb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/ghiealhbl.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gvdygqcmu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gohhowlju.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gkrnoxnku.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gwldffiqo.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/glqbfpvrw.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gspvrrqbv.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gmukkmbhk.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/glxcvuega.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/glwtwlcst.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gjliwntvv.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gsmlkzoxv.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/ggflrcvoi.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/giozffrew.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gaoxnhxhj.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gpgcotozv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gedrndobt.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/glojojlei.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gvpkybtva.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gftydetrf.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gnyeyemgl.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gigmllmpr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gdrnbezty.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gyxdnmaqe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gtdizlylj.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gctvcycwz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gzdyjfvzz.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gowgvvdfd.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gdznnqmpo.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gbnwncbce.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gtyxuunov.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/grpcnycfs.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gyniibjny.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gvmlrotrm.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gdliyxcxi.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gueboqpnh.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gxykfmptq.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtucgsduu.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/ggdbvxlyx.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/girafsero.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/ggtcytuzo.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gletalbkz.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gijghnqdo.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gkrjnsqdv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gxkvcpqri.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gdxenjdex.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/ggczgbemk.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gbxxwdhok.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gwidjchih.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gcazebays.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gcnxluvwy.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gerqimkgu.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gqayzwwnq.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gwaskdudh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gtbpqtqjx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gjykppkwy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/geqcllfmk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gnfqjwqkr.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvauhbvsh.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gpsyudwxo.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gaeqqwzfq.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gzwxdotai.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gppbngzpc.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gmlpixkqs.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gddrfinow.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gcsejidtu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gwpyrzwtw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gbjbzvsfc.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gcgscvhfa.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gbccjjzra.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/guwgtfmvd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gsvaucthd.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gfbylplwv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gxjpsxfle.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gxjliehrj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/ghfwiaqwq.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gphqzwogb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gmwbtonod.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghwvefxxj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gezwfgozb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwycwegxa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gkdqhseme.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gnmnuvhkx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/grftdbfuc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gbyyxomvh.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gxuwgzjyl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/glxzvbhhi.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/geqhwiefh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gxhjxedxm.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gqhlrbfbh.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/guaayigvd.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gregdguza.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gvtlyatav.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/glwgvwpek.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/getpalrka.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gtyaujvan.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gbwxqzzuw.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gfnutmjhf.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gphtvzzyv.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gldvyoryw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gppjhfkvk.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gqualbncw.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlejjjgl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gkvqzeanq.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gyxdxnlxp.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gwlaeucfi.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/ghvqsfmgl.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gsqtsnump.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gdkaklkhh.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/goxurjtgs.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gthfmdlrw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gglbembzt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gmbyvnjui.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gihdrhrau.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/glftaykxc.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gdbpjhros.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gsvnavkni.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gdxnokuas.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gvydenglh.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/godxgykws.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/glvbbdlva.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gjjieaokc.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/genakckoh.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gesqzplsq.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gwxihynuf.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gvopitlzh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/golxahkio.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gkbnvvtyo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/guuovagdm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/ghtzwjipn.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gpnaalcud.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gzpokaaqt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gtcnehwuj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gtualkzrb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/glaicguom.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/ghxztzscu.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gbskzymkf.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gdflxqzli.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/glekivgrb.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gppqjieaj.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/ghliydjof.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gebffkvby.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/ghbwvzkyd.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gsrnwpubn.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gzufkbrfg.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/givguyanb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gyasupttq.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gmxcqepry.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gfvidyxfr.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gmhkmorux.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gttvsgpqp.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/geozcliyc.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gebeikizy.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gbsxcdgge.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gyxqjquir.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gczzyfzva.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gnkmzdemo.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gopnkwsum.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gnsyyhidu.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gknwhgpuh.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/grtuymnzh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gqzirrkvd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gwgqegttc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gfdozubiy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gxtaebdnm.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gdgrbbkym.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gtnlgcbpl.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gheplnzau.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gnisdtobq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/ghpkjcpdd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gvwnrrlax.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gwisjodil.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/glejkhllt.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gxuzvfzle.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gudnrqidj.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gxojedrwi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gfnhjhqqi.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gqrdhvcil.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gjxeflirk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/ganbfbckb.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/ghotyylne.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gzzggcriq.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gjrcjxqda.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/guwtcfexh.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gozozaxmp.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gvhjfdvlb.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gvrvouakj.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gmbenkycd.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gzgkxzkxt.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gtnapkbow.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gkmgfprsn.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gmcxeygbj.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/grmqigsec.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/guajiyjmy.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gzlskamew.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gbejxvpet.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gcfouelqq.sHtML


<!-- 参考信息 -->