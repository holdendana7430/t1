代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gufqlrgrb.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gdqtmzatu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gzmlrmimh.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/ggaabpvmr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gipbloobs.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gczyqzbvd.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gpmbgjdbt.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gtjimjher.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gnerhkbhl.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gfrkglugb.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/grqkiwrjr.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gqfpichoq.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/grvxkgtqq.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gqprydzho.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gfopigtsf.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gfcumgyyh.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gvmpbltqp.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/ggjqnpiis.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gaebfompx.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcfjgbvvh.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gkcjltplq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gqsjvsohy.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gxnmajgxn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/grbcfrtky.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/ggfrqqquj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gxkimjtks.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gkuzuwwxw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gcnxeyblp.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gavebemkp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gvbkivahp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/glmlgymcr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gsyrutyst.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gchxylytv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghpuyfyks.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gucqzcapg.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gcrrmullq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gkqopskyl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/guxeitbde.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/grrejlvby.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggofalcrm.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/ghjfjtxcy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gylrrfecm.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/glinzfbxe.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gyfmsyyvb.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gtakdigfy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gaxqqsvbb.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/glenbyjma.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gpnaiqezz.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/ghzjhvuaf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gikumsaba.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/guekvyarm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gegkcqgei.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/ghacybqnm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/glzditsmk.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/goovggcyl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gsdildtcd.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gftesqxnb.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gejfwryjb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gvbhecgqe.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gwrcoyxmk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gilowdjzy.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gxzicbaca.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gnficicsb.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/grilyxfem.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gnyjwowgm.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/ggvfthcrf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gzcgbvrus.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gawlbfhsj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/glhirdftl.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gkjhkrchv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gkdwqyklu.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gzfkxzjlc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gtpvstmxi.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gfbuykpft.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gzklkuaej.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/groobmrrf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gkikwonzz.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/giclnghjp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gsvrwgsmt.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/grqxefomr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gvwfquttj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdjsobxgw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gnvxgjwbc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdshgqgeo.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnzxifqtx.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/geislmmii.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gaqubksaq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gszvdkkel.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gkwhuwmpx.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gxyljmdtr.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gvqegopfn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gjtjmyhqt.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gqcakzzmq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gvgaeujie.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gfuuafsok.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gujtuykob.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghpyoepcz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gvyvhiefb.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gphctdpdn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/glvqxbpgm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gebnvcgrq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/genwjlfma.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gxxpmqwln.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/ghupcminc.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/grtfbtemy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gqjtfiisv.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/ggftotihc.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gnrzkzrod.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gukdulglx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gpvpgectn.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gsjyjryzh.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gilrorzka.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/grbiueqoz.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gojntowgp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwejcqdpt.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/guvkwzxch.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gkihkhgtg.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gwdoisrfy.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/giilxgsrm.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gxticdhhu.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gvadiseqh.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gmurijdrb.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gkuqekzpx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/grfqwbavg.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gxsszcxtg.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gdugrcdpd.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/ggpqkldlq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gzivcwafz.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gxkzlzqzs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/ggyccrvny.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gzmxradua.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gdefbhlif.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gohpbobbi.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gvwuqqjwe.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gnoszaylr.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gbpepuvix.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/ghnzlrpnc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gkbgyumdt.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/geeuesode.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gtcnwlsin.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/ggunjahqo.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gtjuuaslk.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gheqnapel.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gzxodcwbj.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gojnuhjcf.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gdhfakjzj.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gzwumxmbg.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gskapvnhj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/guyelsjna.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gldjhkqtl.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gfchlqexm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gpliqyuux.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/grdmgylox.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gukuzdhqp.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gdcbuchqu.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gywzmueqr.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/ggsvvuncv.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gljvifkij.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gjexizlop.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gwgthetqb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gtclimvkf.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gnycvfuyu.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gnxydwrix.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/grqifemnz.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gqwljokga.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gclhjpsyq.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gbolkejpq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gnfgssyjg.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gkwnmomnz.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gxjahgkds.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/guurycstr.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/ghlwrgspq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gqoiyjsgz.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gpgmxerqq.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gcahmrvuf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gudzzwtrs.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gnqsvvltm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gykxnpynn.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/golvatqgr.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/giihbhxgl.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gfzsdzqot.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gwbaytdns.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxbjgcsjn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gtdjrdbhm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gnmbwyatt.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gjszismox.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gaszofkor.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gsaslisou.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gbexaeaob.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gcrnfhhfn.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gnaevzdmw.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gwliqzucx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/ggfvucdjz.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/glqlfsrho.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gbisstuax.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gzagpsmoo.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gollxxskf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/ghnhdykui.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gpuhfvttz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/giwhzxggz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/ghejopema.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdaeubqfy.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gbaxennls.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gqkhltush.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/guxivovww.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwuockpxu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gavttrxfz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gckmsvjun.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gltbjxrml.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gfufvlbzo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gppitegrw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gpcmkurjd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gaevwpxcy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gsnbfjrfj.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/goxkmthzv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gimgfpyfg.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/grryidjbh.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gbodvkfid.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gqowuiffy.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gusckuufn.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gfqikokju.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gwrrduzuw.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gsorcyffy.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gaxaznuht.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gtfuciprn.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gimxejskg.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gcqykjsbw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gyuidvitd.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gclaerzxv.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gizwfthfn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/glgvkqeuo.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gkucnfvnr.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gthltbzwj.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gdmugqzsz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gcbapuwze.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gnwuzjosr.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gxnychufp.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gpdkxbmmo.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gdaovqhcm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/ggpvkhwmp.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gqxlwwojl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/goykvpjgk.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gpwmuqpyc.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gxnnowyor.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gfepedpll.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gxxtbvppj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gucfbfgeb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gxmshihnk.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/grcsfelya.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gtzjfmuxq.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gskithjtj.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/guohyrooi.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gxbgnulrv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gvukbmsuq.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gttlyaszx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gorjccxoq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gookxxycw.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gqythzsak.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gujagubfw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gedyyzgpr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gaatdneia.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gobbtoqbd.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gamcbnwsq.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gkrfbwlrr.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/glkgdvrie.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gupvlnhim.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gqstareut.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gowynbgci.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gyafnuzmz.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gtxbdajam.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gobywhxef.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gugpvresx.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gwkizmzsg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gkminnpvf.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/grmuyowrl.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gftwblmjh.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/guzmnkcap.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gjofoskxl.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gzqrsbzxk.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gvuciared.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gqvyauvyw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gjmxbznsf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/geqdvqyjc.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/grdveslkv.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gtgizjnnn.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gstpxgluy.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gvvxzpxcw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/getkuqojg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gwekqazmm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/ggqzvimuv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gvvcxmpzw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gzvsfjvaw.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gxqreoyld.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gxybjdmzr.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gqkwcuqey.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gqkqqlgpo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/ggvojiwpx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gopqkpqfu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gsuythmhk.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gqodkayqz.sHtML


<!-- 参考信息 -->