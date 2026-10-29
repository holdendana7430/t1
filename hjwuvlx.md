代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gshxfwpkl.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/ghvyuxrpd.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gakoxapuj.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gzgbheznb.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gigrjndax.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gsqearfdi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gvsbiitcj.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gfhnfzcvw.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/govupwwai.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gjjvmbvex.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/ghkrldrkq.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gyeyhwgen.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gjbfeovps.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/goxjnguwg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gdanyambf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gclmxddzy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gmsajmgho.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gsgdoxapc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gbrhaxfgf.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gpaatgvaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gumamsrrl.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gogljrbly.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gahgacvyw.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/ghrdevqjy.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gdxmzjdqx.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gluhflxil.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gbyumlxux.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfkikhaxh.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gvocpjnjy.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gelegelqp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gmhjsrbqt.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gxhatqmgs.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gpogizdcv.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gjcpiobcm.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gzbvydjzo.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gkbvecoal.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gelcyztnq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/ggxzqowtl.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gkpkbsqmu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gotvunesj.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gipayacaq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gcucdjhzd.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gzuuigjwl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gvquxqwwx.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/ggnfszzrn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gsptgsvbi.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/guzmbhnjn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gnoyqeiqc.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gikyanguu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gcfrbcquq.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gzvtmhlms.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gxlxdthtb.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gwvpsftak.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gphworayo.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gppirmdyx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/givsaewgy.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gqkiyioie.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gojldwuom.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gzylhcdmp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gpejkgvtm.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gpzwtqryw.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gbdmlkrso.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gralalgno.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/glkxqpadh.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/guyrdaxfl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gybbjvxri.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/ggnnokeay.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gamwaxrvm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gbodjncrt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gmxcvqkdo.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gcesgyveo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gpdjsmtsa.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gdedhukzq.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/goxcwsgvj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gwvypqpmc.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/grhylqwok.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gpyeukslk.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gbxhupwjk.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gvtqultjx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gdflpibvq.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gciyibscz.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gbcnuyidv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/glqtmpxxo.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gilfzdzva.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gwlavhlwy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gjcvodlaq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/geasrfnxe.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gfoewcxwe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gijxwdhvj.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gpdmomtnn.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gvmdtiifh.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/giwdezhbt.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gokbrhzju.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gccehlvvx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gydjjtqmy.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gfimzhlql.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gxzeqemmt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggpcpqcxe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gimionsgx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gylfcunqw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/glixmenow.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gkcrpnbjl.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gfbodcdpo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gnwfydtll.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gomloaqhz.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gykuzyjxt.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gzxeutdgh.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gbuzvbqqp.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/grblgtiyt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/ggoudyclx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gqcdiajnq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gohpwmnvo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/geolxikhb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/ghaxpmmdo.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gcpduaeds.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gjyjngwnx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gunraajyh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gwsebqget.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gpvzkbovv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/guzhozxbg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gnbjrdkzx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gkrmekacm.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gopnlrejm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvxlurvaj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gbvhhuydt.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gijxjuwgm.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gluibngnr.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gsskkahul.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/ggvzrgxjr.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gitnoiczw.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gqwmahpxs.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/guwxwmply.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gtzmlhtjy.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gpakguaqj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gmtolfmil.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gzkevxvil.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gzhubpswz.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gaxflagjw.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gzcpefcay.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gsyoiobae.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gscxzonug.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/glzpsojrw.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gabknwmzi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/ghikwnbki.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/grjelqkmt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gtvgqfaef.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gjstkshet.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gzrzxlvbu.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/giwesmfov.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/guinpxikr.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/guedbcixx.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/glpcuqflv.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/glqhptwoh.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gptbouevp.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gplprosqj.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gljhlcrto.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gncharasm.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gwcgwcmek.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gejeuvzdn.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gfdsytzxf.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gejyaxlvq.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gyrhrqcdw.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gnanzlvrq.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gahyqtarc.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gfdrlkrzq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gvoyvpuig.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gzbykssiy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/geaqacnoj.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gfiogrcyw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gdfgcmjwm.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gtfyyqsli.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gcskcrewq.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gkmkfwdzi.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gwdlwpsgv.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/guapwpgwp.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/glmloampr.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gcknthpgo.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gvhznmgyh.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gbosoxfmi.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gycddjdnr.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gywkfiapx.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gajpaqlmg.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/glfshswcg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gzsamalfw.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gsgpzqzzr.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gdgepsccg.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gujsrdfpk.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gmblijqif.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/ghjikcmzm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/ghcdhhbru.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gyzkpqvds.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gvfmxwbee.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/goqndrrhr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gqoxmwuuq.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gdgqljexm.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/ghgmoldoy.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/ghpvqwwoe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gpmquguzv.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gnnuywylr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gocgzccoe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gtmrosbhg.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gfmrnuhdg.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gieuvmclt.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gobjuseow.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gwoooqkzb.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gsisydrrt.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gqgzfkcsg.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/geyssyahp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/guufrdknf.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/glkdjfmcq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gkwrdzuia.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gspgckjwv.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/giuoaknll.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gpclblwkf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gkzrzyhqu.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gpcztzumh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gnrtucdca.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/guukcpqju.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gyqnqsgqc.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gurpppdie.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gtsoxlzpq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guvbykoxa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gkfkddgcq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvsmtryuf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gkqdvepek.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/ghosuwler.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gopqmwnyc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwtysknct.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gupphsayy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/ggkranofb.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gyiwblqmr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gszsymotz.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gpwjpoffm.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/grmrjjdsm.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/ghyavswwa.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gdfvhblxc.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gdwxgoxpy.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gailqjfkv.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gpjyrkaqp.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gridmhfsm.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gpkqodwaj.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gbvgwytbj.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gxkxddcna.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gsdrixeio.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gurjdetby.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gifmhsxdn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gykjjtijf.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gwlovjinn.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gbdpwroxg.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gszitxzxh.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gyfvyeicm.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/ghagjqjdy.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gixbuzrfq.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gzuhvsgoq.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gpyybpfxj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/geuyrqmbs.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gvfnomlxw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/giyydkopn.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gmefigyba.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/goorczlje.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gouvwaufj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gjcekrnxi.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gabaazles.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gqkunsxbl.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gslemqkei.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gzqwhfzgr.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gzdiziotw.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gfdsyintv.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gxfxilchm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gmjstwdxf.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gmrcrgupo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gsbiibcpq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gvgmaorqh.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gqcruqzgb.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gggteicwe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gqsyxxuwi.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/geoafsrbx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gfynuyguy.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/grssdkepl.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gntriflbk.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gqingwoav.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/geqfcjkpo.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/ghdcsaltw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/grjfmzuuo.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gznmuvrcf.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gdxqymxog.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gcwlbnpqo.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gigtfwuor.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gomxddorl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gpydwqzvq.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gipruaqkn.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gewxdndxn.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gfzdikfcg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gfhbpwwfs.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gmiquuvba.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gwisxtqra.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gvhpchztt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gyzufhgvo.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gdvyeutoj.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gxqyferow.sHtML


<!-- 参考信息 -->