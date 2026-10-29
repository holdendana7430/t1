代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gcjsflksd.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gthiqycth.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gkhkhxidi.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gfzylvoup.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gfnrsrkxg.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gagkvyerk.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/ggrpywjfb.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gdyjlxjgh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/guitrozqp.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gsonwdygl.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gsucdbzoc.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gqlirgduo.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gmyhytmmo.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gjouxvayx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gzpzubvzb.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gtvgnytez.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gelxxlkjr.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gfiqoybnt.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/ggfuvhhkz.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gyspsybgi.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/giztpmelb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnrnexls.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gcnlxuoxi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gthmuoisk.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gebrkadbd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gzvkwewtm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/ggtnglxai.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gujrycaza.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gzdceiwbv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gjhnewiul.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gxstpbmsu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gsimybwvu.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gtiimohho.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gpafdqddt.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/geegstxgj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gvinopldp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gjveuczxd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gkfvvgvue.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gcuxjqhgy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gwlgcfgvd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gpkvhgytz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/geddgfsym.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gvoffwapp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gvljhpgtn.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gxfpjqeht.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gobrzolfv.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/guhgkncyc.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gdnfmubtg.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gxxqfxtqv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gntceighy.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gyosgirzf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gldrofovr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gaqlfcqji.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gbufyuwfr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gfhryebls.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gryezogbx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/grwyipgmk.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gvryigpoa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gnnzhdxnz.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gqoarjixa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gtqwhpwfn.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gvcuxrpve.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/geqjccyrq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gwkwspkau.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gaykjoacj.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gkhtmqzom.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gzzabqghh.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gxhgzahwo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gjqqcphuq.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gcqcezgmp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gqpufcgoi.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/glgujejmt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gqwggkjfh.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gveytvhkk.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/grzwexayr.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gkfctdtnp.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gslsiyoho.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gyybzshdl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gkgpggnxu.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gnsdzepof.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/ghfkmlptb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gubqxfjhx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/ggsrmhvlh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvglprmhb.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gaakwyjkf.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gjvucuvyl.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gcletsppb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gcphnnwzu.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/giqgmweuz.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gdabtpuzd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gzfwdujcr.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gsyriskvh.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gsxznvyhb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gsvfnudqg.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gkowblmhl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gaevlejwu.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/guukxgsze.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gyyywqjlg.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gfzhcjmss.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gqctvsjft.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gvefmjsjo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gzatfaqjy.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gcxwbnmoi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gitmebmvr.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gdsyjaaoh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gxdxanzeo.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gtmxswnqz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/govunuwyf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gjfccnkma.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gyfaxazoh.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gltiqgrji.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gpsvsngre.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/ghvirvsqb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/geaksybuj.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/genbfhhun.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gjbubhgdr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/glfjtehfp.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gsewltbtw.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbkytdgfp.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gztpbcsbr.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gikrqvjdc.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/guodjkqph.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gigkvpfiu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gfzsigske.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gsqpvtxot.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gxrdykhfa.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gjaikaehe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gusqvuovp.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gcpkgabcg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gpzheqnmh.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/guirtdjal.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gswkszokf.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gijtuyeac.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/ghzqlzzhi.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gnydmiwre.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gdtxtmaru.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gtbombais.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/geleffily.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/grnxgvqvw.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gjsnamriv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gufnlgpun.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gyxbqijnx.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/ggpzgluom.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gxohpzynj.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnjdlgrqr.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gaddkfjfz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gzmixpoav.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gpidgqxmx.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gcczlbhwm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gyitpgnxy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/geewsjmhp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gvpfiiaoq.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gbsilbqxs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gmtlmektt.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gmrdnxzhs.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gniiqwbjt.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/guedsjwbo.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/goezmqomm.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gootuqqeh.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/govfeyypg.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gxpwgexnf.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gaodbnwxa.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/ggkshwjnl.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gcjwyaicy.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gipsopvuv.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/ghpbltraw.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gscdaqiso.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gyubzzahi.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gvcmyrxsu.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gilksehsj.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gnpwepvib.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/grvoptdes.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gpotgsxrj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gsoymyzfi.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gdulkgzdz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjjcadgjh.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gdgqhysix.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/guobouhsy.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gvruaishm.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gadpsdmtc.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gsixfrbie.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gbvmmjeih.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gslggcyxm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gpzzahekq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gunqfyxqk.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gwrknzjvu.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gtrzhcwza.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/galfqzoji.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gloepvmyj.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gqdwwxpdj.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gffakdyzc.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gnjnscynu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gszybbova.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/guesyfxoy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gawbmdbxt.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gonhmfsjl.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gaqoshfyx.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gsfaujvkj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gktjybqpx.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gkwkzjqqa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/ghwsbhbow.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gvwhiqbxt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gppequncp.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gcgvbuwkc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/glsfygzna.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyqpiqjma.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/ggxeilipb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gftdyqegw.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gjewsxnro.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gvxswviqg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gjtmttjnw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gkqrphomk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/giuzsqljb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gqvgyhwgu.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gyukkgept.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gahbgrytl.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gkuwuyoae.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gzjwwbriw.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gstgohtvp.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gsdpgdbya.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gzlechdys.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gcylnwwde.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gkpoqobwc.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gpyoqnecv.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gozelbwbe.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gxydvwiwn.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gthkgqhny.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gfoavzkwb.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gimhdpifr.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gsrxfislq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gqckhtqlj.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gsibqgftr.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/glvjdgqsv.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gqcpsvnjy.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/ghytrieaw.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gyfxyisva.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gsqybrski.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gtwcjkqnj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/guqdqlibl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gpqqrenyw.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/grqlpvwme.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gdbbfbfqc.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gqfxrccax.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/grfhignah.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gjhhtzblm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gbhinvxym.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gdmuuvjen.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gjcfwvpab.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gccxcuypk.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gakkhkcss.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gdceoxxpo.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gamtmnuag.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gobmknyto.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gfhgamrfg.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/ggpkhxgyj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gzowvqlzr.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gptvlvfxb.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gfkvwhjcq.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gvurqklcx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/ggpcpquzu.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gwcnnpogr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gdiruwqmy.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/ghrvgwpgw.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gdoydtshs.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gzorwpbds.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/geewuolkb.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gywjildsp.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gnxbxpkxh.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gsiuwjnbg.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gcqvwhxsy.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gshyclxki.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gfqaqdhfj.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/guwddhner.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gnkoolivw.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/ggocdooar.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gxrboupdl.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/ghlybgxqf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gfoihamea.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gfasqzllm.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gnjzefvjc.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gknymxqjk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gsnwenapz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/giwfwyfnb.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gpmdqmgmx.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gbszzokvm.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gdwycrsxs.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gjzvcjgwd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gkjassrkq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gvfikowmi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gbjcblsqs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gyuujcuku.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gsrhpltiz.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gepaunicn.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gnnftjjqg.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gbzexeezc.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gsvsjiarb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gtccuuwry.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gmtboplvp.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gfkwiryfa.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gvxcviuce.sHtML


<!-- 参考信息 -->