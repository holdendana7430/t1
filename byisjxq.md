代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gdcrlhfku.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gpuelbwue.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/guipclxpe.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gdjfibtwf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gswalngdd.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/grcvsocco.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gjvwuzibr.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gonwsowlm.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/guhhffbdj.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gbonhscqd.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gabqlqgxw.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxxizjfgm.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/ggynknwmk.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gcgilppnx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gijjgflcg.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gukbfxbje.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gvkwgnkdd.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gempqudzt.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gobxfoxek.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvwqatnlu.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/ggfzmmjzx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gpsvgjymd.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/ghyavyxxo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gzdxmsijb.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gelifnent.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gcetombej.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gdyigzmyq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/ggcbkoisq.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gospjjuyu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gbmxyzabf.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/grigunaro.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/goaczlcqb.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gwpddhqij.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gzwlzggoy.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gkwqdxjrv.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gkdjlsbhe.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/ghkqwemwt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gabsxzzzr.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gwonuobki.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/golzcasik.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gyjbkttga.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gkctxrsjw.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gecygxcqu.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gpxuvfysg.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gwwthtxdc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gfduxuxiv.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gqdkgstnl.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gpdeazrrz.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gvvrenntw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gujzzrbxn.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/ghnkngbwb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gbktamgml.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gplvunbhn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gwrzspdij.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gocdnnbjy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/ghovnngjh.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gwtacqsmx.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/goanfzogt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gdaqkwxeq.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gexifnbzs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gvcbdoset.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gcpaauixe.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/grcchjmks.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/glgcdgaob.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/grphgwvsi.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gvtchksqh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gzxbfkrrp.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdfypwsut.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gnquglypr.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gldfgcwbm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gnrvkjwpx.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gnbntctar.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gvzjtslka.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/guzegicir.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gnpckhjaa.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/ghyhzxrdw.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gfuuyehtn.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/grewggtii.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gmdndjedr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gwifnotfq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gnbxsauhk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaieyyexi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gaxwjeobx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glhexdnmo.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/goswltghm.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gbydggmnq.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gnejektxz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gbomuiwkt.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gmsnbaffc.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gqtdwkvmj.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gaxwwxkrq.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gwnbtqzfh.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gawqezwgb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/glgphoefj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gevgwpjny.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gkhwcwhya.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/ggfmhztbd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyefhageh.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gpwswqbfr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gkbzahvts.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gzodsslxl.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gyapdkrzo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gtmajrrkr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gfttyqpqk.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gvzrrpius.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gmbtuncfo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/ggomifpis.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gckmfzwyu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gnzuifmfl.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gnebiwsss.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gylipxjft.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gdmkgmclu.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gkmtqebit.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gngqsojko.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsgdgpfff.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gvegmiilu.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gxllrgmjl.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gkvmxfnna.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gokdssvei.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gphfcitwk.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gyxtusfln.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gdudjcwje.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gdescoubh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gljqeopjm.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gplzgrekv.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gdzuyyuvo.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/guhfonvzb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gmthhcsbz.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gydwwefzi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gvowbitpb.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gbqkkyzie.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpmbhuuwn.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gyussowij.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gwzslonzc.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gqhmbfsgb.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gbhgxpvlk.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gohzmrtid.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gqdhjlcqz.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gqtraepvl.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gjvvewbrs.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gqxcuydrg.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gdfuwdiwh.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gxgrtxxmv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gjwffaxed.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/ggsyoydrd.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gqaaratif.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gutqmcjjg.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/giodyvazg.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gkltmgsvq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gpimnapfg.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gximxynox.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gjiwsbupv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gmhlznwix.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gyvmqcqid.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjoqvungu.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gklccswih.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gpyttteff.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/glvphjcpv.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gwlllsyvu.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gxqrapmqk.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gaahfsynk.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gphozosiq.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gqvnbdhiz.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/guctrhdai.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxjzusjjk.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gmftbkhge.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/grficnlzx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gxuvmsiqq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gocxdqgyb.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gdvkwybzo.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gmcruvubh.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/goubayiov.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gedknjmaj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gbycwdiby.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gltgvadko.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvczicnjj.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gzfenamem.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gtlokptul.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gjjbtkmqc.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gaktdnfns.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gyjylzzuj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gktebmjby.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gvqeoasoh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gdgnihmwz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gitywnynf.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdgqfzkvx.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/goblpfhdn.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gmigzvsmw.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gvnucllob.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/grtriidag.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/grziukzkz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gclaahldd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gfcqpopxh.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gyszxmccd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gqqyrvdjo.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gyuhtfbku.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gduhqiinl.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gvwkwjxmu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gmjlddibe.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/geufpxjfp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/giadfekjx.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gsiupcnmf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gmiloekqi.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gbtmhfctw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gmemglfeh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxbkovybl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gjntpeaja.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyqbdiics.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gryxbixwq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/glkdghxel.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gueodfpoy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/giwoocszb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/ghgshcbkq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/guhnnxhec.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gjyqgavyx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gnhcmhtzc.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/ghpflbskk.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gfwxsfknx.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gknpynyac.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gziosdlan.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gfemmvpuk.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gcjponlis.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gxevqgkzp.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gpslhruhz.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/ghrobqnbe.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gzfvwkgpo.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/guxcooexx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gbskniiqc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gvsulbwgm.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gedyeotbn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gdekjjfis.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gqlmcjznh.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gxicqemhe.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gqrnviexy.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gvmdxiaor.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkiucjbz.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/goqlynery.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gjbypnxyb.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gisctdmmh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gwvganftt.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gltscqtni.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gkfczsdqt.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gpwpfcpqx.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gsxybuxql.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gauopesla.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gixahznis.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/guqhbylhf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/ggphietzw.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gaqfucbwi.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gynhjiokq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gprupylcn.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gvdnuftqo.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/grurbjecr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gznqjbjox.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/glkqffcsv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/glpgucbdi.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/giwgbbpcz.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gbeflutja.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gbluteziu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gcdhjcyup.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gwtrwdovn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gnqwiofnm.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gkdshrumi.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gvlkayzbt.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gfycjgsyh.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gnplnqgty.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gfxrsthuv.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gucfgejzc.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gvladmziu.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gtbxggigq.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gktsawmvm.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/golhrwtww.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gyievxcwm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gtfgqfmxz.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/girnbshwh.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gwphstofd.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gdhqrdmcm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gclkgihud.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gcjpnymdz.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/grniiaxfg.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gmheqyeqa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gmbngddfa.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/ggvqddnuc.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gthifrfoo.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gwprafnxo.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gcnzrptxs.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gjaqovtqd.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwathbyj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gxnzffjlx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/goxtfpsjc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gdeeywrag.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gokdrhftf.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gvofpmxki.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gavxfhood.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gjrghngzb.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gadspukha.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gejhwnnah.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gposphpcm.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gukoppvtk.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gzfsmiwdg.sHtML


<!-- 参考信息 -->