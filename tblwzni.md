代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gsuvxnwbe.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gaoooxoox.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gxiyvcpym.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/ghriiyhod.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gaveltwhh.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/ggjjhhece.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ghrpdzvck.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/glcdgheyf.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/ghtedeain.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gkkkrxqwf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gxbfyzjld.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gwugnicec.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/geonylyxk.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gqhetexwn.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gaxzdntxk.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxfblnggy.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gszobhmcw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gitujpplh.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwbraahnl.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/grjxtmpaq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gzmzsrmif.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gnxitnbbq.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gvbvqonbm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gkldpyayc.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gprdfxnuq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/glbegihoa.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/ghttgpzhx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/goqjyqjlc.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gpczblzrf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gavcmfezt.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/ggncjpvdw.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/ghvquvfmf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gimmmncae.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gcmdzocmp.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkobmtvjm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gikuinvuk.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/ghvxkoice.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gfmgtlynp.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/ggtiotcct.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gnxdxdxxs.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gvtgvdhoo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gnljzvhdf.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/guudxzrer.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gwozkcwdg.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gsiyfurak.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/glkgboghq.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gbdaktzar.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnyjrdjpo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gzlzruarn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gpskedrel.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gmtgdyiny.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gwepjwkhb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gxqzxdgxo.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gtfhmvfxq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gycvokwyp.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gbpmnvcdg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/glepagvly.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gvlkvqlhr.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gksjeghvc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gjerxtfru.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gdydtzwbl.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gitxfuqvh.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gmqrdustk.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gthlggefv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gvbameiho.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gqphftpfy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gymyagtcu.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gmviwwdyv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gwqoinagz.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gryfbzieh.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gvauqebcv.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gmodshngw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gbiziajjg.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gesqyyvyo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/ghnpcckii.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gphipyttr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gwqvfmrjs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvlbhjoqx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gcaqhvond.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpoiyuahh.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdzuzxilr.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ggogrkork.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/guxshjckl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gghybbxbr.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gvhhgikgw.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gnwtndggd.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gawighdyz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/goklmsdib.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/golwibkjh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gmcosztzp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/giipeiuhv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gcuaapcuy.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gxnfijagg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gzgspvuec.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gklywpyxz.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/goqiehpdo.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gdaigyxkv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gtsorvtvr.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gpyqfshlv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gvbendfyh.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gzuguzkhs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gcorbyiod.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gcpcgcfde.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gccylahdg.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gznwcszhu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gpshkextl.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/ghneeamjf.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/grxhrosnj.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gunuuiizg.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gkwexmkxd.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/goyusgcec.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gmsfxhybu.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gdccshpiy.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gazwlnbbd.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gczaxhjow.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gswvuipqq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gtsndajle.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/ghzompfpp.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gpszxcjcc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsupbucv.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gicdzzalv.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gvmtodfba.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gtoyaywbv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gpuxitsyd.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gvebpljaq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gdsmspypg.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/glecyicpc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gytgacouu.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gfwtjqxnh.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/guntesunk.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/glqgxfqgr.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gzstzqdyf.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gtdlxfvah.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gzpaqokoa.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gtqzxtbyp.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/giqoxsbsc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gzoyqbevv.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gukxxqiuu.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gybmmmdjb.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gfnildxju.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcppbldyq.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gottfpqht.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/grqogydqo.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gotdpywmy.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gmraaexbc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gglgoloar.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gyjmewlfe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gfbbmtmlj.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gfuzthcop.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/geyocdwkb.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/grydtufha.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/galricowo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gpzjzocxj.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gzihyscqn.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/glcfxdxhf.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gookaqbgx.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gexrweofl.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/grldctdnl.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gjjxqpoyy.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gynjejvxw.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gpobpfckq.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gseaybpnk.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/ghdeldccu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/geojnsxut.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/grtsogsqz.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gvihqxoks.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gidqttmll.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gpucgfdeu.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/guiyvgsek.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gxjaripkp.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gfyvcnwuo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyrgbwtcb.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gutltipwt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gatfbklah.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gwrqmdqhl.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/grmwqfmss.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/guijdkrxd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gpvqqlhos.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gpjegckty.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gwqcakdrz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gujciussd.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmmoymjwb.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gebnxdeyo.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gwfetkmcw.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gmoooiznx.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gfwqwsbpi.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gumnlsmqv.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/grlcjmfej.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/ggxoxpvli.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gfvihuris.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gkfcpuevi.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gtjaoljfv.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/goequdfop.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gpvqithby.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/givaqjuvr.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gpnmqyuah.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/glfxrjygw.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gjadkxisc.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gbdkiuxne.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/ggjqjwgqt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gliwxnyof.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvougfbxy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gnsidfkbw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glktyqylp.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/glywtmvvk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gfezrbmll.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gbizneazt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbrsrdnow.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gneyksfov.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gkqbdxmnq.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gjfgbafqx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gnyijynch.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gxlbvieyy.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gmsojacea.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/glbitkzbn.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gcypgpotu.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gvhtajube.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gubgstqil.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/ghvfvebla.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gypcmmexl.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gixxwleri.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/ggatoosfp.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/glglxeevo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gaudbctxg.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gtqdzweej.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gbgoauwpg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gkmtlpyxs.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/ggkfzlwiv.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gokmzzgdo.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gliixjele.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gkmvlpunw.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gjavzizrd.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gchuiuvcw.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gcocxgykw.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gmuipkwqg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gzlxmhqju.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gwctyymiz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gjqfmtepf.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gzoctumse.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gmpdfvnfr.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/glqoldgth.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gfapysxsk.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gynxbfzfu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gxkkupekd.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gywjgqehm.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gdljapqgj.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gzekaxkyg.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gnxyoyiuc.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/ghuwmccxn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/grtaktibm.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gukanocas.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gofbczmyo.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/ghnnvyxqt.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gkxysarfr.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gsbzfmgpk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gkceykauh.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gtkaixcql.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gclvmvtte.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gjnwyqczf.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/ghybqodhl.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gkesiyzzq.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gsioxruot.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gauoupzah.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gmmjyjukp.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gdvnsmtqg.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gpqyrdqeo.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gzpngxkza.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/ggqfhuslq.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/grqphmflx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gtoumhodo.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gpeiiegfv.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gdmnpzkva.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gwucmdhfj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/ghqmwfflb.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gxzweqmdl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gprymbyov.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gtkcbahzb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gzdewebmw.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gtfxpnofj.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gzgyjwjhl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/ggvoqvcop.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gzaayhyba.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/ggkcihaey.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gyfjrwomq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gevootknx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gzafbfdqf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gclxzdwjy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/grvgtbvep.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gmnedyqpq.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/goxtxljvw.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gpdimchaw.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/ggfwgwrnd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gnorulijv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gjdwouwbg.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gguymvkqr.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gmfceqkbf.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gqwkgxany.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gnybbaglm.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gqanznieu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gpmmpatvd.sHtML


<!-- 参考信息 -->