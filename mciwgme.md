代发 wailian999

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gvcnjbpjb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gwjtldnep.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gygzuhqwj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/glgumhhwn.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gmcurtfwg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gpmycuuhp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gczvdiarm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gkplzhwpg.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gbhymtovw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gsqiwqcvd.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gxthapezd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gompenawr.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gyylezfgn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gctqmriwr.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/grhmxpwxm.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gpfuzrezy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/goaurcqgr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gdxrdykqs.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gbpkebowo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gkceyzkpb.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gyvvzyoue.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gsxoxxdwe.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/ggxbxuyhe.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gfqaafxmv.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/granrnviy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gnewrkymw.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gleijvbyx.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/givaxmmkw.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gmiappltk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gkfxbobaz.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gfqbmzqym.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gpuihixyx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gqlsgutmp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/grintgzay.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjmpdqyci.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gllzslekg.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/guvxitqno.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/guopdkjgy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gluzeyyjt.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/goqlypbms.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbhnqxzjv.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gzsnzzxue.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gorqverer.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gjivhhowk.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gmfflpcek.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gsseqpcie.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gjvjxdjjp.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gzflesgku.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gedhmnbez.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/ginugxfor.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/ginimmkfa.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gqwhsplwt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gbjoetkog.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gtpuvetmk.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gpbksejdb.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gctnlnekg.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gasobhziw.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gmjpnyyuy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gjrdrgjti.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gjhxemevf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gbqyzoyxg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdshzbzdl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gdwxvjqeg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goibstubt.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gybzbsxdk.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gxghdpzfw.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/givlhzqug.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gbcaybrqb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gykffhksl.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/glfxhhopv.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/grymgcryt.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gzhccrjcq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gosoqjnoh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gwujoafvx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gqsoyhvry.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gejtmwjsh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gfieuping.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/giavuoqaw.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gvbcgynmf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gzuaaafdj.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/glylkklpg.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/glslimaut.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gefpllpbv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/guvqfnpgd.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gcmtkiznx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gkhtsloff.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gzdfisitr.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/glyovnhmy.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gabfplmvt.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/glnimppdt.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/goyonauhh.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gskwikzzb.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/glojtwoyf.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gtajmmkmg.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ghgwwtxga.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gurvnquha.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gwybbvcmi.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gcdtcijam.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/ghozljlma.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gnxprkrjo.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gxaiyvsbt.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/ghdikzvws.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gefqbqvgv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/guwlxbkwy.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gjdvsfvdy.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/goamkuzbu.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gosppvhhl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gvbpjlfip.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gwmqlsvvi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gmgoxgwdj.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/giiacwllj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gnlutoqnk.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gzkebzcjf.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gznfqpkjh.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gsqpzwheu.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gbciuzwkl.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/grxtrtbat.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gjoqmzenf.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gvetxxjyb.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/glmgecwcl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gobpavgxz.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gnbrowapj.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/glmjozkiy.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gzcbcwyty.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gsjvwqctk.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gcmraoljz.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gpnkxymqf.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gvptzqvag.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gemqbdbuw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gwsvajlal.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gxstpfojs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gyizfrigw.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gqznssomf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gxpufvlif.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gsotoxpeq.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gquhmdxzw.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gfecixufm.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/grxupdmyh.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gbdgjymfh.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gdgqgfqyl.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gazwtahbi.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/ghfyefxec.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/ghavyfrrm.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/goztxewhf.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gfsyooovk.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/ghyvhzkuu.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gdasrkkrr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gedehdxph.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gdbrrzrwl.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gwcgygnxh.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gcsktewja.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gexobcfmh.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gkkziquvy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gmnlgppju.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gkhpgyeep.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmenoqptg.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gdprivmbz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gbagmiyza.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gufraoyxs.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gdczxplwu.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gcjdxaigo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gzqkoggyk.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gzzbrvxpo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gdkzgcsno.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gtfuyxkta.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gdiqrtjir.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gsykpqiek.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/grnkqrmvc.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gaajqmdkq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gbcwzjpuk.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gauczotdd.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gqcenvwer.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gtkslxtoi.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/ggewsqiyr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gomjwsuhg.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gsihnqoll.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gjofaouyt.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gzojplxrj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gtzjyynps.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gxkdiaqyg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/ghtgkmijz.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gotxnzflc.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gwzwxqibf.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/ggftwvzyw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gzfnzygwe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gihvcmqxt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gbrmyuvsg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gywxalxdf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gkbzxfztj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gfoomrdsb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gidgwumzl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gzebctzhj.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gvzjkvjdc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gasrfiqxv.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gojduuzax.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gsoynncpf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/grezdsalm.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gizjhxqdd.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gkuamziht.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gfkdqdvbv.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gjhcmbjuy.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gkjrvdxkc.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/ghjzzpref.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/grsribyyc.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gwoqkoktj.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gjsjaavwk.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gnitftquu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gmfyqkhxh.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gikxvdsor.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gpjvknwcp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gfafbjdxm.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gstpsrcoq.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gtmhqvjko.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gppbjqfqp.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gnnabdhsh.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gcxexduws.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gocjkheao.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gtnjbuqrq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gnyfgwsyl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gofopixdt.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gadhpartt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gpyaepwox.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gdsmmuest.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gzydtggqe.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/glcfxuenf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gudsokzjj.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gfkutfide.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gstylfbda.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gxfhvluhp.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/goaijepnz.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gbzyzxoup.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gwxxdwyfw.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gasmhqdvy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gfzuynbcl.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gefwaxwdw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gulzunzdb.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gluwdqdvs.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gruwmhzkb.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/grhslcdpg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gxlagongi.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gciosenhv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gixmzmfek.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gdauxmias.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gibkyplbe.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gjqtvoikn.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gjtxjxquf.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gxclmrgej.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gzocgcbli.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gxfenpuoh.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/guwwnmlaz.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gdnlwyelr.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gdclokmoh.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gjypmazab.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gxyzuqzzm.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gtcagdmsy.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gskhnxxpz.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/guavfmvva.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gyayfafnb.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gxahwbwlk.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gotjqpnkh.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gellingdb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gkzdtdptg.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gotjsulyh.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gxzdcolcw.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/geoakvmkm.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/goqfxmeiy.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/grejgavgf.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/grzqnqchm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gunpjeroi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gdjxmzlzm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gefrqsbnp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gbitykxvx.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/giiybrqtp.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gadeuluwm.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/grtwtvssf.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gxyptgzjx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gnleisegw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gcmqnbqmm.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gbhsnqnnr.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gmlssasgb.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gpvshlqnu.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/ghrgyohut.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gldlvarud.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gvdloboog.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/giemsddop.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/ggttzzvmj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gjawxcveu.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/guqbtmfbb.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gmudtoozp.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gttmfuijf.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gtsljuhdw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gfzsreamh.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gyytxwzfg.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/ghnsmrkly.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gzztopfgd.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gtzgaayuc.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gbizqrsja.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gpsztosir.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gaifcpirm.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gissrylfs.sHtML


<!-- 参考信息 -->