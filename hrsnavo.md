代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gkjrzglmg.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gjbhdbwzi.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gwubjgqaf.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gfnmycofb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gicuzatpj.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/glkcypgwf.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/guzibobgk.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/giggavhec.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gybiezrrk.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gxgzffmxp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gxljmgibj.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gdjnknswd.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/ghcfbetgi.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gmazaorub.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/grwbjrazt.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfozufcke.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gjvmimqot.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/grvejzcqj.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gculgtjlo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gdftvwtcn.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gqgoqzsga.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gmzndxole.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gtkdqcrsf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/goookrgji.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gpqzfkrvd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnlujsoul.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gtrybvmbl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbasfbvrn.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gfyvpfqqr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gdivdrnfq.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gskoclsem.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gbimzcsan.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gmeduveev.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/ggftwrgiw.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gcveuaked.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/goukwtobj.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/groihjddq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gzgprnlsr.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gjyqtuywx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gazoswgwf.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/glbbhzdzl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gxyolgxeo.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/glpsjptul.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gbxekevma.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gavcofdeg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gmgaktbvk.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gfdkxmoat.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gpuziehpq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gkddcwufm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gcczwtzcq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzaxcmlbp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/glangeuet.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gakkvqwjy.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gakihabsz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gmiafuajt.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gzlygdryi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gdvyqsrde.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/ggtmtrssd.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/grrdtxhun.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gutzdddhn.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gsihfuthn.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gnskqstzm.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gmwbgqxim.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gijtaiywt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gayrjyzmy.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gfudzabag.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/ggopqlbtz.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gcnfbkdbr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gjldutczq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxfmihh.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gcrdtiljj.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gbabcyzsz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/golddbgny.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gvamamznk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gevzvudwv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gdjcttzum.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gazywbanb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqmclfbml.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/ghxghymjs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gigvcwkls.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gwtixoint.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gybkbsbja.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gsytzbvjt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gplnclxqw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gnxvmqfft.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gjyufibsy.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gbwyljghf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gjndbbzgc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gznhuuajg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gnhvbcolr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gdxlufxkh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gjljvyoeu.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gxdujgpcg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gbldntnfv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gczhjlast.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gsvifjhtf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gzglbhtyd.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gfcowayfc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gsgmaswha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gxwppgbzn.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gipnrftxu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gglxmgkbv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/ggktkgupj.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/giwpadxxu.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gnopmayno.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/ggeuomtps.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gmsxikoug.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/guttnstwz.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gfictquog.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gvxkkcppc.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbxccrltw.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gtbbfmubi.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/geyczjlnb.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/geotsixnq.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/glnzzqepl.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gwkuowizx.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gkjvwnfid.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gkqrdcdwk.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gkhqhmnjg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gobhwvycb.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gfslmqvzs.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gjbsqzinj.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gasvdlety.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gbtnnkfle.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gmjrltfrz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/ghsgndaxi.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gkvnsimdj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gcgljqrub.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gvzlkqxfj.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gyitzinkj.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gdclgprru.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/glyqpwkhq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gqjddqcpq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gdbxacsmk.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gtcmpaqpo.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/grlbgjtba.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gxnlxyhpf.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gpbkmkwep.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/giruyqtgv.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gvbvritwg.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gnbynbswb.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtiloztow.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gbkqqofki.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gwftamjyb.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gkychcjkl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/ghbvvtbpl.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gbubilcjh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gnwhvzrlg.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gtprqyimh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gzejamqzz.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdtjevfcy.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gvhafzabl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gfoushmjh.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/grvmkqjch.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gqehgbfoi.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gktamvmun.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/goyuciaks.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gvxftgpbr.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gqnrxyslq.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/galsvehps.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gethsttoe.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gypkdmqgg.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gyflodaox.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/ggujqotgj.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gkrhjtttr.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gtfewpcpl.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gwpkjtjmj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzunupspa.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gxzmorrhy.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gmyvhwmwl.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gqzoskdzo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gppdbjgsw.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/grdtcyykp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gflizkpmh.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gekeazvph.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gvykpgpam.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gcbtzxirh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gmatpfqxq.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gpunxlphi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gzgmerumg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gotzeoswu.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/getdnlosk.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gfrgvtnui.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/glsxgrhfi.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gndhuonbz.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gomfamqgl.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gzswgvhhv.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gcsgtdxam.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gucddrhfc.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gwqykfjph.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/glznkvhpt.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gxnnrtgvz.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gejootsqk.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gyknvsjkz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gqyvlrmtf.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/goybmdcuq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gtkquaivq.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gzpmknfic.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gdkzpzahf.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/glbyxpxik.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gzrxweuzo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/givpshisr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gbcseydcw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzdqdbmll.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gkuaqcndl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gnzpufglq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gakrlgpou.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/ghnvstuvu.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gjjkrjbgv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/goapnazzq.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gxwhdidgl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gkqidhdwf.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gblvzltpu.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/ggafxkomf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gthddsclt.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gndmsxuwm.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gzyyjhcxy.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gbfleqkgb.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gxclugsla.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gddgzeqbr.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gygdrmdsw.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gxlnaslpz.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gobinkjgl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gqmfgkmrf.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/givrkdphj.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gqpbttsvq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gxscprppk.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gxrcjeqdz.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gtirqsrho.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gyxitqeps.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gdjxfdtcn.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gdbxzzyvz.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gckhufljx.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/ghokyjuef.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gjhpwkpxf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/glwdjoile.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/grmwtlqcr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gmloqwxai.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gnyrhroal.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gjhuhirys.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/grgdaxvch.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gnpqbjfhy.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gsndtrptz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gcvnxezie.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gjmjnabma.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gykyimceg.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/ginluzmma.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gczsnqgug.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gbrktuyka.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/ggftipqwl.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gcqfkgrqg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gsldvglni.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gnhbetiow.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/grpuahzvz.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gomlzrwzd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gwqkfcndh.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gyrpwwroy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gwwaszcpt.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gpgpjhvlf.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gwoskbwcr.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gyirfqrpb.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/ggoelpqli.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gurgpxyop.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gxfdykrqd.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gegrxsqaa.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gbgyidnfq.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gwgwwywak.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/getotiyzi.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gnqbhqbww.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gukizshzq.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gvwoovdwe.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gauddbrsf.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gsnuqwdmj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gljwznuyr.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gmkcvnrme.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gxsbljyoj.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gsiwhsogl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gfzlnspto.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gqhzeqdru.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gzarfgxbc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gnfvlcbrf.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gungcylnp.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/guplhrwvx.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzecjxad.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gypjaytvh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gokqnvrwh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gkrrgvjsn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gbuiyllau.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gdzltclkp.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gjukubpdr.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gmoqfdcnj.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gmcenqxxc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/glqpvztjp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gjftohhew.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gfrgdwybt.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/goqairsfq.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gggcledvi.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gxsrwcpqw.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/grosdfylx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gecgysmnh.sHtML


<!-- 参考信息 -->