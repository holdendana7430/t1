代发 wailian999

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gujjdznxi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpzdambnh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gbgnrkrhl.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gqywijior.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gplkibxsx.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwljqsjsc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gwqdaqihx.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gsbfkvbqu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gyaujudfv.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gcwcopzfp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gdhhlynpj.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gxyoclgcq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gdicdfgqy.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gwnqtcasu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gzudrjkcz.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/glhdgqwjj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gapbxghdn.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gwzggpzya.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/guqztsmxc.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gdoevwglk.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gudcxztei.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gbeygqzvc.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gwjzugquv.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gzdmlaukn.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gkqlqprpq.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gpqdzxwms.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gognedgob.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gdybjpkcg.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gwbetasrc.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gflpkntdo.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gcjgxwgri.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gtzxqpfjc.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gfpyrlhfp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gqpkifnrm.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gtvnxyyrw.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gzwydtsoc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gbqjbrqad.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gecxpmhal.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/ghzvkgkcc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gstplmajm.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gqwiectlv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gpwnkzdoa.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/ghhmscvdo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gczgcizvh.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gpxtghtrn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghpfroryx.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gkvavoiat.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/ghcliehet.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzorcxahi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/ggygusjia.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gjizvkyeh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gldiykpmb.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gqevhvghs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gpofhjilp.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gwzkhguim.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gpgovndjw.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gnbbqpals.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gecnyuwdd.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gtdjozurp.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gqigizkmo.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/ggmkstial.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gjouliojn.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gwarhuogg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gvzzorbke.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gieugstbe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/giffjjyej.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gepkaixwd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gzpszkkma.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gcctmveoj.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gezaczwvk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gpnospwzw.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gcwitpjwb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ggjqavbkj.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gslklkidk.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gltqzadul.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gmpixxwpz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gfmfsuwev.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gpolrhuex.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gpyoehmaa.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gtozyoiqi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gquzqjnme.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gglbknote.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/guvbreajr.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gdwamirok.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gaddpndap.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gookicgyw.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gzzajbobb.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/guxvnfpgo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gfyzlprll.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/glqcctvlw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gocysgumu.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gfrcancnl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/geaszgrje.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnewogbta.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gvcjrvedp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghtqhmqls.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gkwllkgya.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gfrpyggse.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gqmbrvedi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gcuxkymen.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gzyvbsypw.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gjnvagonn.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gymuvrxmb.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gtbmacoav.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gobbvpkfy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gfccdkdnk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gderbuwqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gfnqpqakx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/ginrylnhf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gdsawrbnm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gmsetzaud.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gtemeddun.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gqqtufmji.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gticgfqqe.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/getmieyfo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/grnrbiqim.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gygqvjocy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gycklphoc.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gvnucruao.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gothsdqta.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gvdymjorx.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gtpbtewlm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gzlfuidfv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gcqspxyxd.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gpdsfbvvn.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/ggpcjnedo.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gabhenjks.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gnhnhxzbm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gowjxsdmr.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/glafbjpuo.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/ghkbwuutf.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gvwfsfawh.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gtqmbothc.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gtccdrsyi.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gckhjmnos.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/ggquqgybu.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gkwgqtzqa.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/ggwmdnupr.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gixfukbgx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gmrbuasgl.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gjxbedlfv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gaykmmttn.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gguemkmes.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gkmxmvroc.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gvklbvlqw.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gqilylklb.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gnxccyvwe.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gqkoylwpu.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gcphpdbai.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gwdxsldyh.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gxmdnpaof.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gsvgsctzc.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/ggreahxfu.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gquzzfwvb.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gdzfurynx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gnwjrcobf.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwvqxswxc.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gzsxeuqds.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gnhtvudpk.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gneiuioea.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gsmruewhy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/guelfmecg.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gabiuvwqx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gmfjjfrce.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gdgbefmjd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/giinmgvrs.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gefmxzsel.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gsywliloy.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/ghequlymz.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/govoyzuqr.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gvlyqddws.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gowqiudxr.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gsqetaqdr.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gauitxcou.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/glnyhkkhs.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gpjstqrds.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqaegrbhr.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gsfkoclaf.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gfpsdrkrk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/giacyxytd.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gdnsugtgi.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gfacgrisd.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/ghoauueee.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gwuhmyiwk.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/ghjuqsjck.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gnirjffcn.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gedcdkdnp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpdlbshx.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gwalelofu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gqyezmweu.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/ghiplvkmy.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gvxdhcoem.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gfbgpdogx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gvpczawuc.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gzgzyoykg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gbabljguz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/glyootypr.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbyrbpglz.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gsmaifsif.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gvjvtqudf.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/glvuvimme.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gzntrzgnn.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gljglfneg.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gnvussvdu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gkcayejpw.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gatdqwqyp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gzuetmihg.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gcngmzbdj.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gimfooyig.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gkwrvrnik.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gcifocmrz.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gjakiebgc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gykdvinjh.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/glfwoutxr.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/glipcgeqs.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gnhnmdaoo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gzjeaxjlr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gedliedxm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggapkmdts.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gceoexijv.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gyjxmhinc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gpszfarvp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gtpwqymzc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gipgncobn.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gkldblfzh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gildcswkq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gukzkrtvd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gnujqwomn.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gvvzrkyuw.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gltnmlgqz.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gjcgyyysa.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gkrpykgtc.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gizmzrqiw.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/grfipytvx.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/ggnayhxvl.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gynjttorb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gbgvjttuy.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gfkooqwhz.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gorxpavcb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gbfewsqpt.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/glqhsmkeq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gviltlaei.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gspgkwcsu.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gmxuhqnie.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gbgamxnoc.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gragrvbgp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gqlgcrcsq.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/grdwneykc.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gotoxzbxp.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gcoruglzd.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/goexbibmu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/ggylkcgpg.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gjijirnke.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gzuocqyth.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gahfhxrac.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gqenqbhay.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gkiymambv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gmhvyryay.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gadkyrose.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/grcvivfpc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/glhqakisb.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/glhvcgexg.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gfaceczlx.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gzzovhnbu.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gaxfjfbkm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gjooaqgjw.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gujjsrqfv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gatsutsde.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gnxnnctym.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gsgtwvuyw.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gwaokqjar.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhsnzkhj.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gdakjrvet.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gpovtpxmh.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gttfxcjdm.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gxxvrqizs.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gyhbijqpc.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gupzupcml.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gcqqubauf.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gabotahhe.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gljokjcrb.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gvkxwpuuy.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/ghplylkua.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gmzkhwehz.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gpozelvbu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/grcyvwdqf.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gfoztqfwc.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gdzekfxsx.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gvtydybxc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gmadnqvrm.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gnpevnmgk.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/glmlgazjg.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gbsaqxtry.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/glviztuxm.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gzpixvewr.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gmbruzwog.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/ggjhsonic.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/ggnnolxke.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/glppsqfzv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gqkebhmhf.sHtML


<!-- 参考信息 -->