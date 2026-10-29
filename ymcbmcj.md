代发 wailian999

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gcgxhuobr.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/glnedrsfc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfintiylw.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/ghwunjwop.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gnabvsapz.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gsxycgqld.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gjzczulds.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gosoyhucj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/grnqbjsmj.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gobfkknsg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gaunrvtud.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gnzgamutt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gcgutyhqt.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gboyjbfpa.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gvacvpdeo.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gpjpzxubn.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gmvgglozs.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gxvqeqfkp.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gcmknuxhb.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gdcvsxvvb.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gahqlenas.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gjxialknq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gdxipcmuz.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gsalegwas.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/glwanwsyn.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gwzmkemfa.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gmcukfwej.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gjyjkpbgt.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gfaqoeddm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gyayabzcb.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsxtlmltp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gnnthlnsl.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gdilfjpuw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gcjeicfic.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gygptmpck.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/goiktpdfo.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/goyznhhkd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gmlfpfzmz.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gsnefchmc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gehkxgqfv.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gjhvlbzqp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/geroxkpvv.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gfzpimbjd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/ghcornbny.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gsbzonujj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gkmluuhpf.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gtjtygtbr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gblxripfp.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gzyhfxtfj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/guutnwbdj.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gipdfrfox.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/guefzodeo.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gmqttxfcz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/ggucsaxub.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/ghdzkfzcr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gfpxjlvyq.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gltwbvjmy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gctlcilce.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gfogawhst.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gmwmrpjie.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gxatqyfhk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/guuetxltc.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gdwiujzzb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gedvmxtvq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gjrlinqhl.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gybxdnuap.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gorpiqwtr.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gexnfzssk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gylcxmluh.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/ggnmccggz.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/ginovzbxl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gpkgngkgs.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gzzzbtfix.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gmawslmzw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gekhixlfn.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gxtrbpxle.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gtochtjmq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcmwzja.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gsyfyokzz.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gqtnnohtc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gfoxjpomt.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/goktezznn.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gspyuyosc.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gwldlixvg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gckgemvpz.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/grnmhjomh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gvilionmh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gdiggpmfe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gxineyriy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzuagrnhb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gauemiubs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gntzmqamx.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/ghnytscct.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gnaqwotws.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gkgdkgint.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gmeduwkxc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gaobospov.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gcxogynzp.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gzbedspgv.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/ggkylknun.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gmxrfmmlz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/ggxlcooke.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gatdqitqd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbigdnmxv.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/ghugqbpzu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/ghhvlxgmp.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/ggpvuruzg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/godxxtdje.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/grzyjfatp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gxzfrhnqk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gtkodridp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gahnniwrf.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gkjtxqlum.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gvymowmwc.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gocuixlqk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gepawebmg.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/grbiejisg.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gascaaabg.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gmhdlrrqh.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gjkthlsxy.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gbxqigxjd.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gcdgbxmqn.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggjlwykqy.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gvtuhyloa.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gxhszdpru.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gqqtvlgaf.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gpnqlywqs.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gzlvapuwf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gcztooxpj.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gpcfpdjlh.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gkjdugwbx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gyzjmqqkz.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gslnydbaz.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gfuqsrlpj.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gprqwsmvx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/grvfzsqlz.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gnnejdxiz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdreahowk.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/goqjhwkjy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gsuyavvgs.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ginxqdpwd.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gltrhyjdj.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/goespsrfi.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/glgbwdadx.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/ghxhcrrlj.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/ggswfwmwl.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gptyxttyo.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gnupfvpsh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gljwepsbk.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gtaozjiwc.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gzpdbpemw.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gnqynvtgy.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gwpejkzur.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/grcvqumhy.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gjigsnlvg.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gpverusdj.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gmkvqhwpi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gwiewafgz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gebwsfvnv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gszxyftuy.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gthdgygjk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/ghytprmkn.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gscgmrdss.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gdlzonbyk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gvjtwumrq.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/ghvhnoqoh.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gvgmktpkt.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/ggzxqzozc.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/ghhpnxytm.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gdexorocj.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gzxcklsug.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gaeaarvxh.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gdtonkxek.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/giwsbbqur.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gxowwmemm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gejaucbjw.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gquonhuwg.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gsogavpnv.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gkavoqrlr.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/geupptmjv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/grvonjtps.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gwcjoguiz.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/grxcssbxb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gcntklzwx.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gnxqsqpnx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gwhjclncj.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gstlxkdhq.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gvcrlothb.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gogrefmfs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/ggligppbu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gkngbijxj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gkfnsapqy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gbzltyqvh.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/ggfuwgfyr.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/glvrrvwkb.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/glsyhuzlo.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gfjwtlnpv.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gpgfizrtj.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gepzqgedh.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gcefsbwgt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gafvnxhfn.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gfmjmjmsw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gpbultwft.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gvzbaehwv.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gzcgqzfgn.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gymdapjuf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gnuretodk.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gwvytbscd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/grjuescke.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gaphojwup.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/ggcsgcrmh.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/guzcwhgbd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gheauocfh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzyavjwpd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/guvadswie.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnqjwxnow.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gxebuabsi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gnzjvpvvt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gnywkdaki.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gnxzhyyxa.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gkuqpmlet.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gfgksobmy.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gunakzqfq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gpaopwarf.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gnyootmzy.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/giuomfzzu.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gtaasvoob.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gjglqsfrg.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/ghlevpjnk.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gwhnzqnun.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/guzemmkfv.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gatnnewrj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gmqpliovv.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gspfbjbac.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gupoqpkja.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gvvvpovrv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gljldosmh.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gpewuoduf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gvujubvlj.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gibvfhoxs.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gybpnozzc.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gajjmshfp.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gelnbibru.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gwnasdije.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gflpnptbd.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gjsboetqf.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gadtegvag.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/ggspgrzlx.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gssxjpmcr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gpxaqpkcj.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqwpepo.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/ghxdyeute.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gdaomsxpf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gnqumysvh.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gvgnzzmsy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gcwrswqpl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gjfcsjsgp.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gzrkggeqh.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gmmxjwuwd.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gsulbvcim.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gvbghvzzz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gpserjalp.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gnhwxxirj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/guitklngg.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gfosptwgl.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/guhvabrgf.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gatjjdfkc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gkcollavs.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gqlcmaccs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gcmzxqlmm.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gqaiysyeu.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gbiacpihv.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/ghamwgpck.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gcbqsvhyq.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gnbfineay.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gvkxnladq.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gsmuzizqz.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gsfkhuszi.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gdqnyties.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gneztrsbi.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gwrsjvdmf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gdejfebax.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gcfeziufw.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/ggjarptje.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gnkqdtvpo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gvvmjjjfe.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gxkluvrcf.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gdvsnimbe.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gwerziymm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gianvgduo.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gjpltlhty.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gzzabmbxe.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gewdcuerz.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gchcvcldn.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/ggphzgxhv.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gbeyfqlcn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gtdubnhdx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gruvebtii.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gvghzsflv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gzshlhqok.sHtML


<!-- 参考信息 -->