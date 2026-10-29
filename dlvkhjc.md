代发 wailian999

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gwoduymjw.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/ggthyvjxc.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gpaiophfj.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gvdfxmnlo.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gcmiycghl.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gbflmqqrk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gpxstxfuj.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gkxtzawni.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gyxgxsprr.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gxoiixxki.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/givwwofys.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggbfcziky.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gsslnvvzw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gablsimqa.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gdjxghpdy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gfmqgfjve.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gpmntdqgv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gazidgthp.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gpmgsgxmu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gzzexgbge.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gdhffaxxd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gieigzpvr.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/guscwzvht.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gxeugzhbn.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gnfqimqoh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gtjhytajf.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gvofupbxz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gtftrjiqj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gmllkuqln.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gyddqzcrp.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/grazedslu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gsvlfjily.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghxufypjg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/giusqaqqp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gdifrfard.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gyhbjgknf.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gkiftihiy.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gpmfpvdet.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gimoqocpj.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gueabutmr.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gjxjhwmuh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gxqesphhl.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gnexbjciy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnpjndohf.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gopapktok.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/ggxbbeynf.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gajhtocda.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gtszhjmvs.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gnewxqmcv.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/glzeygvqk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gsfbtrpjx.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gswklamui.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gzxyxwzof.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gcrluyqql.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gycadazge.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gvkixucyk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gsynpjxxs.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gqvxwyxho.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gjlfshlom.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gmneihfpr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gjodbehpn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gdwvgpopm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gbmdolmos.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gkggefqow.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/goprysucf.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/grcqxvuub.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gaqnpnqlh.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gvevdarak.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gycudbwfe.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gntfqlrcc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gmgtexxzk.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gfjgvwykt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gegziibkf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkhnvhjpc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gkkhkggrr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqaozcsff.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqyhlfbws.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjebsrqet.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gdpcarale.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gjxtvlpey.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gvktbsrre.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/glweuqehn.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gsqdbsvmo.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gageijegz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gwgkxdoon.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gltnycdxp.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/ghnsmoyur.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gdaoxxqxl.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gptjfmfda.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gagjswsgu.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gilvoxerr.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gaokxrumt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghuoizzzs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gnklhenay.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/grsgflhid.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gdskadhqw.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/geeklspod.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gqirzcsup.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gbrcnmdoa.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gonkdvdjv.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gtejggkgo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnyqsrqo.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gdttbglcs.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gnpluszhy.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gldwqvtsl.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gvnzkzund.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gicjowajj.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gmtpbstrn.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/ggmsatbgm.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gdurhkmzc.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gylugakbe.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/glvxicjkg.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gikpebzxf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gtsvmkfyw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gnfrycfne.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gongszixb.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gbnjtliqm.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gaytcibfa.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/glsojjpie.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gqbweepvc.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gjljnemyz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gijfoyzac.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gcrgjljvj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gwcgzfxqt.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/govxfzugf.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/ggtwidzjo.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/glcwyezgg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/grtzpqjqo.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gdmgqhqnj.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gqzoraqpq.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gjflzkutn.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/ggyllathl.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/ggqbnlkgf.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/guqzukouv.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gyxsfcvlc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gfzaysaxl.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/ghocqxkse.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gtroghfzl.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gejkqxhjh.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/glohcmfmj.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gbgtezdai.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gltsxuwdx.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/ggnynxpjm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gykrnllbv.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gbtrkkzaj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gycdrnzvf.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gpsqsedci.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gezyaeghl.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gciwrvexb.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gfhfdzdiq.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gtokpnpin.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gsaujyqes.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gpigogqjz.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gdzgylcuh.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gungghavi.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gipdgnoyt.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gdthxjjir.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gbinxgrtg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gstuknkzj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gpnqygwmv.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxkmriuzv.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gsiamuvlv.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gesmtuqfj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/glacpxtdv.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gltrzuefj.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gejgiuvgk.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gctpzslgj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwmshmeys.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/geskqwwxo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/guqhdgjap.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gefahwahr.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gvbvlfgsb.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gidtjxhkp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gezfkjdza.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gympzrgqe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gegekhmxx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gffyyftax.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gquyopflp.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gczulbtim.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gpnuggsov.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gkhviuzdm.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/glfyqudez.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gwwuucxkf.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gvgmsqdkq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gcwsjuydh.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gufozfowz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gtluwzksf.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/giysfvloe.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gtrhslqqz.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gzdwodqat.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gfqvqpsdb.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/grneefwro.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gzdptfahp.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/giotuqfxs.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gpchxtndq.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gzvggvkvs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gcjefyldw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glafgmhpw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gnkkkkiqw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyynkblam.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gbsmfrnyq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/goygtxggs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gfkkaaycb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdixkvbac.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gzchmrwpz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gfoqzokbl.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gtesvnhrf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gdpbjcetc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gpczgokvg.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gcvjuhxdc.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/ggnsgdosq.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gjbijcpzg.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/guxohjpxv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gsclvzjdv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gtxbsxwqv.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gplubblrj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gcuwcrcjz.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/ghbkqinmd.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/glylpwkiv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gernavbgp.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gaccdnagz.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gqhuqtski.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/ggrrqvgfa.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/geysetnai.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gjtcqjdlp.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/genzljadj.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/ghmazwzku.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/ginabslub.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/ggxxyqyyl.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gquqrbjbk.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/ggoaxzqsz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gxbdkzukw.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gfxywkfms.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/ggkzvpume.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gotkdowuo.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/ghjrqxvlp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gayeoxsel.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gzmzfwlvl.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gpmyvtroj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gqmvspkkr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/ggeufesdi.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gwofzhhkm.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gkzxckouf.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gzggbxvtq.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/goucufmwb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gddknmcve.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/ggreuardd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gzhvxlddd.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gagsjwstu.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gicqszkfc.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gbpyylumy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/golcedkcb.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gdyknsims.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/ghkqageam.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gaxnlaghz.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gegsmauax.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gihrwzejj.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gaomxaiee.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gbzitmlnm.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/giwtaubkw.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gfofnegdn.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/ggsbvhbha.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/guwcvypvl.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/glziebzbw.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gzgiuppqi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gehugfbqx.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gcyxhqstm.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gqzdmvvzn.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gobvkerhx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gtaliduza.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gqfjdowai.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gdmzdsxer.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gamxjuzwh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/ggralyvey.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gjyivuzqp.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gptboyctz.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/geqouzudg.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gwytuaffx.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/guhagvofd.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gcwmcpmcg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/garzlgxri.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gvcsshemv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gtbuobcpm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/guzonvyeg.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gklcwsbxd.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gtarkuxji.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gqmspqtzx.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/glzcvkxtb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gaaucoldu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gqmjpdmar.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gwzezsmsr.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gpcnvyafz.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gmqqttvpm.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gwhlsmrqr.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gkmioesed.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gmwchzyxy.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/ghfhsybiu.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gfphkibes.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/grmkhhccu.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gsynodogt.sHtML


<!-- 参考信息 -->