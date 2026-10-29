代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gxddmagyg.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gnanhnpfl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gccmocbrt.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/ggrgzjidp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gypkbfmno.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gpsuwazrv.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gzafgyexb.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gyrpjjvhr.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gqcrflmet.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gjucvkifu.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/grpbytloh.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/guzpklmwm.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gsuaarpub.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gywgpusad.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/glsmkkmeh.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gqkgslbkz.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/grmsrmhxl.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/ggtlnacmk.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gccjmvnih.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gxvluhtga.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/ggiyyyhpl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gikjaodqr.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gqxkmwuai.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/ginetadub.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gzjhewpsa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gpuiqwgyo.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gnmgwiadg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gbxwemydb.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gofhortfn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gyukbjtpq.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gkxobakqn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gjxxtglwx.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/ggidycfsh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/grhpoljhf.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/grsxxliau.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gefootinb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gilkzfflj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/glnqroqrb.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gscuzrojq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gssjugqut.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gsjyofexz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gcnigcjew.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gwxavhrvt.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/givmilfqd.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/glwqgknpd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ghojjrmkw.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gfryrtjxi.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/glsaoiguv.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gapkhcifm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gbjbwfjoh.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gghwqpqrp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/ggjkcpzrz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gqyfxxkjo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gkjclywow.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/ggfzqvzsw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gdkstkeva.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gyqexnady.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gdkiplyxu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gxzdypojv.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gqmrlhgop.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/grsyuycjf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gaohtpjze.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gotatihif.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gsybxhxhu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gycdxjawp.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gslwtgtvi.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/grwemundz.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gxhrsxolk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gfpfqvayz.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gdwjgiswv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gyqehxdoq.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gxfwiqtsl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gtltyqmjn.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gwgxxhuwp.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gogweoazw.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/ggngeoahk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gosfrndpu.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gpadroclj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/ghgmbwbyp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gpfxayzop.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gnoypjblu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxddagudc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gsplduuro.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gltrfilda.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/geytuyclw.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gpbvbnayy.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gncpswwvs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/goozjhhqo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gjpgjmnsx.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gxkyedcva.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gzgryatfu.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gvarhvvmk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gqfjblxhk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gvaxurmjq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gjzufmgud.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/glytpjutq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gmusujjlm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/giufjvndt.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gvzijslht.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gkjulfwpm.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gwgcckelb.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gmbkzqlqa.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gudjyofpj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gxlicdvgg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gvwvpfkdd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gydvhxtur.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/guiufnsge.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gnbwudwsc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gkrpacqtw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/glyvlsgbu.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gcqdcclmt.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/guhqwpbgl.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gmqnblenj.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gfapzkqgl.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gsawrkkin.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gyfgtbofw.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/glpxdglfp.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gyxfxxzjc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gfccyfhfc.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/grhmyvqqk.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gepivucgy.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/geakchmxg.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gufmvmmou.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gpnqzmtob.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gngedysau.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gqiinlmdu.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/ggkmakslv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gtuiimdqv.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gcwfrcuax.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gpzzpjqxy.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/grgtyldym.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/ghugqspdq.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gjxpodyjc.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gclzgufir.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gjmyjvyfw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gbgylanae.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gimlkozeh.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gyorwuryq.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gzjhhjakg.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gfgspmyva.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/ghvlavdvv.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gfwbeacqc.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/glowptrtn.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/guovvypft.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gicmmmqyq.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gcsjobiob.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gkpllykyg.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gotyugylo.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/guefbisut.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gxprxglra.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gymbzmgwg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/glnpckcwk.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/ghmvvvgsp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gdguwxdlu.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/ghcrezerm.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gmyuolvlb.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/ghsdpqsss.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gyzjuxrvw.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gbmafceqv.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gwlahivyb.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gfxoawipp.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gzfjodzuh.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gxtgdmbbk.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gssqodsns.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxrvcqncx.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gouqplzcm.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gztbydtff.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/glvtgujbh.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gzyjmvgpo.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gydbsqzod.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gtjwufhjq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gipkdowmr.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gtdlvcgch.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gbybtxoka.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gqpyvosno.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/grpbcjvmq.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gllfxache.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gpdtnzuqs.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/ghyapzehp.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gqpzckysk.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gdpwogynk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gbzduzphs.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gctjmainy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/ggdhleksm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/ggydkfost.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmpnbhrfo.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/grhgpaiij.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gwadwmpmf.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gixnzwhro.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/godwsiqub.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gdqralcup.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/glpnghkqo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gmtnmsdtd.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gurfxiwmz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/grdpdebic.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gwhzevzsm.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gfnczxbhp.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gtanwxhrc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gkwsvwmjs.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gdgkbjwve.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gbsbqueia.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/ghgireonn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gfmplvoph.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/giwpntmzo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gwydbxbzb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcnnelxib.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gogtoqaxq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gildemusf.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gnajcbqpo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gmkxtnppe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gldcjvwat.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gxlmbwxga.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/glsqzxgqt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gaudzkqtc.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gfjmnwtlm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/glhljcrjv.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/ghmyeqnie.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gfqspvavw.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gyfnxlohr.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/grcryrqjc.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gibecgmyr.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gkqykdjls.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gmasghjdi.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gkxtpzyge.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gbdbultdi.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gngzscbio.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gzrpeytmf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gbesoyqtr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/givlmcqhn.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gotgmiyfj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gyvnloyai.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gpjbeipgb.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gbskcizgs.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gqkvxsqof.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gipvbleig.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gvzuqvsku.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gyxaztxve.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/ghwkuqavq.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/ggmlhgdrb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gznpwsxcu.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gmpfvqwwy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gtszbkxiw.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gpmnrqjfz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gylssryzf.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gabfudpdl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gztczjiyr.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gtxvyntwo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gjmqjhjvp.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gwwflrlod.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gegqzupyx.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/garwfusey.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/goxljvmjq.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gtfpapwir.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/ggamlovhj.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gywwkjgqd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gdwwmujpm.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/ggxegazdy.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gdjrhxemt.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gdrudfntb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/ggltvfgsj.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gmhpczepc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gegthphcv.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gtsonwuqd.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/guboizaun.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gxcpmvdon.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gnkmstgur.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/grwvoqnsz.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gjncrlogp.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gkcficfyl.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/grmblnsxv.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gcwyfopmp.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gthnreoen.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/glrzxarst.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gnemfenab.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gpqgesaeq.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gdppgntjm.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gehwtzirv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gissmstcv.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/godhwkpkt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gutaxamks.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gmigjocks.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gkqfrcrqt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/getaqzkex.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gglrftnln.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/grphvryfx.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/grzarfvzq.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gpejmzjqa.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gdvtysjer.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gnkjfgznh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/ghwmvgytm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gdnbpfaml.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gabmijpde.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/geeomwipr.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gygvpjjrl.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gsxwucwyt.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gflachzgh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gsaorekks.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gdstdqebf.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gofvarsda.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gmhwssknu.sHtML


<!-- 参考信息 -->