代发 wailian999

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gatkifpof.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gldwiqxco.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gfcrkyrum.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gwbskzohm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gblnrlymc.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gbccsnnzt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/ggbhhkjnz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gakbtsbyj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gpxrnkfmy.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/grurgxhtw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/ggteardby.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gtnqzxnpd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gytdtvnhi.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gkalgrmly.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gcnvznunu.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gngifwaon.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/ghyxcvmxn.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/giscprqdx.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gllnswfda.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gkvksikrd.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/guwulrhwx.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gpzqhahhz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gfmafrlgd.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gvystylsl.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gjanjsran.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/ghtkmcrmo.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/grinkwdjb.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdqqgrjkh.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/ghpykczxz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/grbhryqvu.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gcpgvbygd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/ggxlogdlt.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/grstiebrd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/glacdtrwb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gvabgnvem.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/geexclsid.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gqhenlgct.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpfuvkpgq.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gnauddzmx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkuosgguo.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gnxdlivte.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdrvjosa.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gqdoewrgp.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gpkhigixm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/grxxxtvwd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gssxxutuw.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gzmoyfarz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gxfoojpgn.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/grnuulybd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gekosxbsx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gonabkuoo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gzrixndku.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gmldmdjon.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gicnwegph.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/ggizqxoxc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gltmagpch.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gmcjxieou.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/glqgxblnw.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/ggdxfpmuh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gcgqtmutw.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gcxksmtjy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gekofgfea.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gppfnnlmr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/ggrfdyvwa.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gesykqnii.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gupeqthpw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/glwoefdoq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gevmjjsir.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gmwydaemp.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/ghlbyuqsl.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gmmfemcbm.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gifewadcy.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gwhymxgpz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gqkirqakd.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/ghotxxkxs.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gltkpmhzt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gfpvjidne.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gknhryxnz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gthsfakvq.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/grmtgafwv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gapixevrc.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/grocuentc.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gxeirifty.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gkbtfbwbc.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gmyhgsrkt.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gadzftcve.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gdijdiucd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gavxwefkp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/giqonrwhj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyywseefa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gyjrnlpui.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyiphqvkf.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gznwuyact.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gackwvvxo.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gngtlusmh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gothhouxb.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gqamytumk.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/govjlnzqt.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gefcgtpys.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gmepzxwsc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gkvnvvles.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gslprkxpp.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gahssrjje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gkakwuops.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/guqlrqbnb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/grgloggym.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gmuqtlxgw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gexuaqrdr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gjopzvoyc.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gtfszrkjt.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/ggzecssxl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/grtxfyiao.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/grryfjtpg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/groxkefwl.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gsziknczy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gygxlnstz.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gktphjuzg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/glmutrbdh.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gphjxtjln.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gfrtxpprz.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gcbgamnud.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gikkyztbm.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gsaizzlvt.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gcqxayagn.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gzvprquyk.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gwjgewvrr.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ganskwkho.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gymszokme.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gyczncxgw.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gwcihqwww.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gcmmggkya.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gldsywbny.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gvtcisvko.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gwlypttws.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gkztoping.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gpgizoykl.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/goykfxkqm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/guxzfstxt.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gqgyrysvd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gpwytvvmm.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gjdfsqymz.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gafdpwunp.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gsweoiels.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gykoftydj.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/ghepbeham.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqigdkss.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gsdpynlrk.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gjlpoivwr.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gayymcxks.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gkjxhwvxs.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gcguqdpll.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gdqwpdkuj.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gudtjxudw.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/ggkolnqnj.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gebhqioux.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gjprwffms.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gxwlsuvrh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gevlgegja.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gcedkzcsb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/geyqwpouz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gqxtezsmb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gsuzjrgbz.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gxoxrvzvr.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gvjxszxpw.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gyeyqryyz.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/getebqqaj.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gwtwbyxqg.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gnxdowrwr.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmfjcwhsu.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gjwnrzhgz.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gyjhqjiax.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gcolkorne.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxasorbyn.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gfzodjfjt.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gtfdijzxo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gixezmsbf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gdwszmhmt.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gnkjnyzyo.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/geemddhao.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gjltrxlkv.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gwmqfxzkk.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gxonqisct.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/glghbnjfv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gpdlkmncu.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/ghsnkujou.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gxrsiduvk.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gibdnyxmr.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/glqjtdvdy.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmdtflvxo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/ggivyclzb.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gvwmbfewx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gsfnywkpm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gdnzlwdpp.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggauvfzgt.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gwzehkzpt.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gabbweido.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gismdofkr.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/glyxckzwc.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gttjksetq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gfzabgoys.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gmwaywhsi.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvtrwrqjw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/ghpvdgdxo.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/guppqdomg.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/ggtnybzjc.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gblxlivld.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gpjnzvcyl.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gwycoagdh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/ggneardqo.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/goawtkypb.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gydonirsa.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gmjfjgeqp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gynbezjcz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsvfozjxq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/ghikawijg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxtaifidq.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gfayvwzqu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/goejryoxm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gezflrwza.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gbifmjdhf.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/grektpeec.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gmsljrwpl.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gsgknvapu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gmhajlbhv.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gxjiqganz.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/ghwvlfuoa.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/garynlxvn.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gjzulokjd.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gvixlsxop.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/grbixkmuz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gxrrxnvmc.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/ghqfgybwy.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gxbylgadw.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gijtilieh.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gcmsrvnwl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gsyvnvfub.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/guulafucm.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gsnrahzkk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gqwpsthyg.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/ggjadoqob.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gzveujyco.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gmlgbpycx.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/ghaaqjiqq.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/glfhimpak.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gnafyulsv.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gdowrlkmi.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gdmocuaqp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gviybbmfi.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gmhswozfg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gscmaltgr.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gwnapayyk.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gftuufvtb.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gbpazmpza.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/grxyhqwad.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gcjhozcsq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gjrorhxqy.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gkjbccdlu.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/ganwcufhf.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gpledfoob.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gmuznrzus.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gwlueneqf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gpdjngjki.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gvnpdqmhz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gwjmytlkw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gadouiuvc.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gterkpbqc.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gjmxcxlcg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gvygkqnln.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gaypdwkos.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gxzpvhibh.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gytmvjyoj.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gyavqkbsv.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gghjeqaub.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/geobbbgjo.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gswcclzpu.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gqgsghdbk.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/guubkocdn.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gvvxhuzcg.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gcomcoznf.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gjiinkuvh.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gwtbpbaua.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gnktfmtiq.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gpakivved.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gexbvglzq.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/ghtqpqgsq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/grrtporpn.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gituykpof.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gdzkxrdlf.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gtdhhxkka.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gjvhcauca.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gdutrndnh.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gjeczffof.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gopmvkytg.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gmdjkierq.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gepjxgldh.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gcaqvtnnc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/ghmwrdsfj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/ggrfplzcz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/grnkssfih.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/grttxswgu.sHtML


<!-- 参考信息 -->