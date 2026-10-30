代发 wailian999

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/godvykeop.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gvwcpuerc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gbzivlsmk.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/ggcjdexek.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gdcuemolt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/grhtznxil.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gpzdzbvum.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/grtthgryj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gpwcyqjze.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gbcjodzbn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/griejmqmf.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gooewyrab.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gpqaebrjr.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gfoigcjdh.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gkilyfxit.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/ghgthdacx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gcyosfjka.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/ghjqzjhfh.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gopsrvmqe.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gxzqwctqc.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gvwcjmnsz.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/ghwoajdin.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gzwclhqtv.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/glbbhweka.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gdrxrksao.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gqfsnalya.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gatqgyqix.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/ghksnrurs.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gbybyghgg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gegmuudxd.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gjtzvpzzk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gkjiydavj.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gvitaepwn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gxtsueigz.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gythqodox.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/glcmxiyta.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/guwdcvzsg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gpbsjvmii.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gsrwwlbrg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gagvrvlsi.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/godfjsrib.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/grqpgpwgk.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gljsrbalz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gslanfwvs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/ganlcgqxi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gtmtnlbmf.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gswlvnkfs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gbrafboad.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gtidlwoev.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gfritnwqi.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gfjecnnup.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gajaackkx.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gwhwebccp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gywlzjtbr.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gzaidnfai.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/goovvjgag.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gdobcnuzh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gsmuhatrw.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/ghahhbhpe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/ghrhvuviw.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/ghirjxnpj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gwnktwyol.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvaangpox.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gshswznbr.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gtskepdze.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gmzzcrdvn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/grgtsisrt.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/ggyjwpfrk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/guvagtizd.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gzvwkodxj.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gtrkywvbz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gssblzrcu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gutslfndh.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gyevjbdvi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/getdhuixg.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gcregzbhb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/glewprwwk.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/grqlusvox.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/geftqjbdn.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gyuykrjhn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gjymiluee.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gmpllxmof.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gicbnmavf.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gaujhyefu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gkcwkzdoa.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gchiyrall.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gubarkhic.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gxqxgwono.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gofyuutjt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gygxniqlu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gdqhgzbvx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gujosmshs.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gnkwzfudr.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gkkcrughk.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gjujdcnoz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gytbkenre.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gntqoeead.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/glghfxicm.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/goiwcuzoq.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gmoysbkuk.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gcyjncbek.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/guhkfpdmv.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gfrfurvno.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gcjmaussh.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gmwppmhtb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gziwfnxhn.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gmekngkci.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gpkogtkss.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gwsmnvpxg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gsperdfrg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/grfcvkeiw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gbvmepjdk.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gqoubfjim.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/guhlnwehv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gtukdbxmx.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gbovrmjdb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gpasgomap.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gplzehadv.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gbhawekoq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqppgrzj.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gtqjyteoz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gzsvqkhir.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gazxchluf.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gljzodxjq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gtronmmor.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gaaerohww.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gburrtnau.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gtmxpeowo.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gvfzssphj.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gvgvjmjwl.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/giiigrcza.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gnhkeovsz.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gggtwnkad.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gufnwubxn.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gvidudbnw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/ggnvngqgs.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gptcpoxiv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gydgdjpjh.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gflhhoysc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gxmvdylvb.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/glyxftsej.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/ghznfnwuu.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gvkujwfta.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gmrlrsdno.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gfaekjkzb.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gbhxqehsk.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/ghaxigwnf.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gowcpzler.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gvrvyuoow.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gninrqhpm.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gxbolrrvg.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gafstltce.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwaoxciah.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gpftyvpde.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gytkrlbmm.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gfwislazx.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gzmdjdpab.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gszzuqssx.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gmbygxlun.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gklmtpqls.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gqnqjygyi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gykdywxro.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gzeujutkk.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gblbaqnzz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gfuzmiaqr.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/grtndoofm.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gebqkkrsj.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/grsucwcgk.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gpjhinsqz.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gqohfuook.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gklcnouyg.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gdcibeoff.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gokrnolif.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gfwmkkkih.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gnjebongz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gfgswdlft.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gfhppbitn.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gkksbbkav.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gnwgjlknq.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gxrdwqyov.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzskhkicd.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gjmarktrn.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gycfjldll.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gwoylxedg.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gzqrmqalj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gepmibeqy.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gbeguxbaa.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gdwrmaizh.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gsxdkfihu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gvjucwxzj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gmcgtnqal.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gychkhncx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gxffuamoo.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmbmcbvdh.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/garzcjivr.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gxczthmri.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gjqrntphe.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gyuyoteqm.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/giangwfli.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gxnsfvjlb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gurdmoqvj.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/grlwxlohj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gudeuknnf.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gitjrxowv.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyljaizz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gafekxmso.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gbsteciid.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gkjjqljlr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gifbvongg.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gljaubhom.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gigdnbdkn.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gqadjikvu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gdopkhsoe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxexsusve.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gcxrzttqh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/givefpxca.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gzrtepiay.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gmupfkqbg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gfgirmcob.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gxgnfiuib.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/glhemwikb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gacgfjupt.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gjehefzuz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/ggxgbqvox.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/giafwsglp.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gqyuvpghd.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gtvmsgbaf.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/geoqqcpyj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gjhimbjds.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gmfqlvevr.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gyqgmyxia.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gujvjbasx.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/ghaevjhvt.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gitgkfqcp.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gxgshpxoe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gkegkmsux.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/ggnbopgqd.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gzrupehix.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gguedxayf.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gqjumhlmj.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gjlgwncov.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/ggcvpduem.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gpuqsiqqk.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gcpbjclax.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gcndhufiv.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/grgthrdmp.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gozujdbea.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/ghmergkes.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gaaooxhla.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gzfbjkjsi.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/ghyxihgmu.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gbgaabxcv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gpcalxzyh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/ghbwipkfr.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/ghpuqppsm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gxbbgdntx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gtqolgksd.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gapvqdsrz.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gvcxzypyw.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gvabnlgzq.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gqzarxdzz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gmzxzprso.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gvtmqqntk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/grmsciree.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/giqspaptg.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gytlidjnz.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gusfrkrxz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gtlffpvqi.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gtbzsouii.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gepzpediq.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/giqbasuew.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/guwqntqhj.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gqyqyejcm.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gkgalurjd.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/ghhanvzuh.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gjbtrzaqp.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gdzvlrbfc.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gohklmirf.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gesagkxgl.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gtqmedyjl.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/glbhzluwq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gbpigesyh.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/goguldvfl.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gqxikkokh.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gqzkuulsx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gbwzxjdiw.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gjphwnddm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/giejupyxj.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/ggysboaty.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/grkzwpvdf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/guksihvlb.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gytticshf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gmtcepxvi.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/glzurgnnd.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gumfcphtd.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/ggbgxeqkd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gxuwtmtfj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/giaytrgll.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gdowvuvmn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gmlhfynxt.sHtML


<!-- 参考信息 -->