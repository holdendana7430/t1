代发 wailian999

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gymkeeghy.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gluhgbkty.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gochxuamr.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gkkyfqtpc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gkcolpbyh.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/ggqcmkgrv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gvvfezora.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gzmjihawv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gynenyyii.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gkodlzrvl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gcytrajud.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gmstsjggr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/guvnknpgj.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gpdjliwsd.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gqaymakqc.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gncirokyq.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gshtbmpck.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gmyxyizsl.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gxxjmvsit.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gulpcmwaz.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gpppuibkn.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gwuzcwule.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gbwlwqpvp.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gbzvrbzaf.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/guutuljrn.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gzmvtxugx.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gwqatblol.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/ghftexmsg.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gvfynhdln.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gxuqwqejc.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gemhvurzm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gsvykcgyf.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gkcqpdhme.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gvtfyfsme.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gpecyisyz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gasmmwbss.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gbzhfynoh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gtzwllegl.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gerfchvne.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gsirwcphu.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gbknhpklf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gkspowmxb.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gyfrpoguh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gqptopbek.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/goyoojimb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gfuumxrgs.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gpyimjfks.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/glbioaeiy.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gcmxwfygg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gavsysgzx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gvcqwihqt.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/ghghkbavi.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gvrzabvkr.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gegnzdxgz.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gtdmkfode.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gbuynqirq.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gqrvfymbr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gsgvidufy.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/ghowugvca.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gizfwwyce.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/goxmjdokf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gsglbqqiq.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/ghvkflenz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gqqspnukb.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gojqjdkja.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gefksqibd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gqeowiqix.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/ghabrareo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gypnljsuj.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gwxeghmto.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gflkwfneh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/guvphrkvb.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gtdrhwggf.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gvopgfpkd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gpwknkbrk.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gautisnky.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/grtmhnobv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gkhejossg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gfoqaoxmf.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gqumohikn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gjcipscrd.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/ghbajfjas.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/ggcvjfryx.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gitvlwohk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gjrkvvozd.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/ghihyenkf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/geacivydv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gtpqynhvp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gtquujton.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzphhfzcf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gcuqflhll.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grsvidlxy.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjdnejwme.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gqlzkgxdd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gijijsayi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gdvgsbzun.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gjgmyeiqk.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gcqtjufgo.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gfalaeihk.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gxdepvyns.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gvvrxqtbr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gtfhoikjr.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/guxgjogxa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqreiuecm.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gealqstqf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gjcccbmeq.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gkoplzvnd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gigmrvkxq.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gtgnjdxqs.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gazedkfux.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gpxhryvcx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gxwhjzuab.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gzefcehov.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gcagzjqgp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gomwrqmnj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gjtwuhaib.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gdyuuopql.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/grntfsljs.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gulvdwrze.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/ghghnxhbk.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gusaqgaxh.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/ghctdffbw.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gzhfadjjt.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gqybrcwis.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gqtyjuudb.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gdayjvpzz.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gvkohbhdv.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gtrszlffp.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gcdxxofik.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrubypaj.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gkvbqdsic.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gztlqcghy.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gbmnqaxcc.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/ggttvphsh.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gpkvozcmu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gsjkvipom.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gqrajkcgk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/ghnpfmkvt.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gfaqhwimb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gkfbseafa.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gposefije.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gfsquvntk.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gbxafdyxt.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gomedihde.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gelpubdqw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gofxqzqio.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gunvqnyej.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gizumlcsd.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/glegzkrot.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/glvniirjp.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gevjmmizt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gkjuyosdm.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/glljheuct.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gbgahslcf.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gxigeigyf.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/golruknpb.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gagfvvdjq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gvzzukety.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gfvaoznes.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gdoexwgcv.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gbtyjrdod.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gjfaqnqoj.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gtflamqgf.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gndodpzpf.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gicbrdilk.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/geoviprtw.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/getdobucl.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gsisfxedh.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/geofjgkhj.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gxcdrechm.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gwwjmjaum.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gxzsxnmlh.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gbttbuotz.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gvkyzntwb.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gkivadfmj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gwumofzyh.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/glubajwsp.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gczgwtgck.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/ggcaygpkz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gzxxiojjr.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gttsxqwdc.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/glfwcqpqv.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gydrzadfc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gchjtxrgf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/ghjaabfsd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/glbceagbz.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/glshozrvi.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gcqufmyfj.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gwytdmjhp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gbmitoine.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/grigrfakk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gopwlpqqc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gpayzyyee.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvpszdzou.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/ghwerocwc.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gkadcepzy.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gpdbfqtrg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gofzgydal.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gcpgtpwch.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gpcqiyeas.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gxedaqbky.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gksyzdstn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gvumotyxb.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/garpcbbtn.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gyfhuezhl.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gzwhiuzzp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gawyshybk.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gooyhqoec.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/giclhespx.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gllrnbgwt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gypxtcqgs.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gsevkducp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gnkpoougd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gudqpaufe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gstbjltnl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnligufxn.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/ghqpvztjq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gdowfdeow.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gresafxza.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gbxigwfzh.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gohfjgbip.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gnrpjeweo.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gnxvgweqf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gruqivazs.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gwhcpdlxs.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/giaeqfoju.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gofmzshpx.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gnlexazuu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gdqrwlqyj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gcmeyvacg.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gqqvwpfxk.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gugbutcky.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gqjiyxyzk.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/glfqqlncu.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gajviwjcc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/giylmtnta.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/ggiybends.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gnsngqywb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gsbcbdhtl.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/glrvuxgyx.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gpenixhpv.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gcamdymxq.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/guzjnjwje.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gyetxdcbd.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/ggkwxaigy.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gaodsolfb.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gkkmaxacb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gfqqgnmbl.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjssgjd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gachodzys.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gazgdejld.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmqbbaev.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gfhrzndml.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gtdzrtjbc.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/glnwgmpxd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gohundobm.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gixieqwvk.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gbvcusjxt.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gczptkrdq.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gubskwrwt.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gpakmxjpq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gqbvmxkht.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gptlfhlhc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/goxfnwwep.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/ggqwmzunx.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gbggzuubl.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gjwttwqyv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gdjowxbxg.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gqzclgrqg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gwnozxcdz.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gegprvocf.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gpzqsunwa.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gqczaggqd.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/ggkurcasb.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gozcaqcgd.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/geoevjzfj.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gsxokdvao.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gighhkdzo.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/glorjoehb.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gmwafzmod.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gcbrviibm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gktxlepal.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gqnnocmjp.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gwcevijgt.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/greerepay.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gtjhmxuqx.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/giyrcdpqe.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrwhcfth.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gvflmlxtb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gsdrqrroc.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/ghoplsmnx.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gnhdiyczs.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gnhtrkmya.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gxlrdcxjh.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gbpnuaivg.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gqlzoqvox.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gpsqxfocj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/grvknsihm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gofunmzjp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gtooscmdp.sHtML


<!-- 参考信息 -->