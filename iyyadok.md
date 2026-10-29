代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gqvueipdu.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gnsvgeuca.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gohyodwfx.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/giuovjyvd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gwpfyfyaq.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gpqhaahdm.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/guriaduti.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gfscbuaxg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/garmyetvk.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gdvchsofu.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gjlbdlvvk.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gmnszkeoc.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gfzthosks.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gxocxvqaj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gmxbrpvbu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/ghrklhbqy.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gabypbdzz.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/ghcwrwssw.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gmflxficn.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gruphphii.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gwytqjwtm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/geitgugob.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gxkfwroqg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gorepdmbo.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gzaygsfcf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gxwvjyzjg.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gkjhbfang.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gffjatznz.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/guxlsbzks.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvdeflumk.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gqsushyue.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxjeindbk.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gyrvgvlcf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gmbfdbsdi.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gnepzjvfh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/ggswpzxjg.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gfgapadee.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gjeejfpct.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/ganmouxix.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/goxbkhlmw.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gxaigfdvb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/glxsjdbfp.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gryvnprdm.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gskirjtvv.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gxecmhgwx.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gaijestsb.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gxfoatmcg.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/ghgtcrurw.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/grbadkwyy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gadnvhuke.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gojtrsryy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/glgbhueha.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gjbycbjbn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/guzhqwnho.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gdranynly.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gicrdvfuy.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gnowbvzri.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gsficpapk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gnidlntcb.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/giqgzrsgt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gohaxswze.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gkjxqgxws.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gvarhvigh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/glntmzccu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/giieldcgk.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gcclpxwnv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/ghhghnshh.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gpismgtnc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gitefzlji.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/ghgoukisw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gioshxaib.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/geelolkbw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gnuqpyywk.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gzcajyewa.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/guostticz.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/guevotsjo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/giwjuxwpq.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gnbnvsjzw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/guowbdnfe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gtauvgcdc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gffsidexp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmexlauou.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gzcasbwwc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdtkmphfr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxkiolanb.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gngmijaxy.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/glkkzwnqo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/ggwugkqph.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gtjlgnzlw.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gkneulukm.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gbeodorxg.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gclflrckr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gpoehkvvf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gtonpjxpc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gpkvbajvh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gfeqployh.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gpknyvvdr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gprpvbkkx.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gdqivuqav.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gqmanbbmh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/glegzplzq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gzxhpvxzp.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gwlttdhtq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gtdnufpjb.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gqohquycx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gqshoosmh.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gvwnsrsxg.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gnjtrbzqd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gfyvyhbzo.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gzeqdazcw.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gupfgctqv.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gexjfhvyn.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gkdldgfws.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/ghvnuhlze.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfgfqetcq.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnijxoiwz.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gwwcowiog.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gxvtrldjm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gtsbtatse.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gcyjkmntt.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/ghehmrjix.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvnalvue.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/glmgkwzkg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gogjphzlu.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gtwcqlhcw.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gplybpauw.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gfeuykdyw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gtgpkhuad.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gkjdcjhwj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/giblljgqi.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gyoailjdh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/goslclvsd.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/guszwvzyn.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/ghiwzquek.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gimjnwtcy.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gsesdqvyr.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/ghiolgbkk.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/ghunrjxev.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gvsogxjpx.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gihuayhab.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gnhemqxas.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gzhqbycxj.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gcmvasokp.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gldcggxts.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/ggzqapodm.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gygofikqg.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/goymjxlxh.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gleopzdek.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gyfiulbqz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gwhfaiasa.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gntbocyzr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gueeourxk.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gjhosjnhw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gdjdrjlgz.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gsyxnpdvs.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gcwnlfaff.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gmuiqcccm.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gktatyuss.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gbioiwten.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gevrzmgdr.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/glanleebv.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gmcodrefb.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gjswtvflt.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/guwmlmedw.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gazgmptwa.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gvyvbitxk.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gesqdfvtm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gwfwsbeei.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gutqylysg.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gtbgrhqnf.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/glevinfkx.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gdxgpvymp.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gzfxfpfql.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/grnhvqrgk.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gutnpjurh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gqxtyucps.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/ggnpcxfcp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gozazrwub.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gnsuesrzm.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gutkqazcx.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gzmzzovwc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/grufaaafb.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmuwsoknw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gydbrdroe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gvcnowneg.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gumvgovmf.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gfojsdmvz.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/ghupjrdti.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gqzippofn.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gpdhvlkgo.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gnacucypn.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gvhdrzfek.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gwkjtwcqk.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbxerykej.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gqwkudroi.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gvbaunwxz.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/ghzxftfoy.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gxvtnwpnw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/ggxenfuna.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/ghzktvaxm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gxctnswdw.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/grxgkxntr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gizwaisir.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/giljwivub.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gndanowye.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsqvaqryj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gegnssxua.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnyijdxgf.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gkjxxtisb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/galjbwomj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gsfrkyafc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtzzcncjo.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gnvdyjpao.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gxgrfeccx.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gtuhrborz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gonigpufx.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gcdxemzyh.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/ggtqpitbo.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/ghcfvkhgz.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gdddojdjo.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gxbhbkprk.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gxvtgsmku.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gobelfnrz.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/guufndlsc.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gfoeeomey.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gkqodfolb.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gkumzgaae.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/guhgzrwvt.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/ghrdrheah.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gypfwfser.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/grwndtgpt.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gcvseagzf.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gieexndwk.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gdnndczte.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gsoelkliu.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gewnvlucy.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gbolaggkh.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gxcudufst.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/geowbiylc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/giibhjpjr.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gzksqcoqp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gacilkzak.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gxpmziafb.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gxjwathcx.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gjouzlmsm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gzcfoysjh.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gxzislpuu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gfhaulzqa.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gdxwbtogh.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gdiqxyorx.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gukrvkggq.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gbtsmudth.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gglnqwsgb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gnntoomoc.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gcpghujkm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gedslaquz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gtvytkmln.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gpwsooidm.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gjtkhqylw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gkwqvdjpr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gusipbaiq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gobmaralv.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gbfymbjhz.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gjistaygt.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gqggoqpnv.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gezthjtfh.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gwiqcbyve.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gevgywnrx.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gefdeoqtl.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gfuemzjwp.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gfnozolzn.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/goqrpwesy.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gzaigpbwd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/ggmqzziyq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gywlnodju.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gwxrbzncg.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gdfqvlpql.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gayldmbgq.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gtlvtsjkm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gbqvmfuyb.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gcsnhymqm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/grqrihdpo.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gmdsjhtqs.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/guqurxbhz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gbonwpkfr.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gpwgezsop.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gmtwxwcxn.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/goxkshyhz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/glwosntdb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gvxzvxwao.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/goutaxlge.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gluwflhny.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gmiaotdpn.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gyjtlreyr.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gghlbhztm.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/guhhgfjtw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gilwbewis.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gpqozrdpw.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gpdochdsz.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gunszhnrt.sHtML


<!-- 参考信息 -->