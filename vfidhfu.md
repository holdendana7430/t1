代发 wailian999

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gonyoprdo.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gsyuzveug.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxfzhoga.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gpivdyxht.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/genozgjhy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoyqldnw.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gnkujugyp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxukxxbo.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gdvrmqjdg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gobnnwjcz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypravqvl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcmxfrsdh.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gfrsawxvf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/grvcmlrwu.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gyaccftlw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gszroltfd.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/grifkcmto.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoqzfpkp.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/ggewiqhcd.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdpeovos.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevmfvqtx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcldrkej.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gadyxodhg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/grkdqnntc.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwfqmvtou.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfocpbbfu.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gouzjjybc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwjmzmtt.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gqjjzjtgi.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkelvinw.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gebedbtyc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjbbilwha.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gcmtbjdnn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfionvade.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyugrliy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvttzvsue.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/givfpawiu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzbzueykg.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwqzmmpv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/grksrfujz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjquaamyy.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziprrhzh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/grxzfnbmy.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ggorfcrlz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpkzkejtm.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehfmviul.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabzinweq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytlzwxjt.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsblpzxze.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gcefjdsyw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/grberwzea.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gmkivvdyu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gpdtlfgmx.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsrwjmoz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/grvlhipmr.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtduyrse.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpieiove.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyywxglv.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdqzlekx.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gremrgdzu.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gqqtrxnbb.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/guggrhsfu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxesdjci.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gqniwmmuc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/giwsjdits.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaxajxpf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gbgtrochb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggpzhzgcj.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gczbtphbz.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gbhtsilfd.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyyahfyg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gciswidfw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gcatfkebj.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/ggdvpjuix.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyayhbfa.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaxnrzmb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gutudjvcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gdamleuib.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkfhytmv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfhmyrlf.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gzkcwmexx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsspowyfo.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjpacruo.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gexgckwys.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gakserfyv.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gomypgzvh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gyllxquaw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmavxwwu.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduaokjal.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gzdemfnqh.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gxledzrmx.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzkltsqj.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfbqjaeb.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/guyjpwkks.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gmzmgczmx.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/godatyqvo.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gxzoxarem.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdxvahat.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjwdgddpn.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gteualjym.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqfbiirg.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxmqihfpq.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmodzjvht.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/ghzkknndn.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/grhhacyal.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwbjdlwr.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/geueehhvh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/grmfyxtet.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbboizea.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbhyipwo.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/golbzglpg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gpsauqrot.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyhuwfys.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsrnltuv.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/getudkfft.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikywqfqb.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnixyqam.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxyfgdzu.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcovmxolu.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdnvojlr.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gwxxtzyet.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/glgweebrp.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwpqkyaug.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/grkgkjxad.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzberaaw.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqxellhq.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gwnoudbwz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyedxclfh.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghshbuzfw.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbhrebhbv.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghziyxdzw.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geewqnfnd.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gskeffmep.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gxswirkxg.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gmsstikji.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtsolspz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzdmnldv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbxchhrul.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/glqaogfxu.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/ghhycvrke.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gakbrmjlw.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gpagzhtlw.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glwvafevb.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/grrxylomc.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gfagawbda.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxfmdpor.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gvckxgwsy.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfvidlpg.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfntcxatl.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gvntapydg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfejsozm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibxieyur.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gvpxngdfh.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gycwriejz.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjfkoshnv.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyshvhyr.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/golhbmuqv.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzozyqeed.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/glnsojqre.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gywcaonor.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpslilpk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gurwrgiep.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goubvfteq.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gjpwegoup.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnahbzwhs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvebmyngp.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwidfpaei.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gntdfosgm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gchrdfyns.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gytssswcv.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/grqmkgolu.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzfpvzvp.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gptxjfeoo.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfgduqhz.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzujvdvln.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeoadtps.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzlsccbn.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gaaadgfme.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjstpujy.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gtiybprny.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhgkjilh.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gqccxykqw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/grtgtzizd.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpuagtoe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gbtepnjpq.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gajccbsui.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gvjoophzc.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gqyfkptrb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gtvclgcpu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghmriygaq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guaeemotz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzyobutsh.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/ggkvsufup.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/garwqlnqp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gdvhckiyk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guacsosjo.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfglezpg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gldmsplpf.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gehngkrkw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gchznwykj.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggejmqowh.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqyppfkz.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gfrmcupob.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleyzdxpk.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gctzviels.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfcsmvbk.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgnntlva.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gowodskgn.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gpozcwcnj.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkkojcii.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/grwhipkvt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfccwrpl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpshsmwhw.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfdffmnx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/ghcryymvp.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gazfbdvjh.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gdctpzjvt.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gzpuieijf.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwtavzdo.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gukxrmnzm.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/guicdkpsf.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjepzmzct.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/glnohgppy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/godlnzqzr.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gxstnbaex.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gbpjyylhk.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgvvriud.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gvgjxxhfy.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfuhwium.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbxmwgmi.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkuthvhw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gidgzvdyk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxjbadls.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gamtprmwk.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviwkceda.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwamgkqdq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkqzenoxe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gtpouzkyk.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/ggzlrfkvh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gxuipchlg.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwywbvzh.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdidezby.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gwovkoztf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/glvakmniw.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzfhkket.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/grxghmwwd.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmcgmove.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlpzvaba.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gwkttszyp.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gzsvytypt.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/guryfawwi.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjxfncwm.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gcufpdzdv.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/goowudooc.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmbsboke.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapjkyjnc.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gaqhylvia.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gcoqisevz.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgqyokqh.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzrejbah.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gtowpitzz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstwgesmi.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnvlyyvb.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gvjgzifan.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gemygxvol.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gfocyygku.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/ghznouogt.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzzxuqai.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjdhpqex.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfeyvmlh.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gzprzqess.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghotbbpds.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/guvjwhyzi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/girxiuusa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/grqfxjkgr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/grkqvasbh.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gjogsglzz.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/ghdofhfvv.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/glhxgjgey.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gqismkgkh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlayikpb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqclmxfgz.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzfqyzhm.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gdycymzlc.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gngtkjrfi.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gzivajhrf.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gdrvokquq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gavvfdipv.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gmreigfnr.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/grgqxpihs.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsmpuuxk.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggtcwyhtq.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvibzxggp.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gmoxacmgf.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnensapgl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjazxaexs.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmdnezcc.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhjhkgvj.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhyowwkh.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gczofryvs.sHtML


<!-- 参考信息 -->