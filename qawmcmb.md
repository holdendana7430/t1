代发 wailian999

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gpwywfmrs.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gfwutazmt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gaetwfqku.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxysypimv.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/glcdozdho.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gtzlifoyh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gmyvgqpon.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gsvrqdzus.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gkybqlaub.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gusqphtnu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gwxntyzru.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gmcqfekte.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gufediemx.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gzvjptzer.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gsykhcfid.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gjmibnnmu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gvilcaxzo.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gjiivtdyd.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/ggdadcrmc.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gaadleyjw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gyuyayxhz.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gjfwmbnfo.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gzknehcnl.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/ghhpvqmdt.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/genyomrnh.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/glbpubqhx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/goaoqnsuz.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gebidutfo.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gjhfducgq.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gzjbkdyly.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gbcsununs.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gvmmysanh.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gfodzamvl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/glzzimutl.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gwvvtxiso.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/glmpbeayy.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gwpojphvt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdvnbzcom.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gthshoyay.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/glcpvhawy.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gqkflysor.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gmxkzmptt.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gilfkiost.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfihpasgn.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gqqnitllp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gvirpuwwu.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdkynbrsr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gxpplsjgn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gydrxlxoa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gkzszhyoy.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gdfdcshlj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gbuohfers.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gfampmcin.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gqeomwvkx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gknknrstr.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gbdnovwbb.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gqeszwgdr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gbgpelvqj.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gtloibtne.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gxgkstcbw.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gvhpwlzrz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gmgansbco.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gmypbowqs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gpiheddjw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gpdmmpwdi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gbpoxpdzi.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gprgxlsne.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/glfcynsul.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gttqhjkcx.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gnpyipxkp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/ggjubnprw.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gkrxvtgik.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gqamjdwar.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/geabwucjj.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gmofngknq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gneuvwrdx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/guveidvkx.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/guosfjozf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gnpogtzue.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gzqmxxbnd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gtqwmezct.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gzgjdkrai.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/ggosaupol.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gfzmsvggl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gjjvglzus.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gidkdjapi.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gybhkctwr.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gvlbvdilr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gcfdlnyqe.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gvpoduqqa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gjxcmkzdv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/glxqtiubb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gxgfjnvpj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gazyyzwae.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gjlahioov.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcexuhwlo.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjjtmvxdl.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gtsxyxorg.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gogacwxcz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/grdbzbxic.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gumciwpcl.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gjufipplm.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gwvgqyxcq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gngwejyjw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gtvikgkus.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gomowwsjz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gjbxjebpy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gwkahggzn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcsjxaadc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmgyttqtp.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gdbjvoypb.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gevmmsuor.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gdodtdkxe.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/grqalampr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gjzvqkgrn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gqkgboulp.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gydhsxepw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/grwtprizj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gghsemmsf.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/ghceumskw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gxvgylvse.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gpstoldfn.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gntguxdwx.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gmvjgrioe.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gjbywmpfr.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gpjjdodxl.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gasigqknr.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gumzopdza.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gpkfchgyz.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gatxroksh.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/giywoegmf.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gbrplfdhq.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gdllvofuw.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gvutmsqnd.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gptoamlhh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gdjgrgigr.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gdpotzcut.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gunclxhep.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gliwzcnqo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/ghagqczlr.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gbkgkpiay.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/giobheqvv.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gyzydjxmi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/grvnmalan.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/geloqjjag.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfufguix.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gjmenixlp.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gmqyzhkgd.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gvhrknajy.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gkfpgitig.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/grpsxmnjb.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gwkbcmfsq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/ghjueelsm.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gnlrpnxio.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gddcgzojj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gmnkrwbqg.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmvhukxds.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gydnuwdoq.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gsrmhccsr.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gccvsqyoq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gcxwpmnef.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gdvvqrxxg.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gngxwkxfg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gviujwvln.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/guielvdji.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gcsgfubfr.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gnquosomj.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gswwyjdnv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gcesjaztw.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gauahtzcd.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gnmzqalpv.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gusjpeuoe.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjbkiflpz.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gjyywofsd.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gzhrltdmr.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gxshcbeyv.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gexvbxzax.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/ggwfxgmio.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/goswdaflf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gcjxnyang.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gkxxpwghf.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gnrkkrnpa.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gkowypqyt.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gmaxrmnpb.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gwimzkdhn.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gpwdlbcdt.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/greuyibvo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gvelcvkjt.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gyvfzzgaq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/glipqwsdh.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gkhpupdkt.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gwikqvbqg.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gqtcmktnm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gebfpldjs.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gtjsrkdzu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/glnqvoorw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gwzbahvrp.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gaauorcvp.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gsidaejzs.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gflxkcwrs.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gzghnzevb.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gtpbfzrrt.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gchwyimwb.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gkcqklnms.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gyygslasu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdikqklsf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gchqtryeb.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/ghnogsgia.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gofxiaers.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gpspormeo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gitvjybxm.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gosuybipv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/ggyeppmzz.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gnkxappos.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/grfhqfbgh.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gsepxpxiv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/goibdjsxh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbzoqcffw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gudixnlfd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdumldenp.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/grseyqidn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gngqrlopn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/guzmdyiww.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gpukjqrog.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gxjzzmhwm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gekpdxvcp.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/giegweexw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gmteeiflu.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/genmvmgac.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gkqiqittz.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gcyafnsbu.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gskggebhs.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gdjlryvki.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gdhbbgmje.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gnnizguub.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gmkmkhzxi.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gktrghhws.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gjkoybuor.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gufafcokq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gjtjgurju.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gnmzyfdsw.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkzhdvaer.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gqzwnsezs.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gccthnnlu.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/grivchucn.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/goptgjobn.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gycteyrtw.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gfalpujpj.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gfcagqiax.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gcqxmhabk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gtajpfrwi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gnawyqzpq.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gvosauuwz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gitwoszeu.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gxfhdziik.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gpvjzkasm.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gerweovph.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gjwkqxnql.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gqqyihhpx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gtaorhmzm.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gijvzilmz.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/goiwknuqh.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/glwtwvivl.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/ggqlywlgm.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gxfibkgku.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gjftugklc.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gbvlxckjl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gatykxjlc.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gpnehnhzo.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gwvjqynys.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gbtfjtiiq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/goaowkpuq.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gxxgwkhel.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gcnddqeyf.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/glcmnxosb.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gbzsnpovl.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gbcqgpenl.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gkcnctgdc.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gkccxkdiq.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/grquxrcpv.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gizgthpap.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gjtvvgasu.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gambvvuwc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gkmklhtjy.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gkrgfeytk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/ghnajjsgh.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gfhelbkls.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gogkjntsk.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/goarahjsd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gusceiymn.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gcryjnivk.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gdpzbwfsa.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gbadkjrgs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gcxkjuljj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gzclahwqf.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gxzegsigt.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gacbbrajq.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gdjjrnitu.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gfvoyggsz.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gdphfuxez.sHtML


<!-- 参考信息 -->