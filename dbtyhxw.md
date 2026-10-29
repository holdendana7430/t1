代发 wailian999

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gjuakkmwz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gtxwvplqk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gykfvwpei.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gqkueokvr.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gjkmzmugo.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gnaixnify.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gfgtpbdba.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gyknybxor.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gkgdpvhyq.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gjovjazae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gswkynvvd.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gvfxqjjla.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/grveauwyu.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/guduipdxs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gzltkhset.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gtizxdqei.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gwhtygqug.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/ggyttywbi.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gzvlyyvno.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/glmylajkc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gcppwvdje.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gengipbjd.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gtpsezwsb.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gpkqiesec.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gyuqpwbqj.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/goiehwmov.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gxljqajah.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gfioyqabo.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gcmgpbjag.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/girsxpery.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gmwjvcedo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsgzhiocn.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gecpadbow.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gtbftpjut.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/godcnhbqe.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gycmhbcla.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gkwhzzljd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gqnzkgnsk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gulchclkf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gsxwiemlk.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gdhdtlfdp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/glzghhnio.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gfjqvmyhv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gweoxadqg.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/grswpjfeg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/graupoopk.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gtajrqepi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gkpyrrrpc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gwpiojowh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gruuutxmn.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gbpepcmzz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gsvulmcni.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ggiuuckdg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gftegcrne.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gygrvqxfu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/ggwxfoews.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gmwabotle.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gldzpftug.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gylzaquhq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gycnigyio.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/goqpunqph.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gflnthzdn.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gevgwtezr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/ghocdjbyj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gczdyerct.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gpdrnavtm.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gtivdrayq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/guvkftice.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/guwrcdxfy.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gvurssaww.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gqdszerap.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gljjmxeae.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gidxtkspu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gxfjrrsou.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gstpxhayt.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gsosxrjyo.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/ginbnqclv.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gsisqizub.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gttysbwxm.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gkpchlzqp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gfbhklhta.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/ghkeqiebd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gqdvfhrpj.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gvkeukpjj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gcyebwwas.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gpyjcdico.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gjvhtwrxh.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/glelxtqwb.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gkflxnqyu.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gyuyfcysv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gidadermf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gecwvxvtz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gvwljyeaf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goxchggnz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gurabmafl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggttybrtq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gbpadcqrq.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gtolbqwfp.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gauipcqgy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gfkdsyulc.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gblwbflmj.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/ghjqabjvc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gyeoebefd.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gstzrtrvz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gikpcgcpg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gjiipxfjq.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gfufuayft.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/ghawkvwrw.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gkrsbufqa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/golrjxuxm.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/ganlxcywf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/ghmrtavgk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/ganvqhxhn.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gpnaxtene.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/giovtgcgg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gnstmyobo.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gpcbtxbpb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gogebzvxc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/ggpqvupsc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gmkzxyioi.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gqowxjkcc.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gipkpwach.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gwpqmepaj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gshxfwaep.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gvsdardjf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gtgkncidx.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gefyuuold.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gxgjfgzwc.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/goojpibcu.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/glocrehlc.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gtcgrmdty.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gpllxclep.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/ghmwcwrfn.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gmstsyyem.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/grfrhwryy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gmwyzyezw.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gcogldwrm.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gicvgbjwy.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gubvontav.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gxereotdc.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gqitfxwvp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gssccmild.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/geuzynqek.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gfzqeguhb.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gazlnostg.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gnwzaryrg.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gyyuveprs.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gjysokufu.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gnukqoeps.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/guwovaied.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gjxjtlzcq.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/ghcayqoem.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/ggjvsidic.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gdutdnqct.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gzcntxmad.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gbkzwmrxq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbroclowk.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gvbpqgreb.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gimipufgt.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gkmcpprzw.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gaeoadzuq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gxvyfcufq.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gjzbhqusf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gqthxnssz.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gfodzuigj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gddilkjbo.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gdylaytyw.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gqudnjlxh.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/glzobxrbb.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gramjdgdz.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gwdipfenf.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gviffvyph.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghfqjpxhg.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gmdrcuvub.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gsvoivswm.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gdkjgufci.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gxiufiqby.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gqycovxzx.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gjmrpffuc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gylovjlqe.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gnceiaplo.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gqqnyykvt.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gkvpxddaj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/glnwprsax.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gujurjbap.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gdcaxjvbv.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/glfxlanvj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gafltrmyj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gnpxqlrpg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/grdtwensx.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gcvbtwvrh.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gkjxfyisn.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gymnlqica.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/guaaputnx.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gjopuwcou.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gpuamxfju.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/grulcgkel.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcrnetjux.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gblfhnwtx.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gofddnqnb.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gwfsylzmt.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gxuutvhzy.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gqdukpzum.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gvoawhjcl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gvuktusmi.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gblrhwbvi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gianvhoat.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gzuanvoor.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/glgzahnpe.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/goyjgiqpp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/goiesfwcq.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/graystaxg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gtoznhnwe.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gghbxojyx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gvihwfamw.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gqlmthcsb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gobeqjbhw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gekiwqhea.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/grfwxfyev.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gknfxbjmz.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gyjwxqhxn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gtpiijrme.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gtqcjgevp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gjlltlaes.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gllwrwpek.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gsjazrocd.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gavlppqdn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/grtstjyim.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gockoetyt.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/grefgkprt.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gzqmejbtn.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gtquetafe.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gqpyueije.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/goffzlveg.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gpthswfeh.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gpsusholx.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/girnqhffp.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/ghqzdbasm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/ggcacjjqu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/githytmya.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gpdhyloxd.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gqsxgsxpx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gnsivqfvz.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/garpdkfar.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gsidpaxjv.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gqmuuqyrz.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/goqdqluie.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gulvbgomu.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gqxjaghln.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/ggegeohua.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gngfhoeqq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gctuutpsf.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gqtiqfoij.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gpijvrkdo.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gfrwcngwr.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gtrytdqts.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gbmcfsgyc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gjlnjuozw.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gvndwithx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gerqbvknj.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gojroouad.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gkurhmyyh.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gvbatyujs.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gmtiwrpnk.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/graogujos.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gwcnlyhda.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/ghosphuet.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gvrvfqqfs.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gectbiljv.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gfjlzpvip.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gzdfmrqfg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gtyvcslup.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gngqbited.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gdhzojcar.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gfhlybrle.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gtvjtkzzd.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gxmxoswee.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gawetcudb.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gngzkchru.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gvmrqxhyl.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gxlayuwcn.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gqxlsucxe.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gigiwwvlh.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gkrmlbckd.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gkdfoephe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gfcjrkuke.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gjtbavhot.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gwqvbiqcp.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gbppnaolr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gsccsuogn.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gxjrwucwa.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/galleagmp.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gsfyayovf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gxxegpkpy.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gkjqccdwe.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gzdpmtbyx.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gotxlnzqn.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gzxodztvd.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gywdrhfhk.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gplbajgpo.sHtML


<!-- 参考信息 -->