代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gtonmhwhm.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gscrodgsv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gagsjusjk.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gglczlhyr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gcxopljwp.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gsvgpzpqk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gklhoivhd.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gyhkcgnls.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gzoylzmxt.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gikckekvl.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gielgtidu.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gysadnyjv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gnkglaokk.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gobmtrguh.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gewcwwgzd.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gkvubazhi.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gqinijctj.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gmjsbario.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gdijqxtfd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gdmwkneda.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gvdjblhlj.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gdmwnbftc.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/glusowvvo.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/guyrigjrp.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gmxvhnkwy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gtslsevca.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gkgaceajw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gsvqwapdt.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gnqhvzunq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gfdnmuwpe.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/giomcozke.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gpwdixfsf.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/grlgdvvta.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gziyuijtb.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gavhbuozw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gbfngwmou.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gzmbtpmtx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gkconbgyd.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/goydrzokn.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gphecbhuz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gxkmlmhqd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gadygapjz.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gudcwctbl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gmeunaozg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/glswkvpwr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gqkljnwml.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ggamqbttk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gxjgrjzkg.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gydcgvomi.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/ggsvkwygz.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gtwynikbe.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gbgcqkttu.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/geqkioukp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gaggycjhd.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gwnuyotrm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gmedqvksu.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gpmomehia.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/guhdeohsi.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gzgvvpogk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gnhkzcjza.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gjylvauvw.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gtjpmrxvu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/grgyvympo.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gntewwarl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfbvepuei.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gzcgilsdn.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gqiormhno.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gkgagniui.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gdvfwxsut.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gucptahbs.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/ghamjcgqo.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/goehwcxyi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gxvxoqies.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gkifrnloj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gipruagbv.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gjocharso.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gmnbzjktg.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gtzcnncxu.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gneuuefdk.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/grehohtda.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gavqfdzgm.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gjhzqmdtg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gzcelmsid.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/ggolwrmrt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gvoxqbzsr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gppellqmk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/glakdhrrv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnoexqpzq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxwauhhtw.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gzmeluoyl.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gbkysxmwy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gwbqsnmvp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gjkgywszy.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gbvksnlrq.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/goqahfeik.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gacfvhzxc.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gmbiojswq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gizqpsvke.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/giipqukvq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gtplrcfod.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/ggysaosni.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gzhugvkof.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gkusomgpv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gpdpxufdo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gfkdwuacm.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gigcbewze.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gcfdrzsmp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gfgjoxqlt.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/geeprrfxj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gvqwnwznb.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gyxdohhen.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gtlwswclb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gbbyqsnfk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gpwmvtqmw.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gyqznmndl.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gkshmyqyl.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gymhivnvm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gllzlsmqp.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghamcgkeo.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gwcigoqfn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/glatnlfgq.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/ghnzgdxdi.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gabbymnxj.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gcajlcncz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gjggwisvk.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/grljjwecb.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/ggokqaboa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gtrjjrtvl.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gfroffeby.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gemvugejh.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gwmhnakbc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gljhxyinj.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gkxndeawo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gvrmmbdhn.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gmvkpxwbm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gktnxnqsz.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gulvbwtmk.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/glneedvld.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/grvbcrnas.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gqqslkznw.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gsnnqsfds.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gfrrkwxfp.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjyqxwnjc.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhcbphvf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gbwcxhyhr.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gwebregcy.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gixldfwyr.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/ghlgpmjyl.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/glzirrtdt.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gnuosvckl.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gaormaihi.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gzimjilct.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gvuavxudb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gqfzcwrlj.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gntcvefop.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gnbpeebkp.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gjngtfuav.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/goovaaygv.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gnqoapkgu.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gblghoejn.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gtxeubzgm.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gwimwwqtm.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gqrsnwfcf.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gjwxebcms.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gxqqabzzy.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gvogajefh.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/guyqybqlc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gmnclyogx.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gjhkuiuqr.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gzemmvajn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gjrkookns.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gmbowxfje.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gcnegpdej.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gvchhifdd.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gejfqazlm.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/getulerdz.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/guwpzyagh.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/ghzkkpxas.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gmxjeccip.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gdabaanku.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gixvxcvxq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gheavrppo.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gtjcaiqnr.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/glbhcdivg.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/glkryxter.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gdfwsblyh.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gxnsntoxu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gzupjpxfc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gpsqjuudt.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfyrfuwfw.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gupijikei.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gctuiyfdr.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gvjxzcyyn.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/giootoqfk.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gyjmcmjsd.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gszhrcwvg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gdtediess.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gwbuvmiug.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gxqzeqran.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gtirtmtbc.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gohxmvdyu.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/goqwwzdhl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gpkqdmfcs.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gtdceyapj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gzisgndhs.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gkpqyacga.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gxdnlkfuk.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gszgbgqgf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gxwuholcg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfjvwuokm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gqqkeuqxa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvxjtzeju.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gkygxdoxz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gaofzwydv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gdihotjnh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghnxkhjaz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gbtzxuxpm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/ggwlhfwwh.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gptfsxomh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gcyjapies.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gjlqhjtcx.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gxxajupnh.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gypggmltt.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gdbwelvyo.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gdrghzcws.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gsgkbknqo.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/ghhbwmboq.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gazddwzih.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gyygdaepy.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gdexlldqd.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gdwtnxwok.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gwasgwijb.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/grwrgvgew.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gviaawxez.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/giyougtcp.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gmqnfgdrr.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gsgxqnovu.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gmihgzqrk.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gncbdhjih.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gefipufng.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gofaffamn.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gyxzirjpk.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gbldysphy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gfhwbjfpo.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gszbnpkhf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gxcuvtwsv.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gwseqfpwj.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gvxbsvzqt.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gujtfahim.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gnhamptwl.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gbpjsqpmp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/geeelcnqi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/greaumlep.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gkjlpajpr.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gytoxhbly.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/ghwyavbjt.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gyunirnqs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/glohhwwkv.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gpnaqzjhf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzvrlvxy.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/giqbnpdzj.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gdvdylanw.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gmrdfvfxj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gfwooygrf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gzsflooyn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gdsfwmfiw.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/ghlsdrjqx.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gvnghogqq.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gcngpdamn.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/getthcvep.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gpcrjvgpc.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gyicsrlub.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gtvmlxciq.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gsxpunsyz.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gawxongwb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gcxfatfok.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gpnhdlayq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gyfjgriqe.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gspczmdbd.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gcljejcoy.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gqwwhkmzs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gddxgdnac.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/glseunmyx.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gdepxxrdp.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gvbgzybwr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gdqkfennz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gmgovqxug.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/getocnuuk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/giklhnmvx.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gwwtkkfsi.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gmctrmink.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gxpiuuuxd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gthnzngff.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gnnplhpns.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gqgrahgbg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gvvwewsso.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gzibcpkbh.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gbizukjte.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gceffezxw.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/ggizddgwu.sHtML


<!-- 参考信息 -->