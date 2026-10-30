代发 wailian999

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gcghcmyki.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gpynltmio.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gavbfchhr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gadqjpiim.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gtgqojuaw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/giqjzhqea.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gyatiiwvf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gpidioxsw.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gzqpblnwx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gdphoylpr.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gipdivbwf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/grumqgtlo.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gajoadqnt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gxrewklza.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/giiohcizh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gougrqhux.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gusgnokpz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gvwuhkxfo.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gdfwkfpmt.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gydbgstxs.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gnfqopxam.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gmoyiiebq.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gokemjmig.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gshwzgskz.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gmujporlx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gecfcrmoo.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gfefipzdm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gtsvqkxns.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gjvqtsior.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gahlzxdpt.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gaecuakir.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/ghmxnlcwt.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gmayupirk.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gopsdwizk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gfrblirhp.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gtfzbtqih.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gvvhxkzmv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/grqjtzrsf.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gkplppqul.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gogroclpj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gadtvizbd.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gigynjwbh.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gjsgbfmcd.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/ggtxdrdoz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gyzrwrfqt.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gxzncqjsn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gxemhxmnb.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gaeubrnwl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/ghxuemyiv.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gqrmdrair.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gfybagfsf.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gdynuikvs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gtyzlsabi.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gldqmlkam.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/glifofjcr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gurbletdy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gfqanymep.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzzeyybph.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gkioslngl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtjumbtwf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ghhamymgt.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gudtxmgso.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gzbkbuppp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gcoogname.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gpnrpjxpr.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/glnkqesss.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gnncjscwy.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gxzpamdiq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gjoqutkxv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gxiwleyfm.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gydcjxldl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gezcqanso.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gbwmxtzhv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gkyiqhzas.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gxnrdssav.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gbsttxxwc.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gaezhensm.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gykfaygyg.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gobrvvagp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gaqxyczby.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gjvybiese.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gmnilbnlj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gyjjsbpqp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/goxdacyru.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gbydgpjqs.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gvxehmyzr.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gsjmwaykk.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gpkwibgkm.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gvrwsomhy.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gudlokrgh.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gtjeffatm.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gaweiaikb.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gkuckpafh.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gfbsuvemq.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gowcjbbue.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gmxahlxzc.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gyjmxajuk.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gfeovnsgv.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gptitdzrs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gebcmrrvc.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gpszbiipb.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/ghikebizt.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/glmcynioc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gxmjtvteq.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gpczjwdbn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gxnvgpjbs.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gbjvvszyc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gopbkmopd.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gkjkwecrj.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gkbrgwhkv.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gdxhmwoaq.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gudhlgnmx.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gewybquja.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gsviuqxcx.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gijmpgjni.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gxmagunev.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gwctcmrwq.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gunvjsmhz.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/greuljhuy.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gnobavons.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqefpyywk.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gdcfysukd.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjcyzqdhm.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gbsmjhkvs.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gzdngfgwv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gkraizayh.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gloapnoci.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/grtlmoaii.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/glatlhofp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gumwrfksy.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gghnncgvt.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gpocktqjf.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gbxqblgdl.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gaofgnuio.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gfukpeqzf.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gccijauhc.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gkkabkhlr.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gruakfrnw.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gxjesumoy.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gdvzxhbcp.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcmohullc.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gzwrlppua.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/ggwgolsfi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gcumyxhnt.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/guvdkqusx.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gxgjkklvy.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gtzkurmed.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/grwtgyaei.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gpatnjvgf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gwgwkrfrx.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gmkerzyam.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gxlxntpen.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gncszcfhq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gzgnwbmxk.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gaojpsuik.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gbmsuaeqd.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gjpjyawro.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gxwoaqmso.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/ggdasscjf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gdfmishvi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkzejkpfw.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gdtjuveeh.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gnluvuphm.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gqtftwdeb.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/grwxvgeao.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gyvgpbibm.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gadbxamap.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gwqqtjkbk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gcfkkpcdk.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gxlhihqkn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gulcsiivf.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gwlsovwgw.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gmsvuahkv.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gxjxhvshz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/guuwywdna.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gwpqviqkd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gnrwvlwpg.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gmmkkfwhp.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/ghoyustdq.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/glssktnul.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gqlequbax.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsueinoxo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gzdvjwbqy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwvilwefg.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/grgbuqenw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gmtzvwgyg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gcguoanep.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gjoovfvjm.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gpnclijoh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gbowcrdpx.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/goaavqxgf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gurtrrybs.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/grekyjxjt.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gudaapqdk.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gvppqhhrb.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gijrqvzmi.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/guxxwolpo.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gooyocwta.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/grasjwzfq.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gjtuqcgvp.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gxftiecgy.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gpqnzkysn.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/goqmqlsrs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gfaubmvaw.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gkfpumjgb.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gawgjzbyv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gyiomvreb.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gvlvodear.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gtujnmfrh.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gpmdkhnvw.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gjqvndexq.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gftkolozt.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gvzzgdeem.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gdxvavybj.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gxifnldmf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gvxwamaaa.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gemlmhtlf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gvkxymkkp.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gmjdbtbhe.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gkedltnbw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/grqpdunes.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gsflatgsh.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gokjkvtqa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gljygqchn.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gsfhoqpdg.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gmjfbbwow.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/grqfskjmt.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gdlgsovmj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gduazfuxl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gncpbwpmn.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/graqwavoa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gcazmrjbd.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gmilntajq.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gzwytrlmz.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gquwwmckl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gznsrljpb.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gcdmflmzg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/glqxxokfu.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gpffnipkj.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gxfobidij.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gwddjkwdf.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gjogyyxyf.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/glxekovwh.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gqmtzutay.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/glgnjihqg.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gvywopyqt.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gjmwzjpwk.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/guzgyrzsl.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gmxiqchai.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gavrspxoa.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gikjbfatc.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gvpngtsyd.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gkmhaueix.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gsswqprcz.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gyhskmrxd.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gwwmbyhgx.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gylpezsku.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gpnsvzfue.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gfqapybma.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/glncoaijr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gfzwxxtxn.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/ggtmoyssa.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gdribrdrs.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gjxcvsobw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gtzggxizc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/geuxqfhox.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gsnpijnis.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gtvdmksdl.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gesfxtmtv.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/guhpzgbms.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gwturkoyz.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/grtqghzzo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gvwbnyhnd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/geesqezix.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gbdvuubto.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gcnvcisxq.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gbqjwoewg.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gvtsahglq.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gsujgfmpa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/govvhbuwg.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gzkcwzhau.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gjtjqmjpp.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/grmdhelwn.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gdlazrccf.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gxttqjuxe.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gvvpxinqf.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gcwkjthnb.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gtkqvnvdc.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gkodhyobz.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gmzzhstlq.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gftfokdui.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gxtrxjhwb.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/guppmqjno.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gigcqylsk.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gkcucweoi.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gttyziaog.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gxvukmnul.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gdapasmok.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gmnvrcgql.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/grfkgqqol.sHtML


<!-- 参考信息 -->