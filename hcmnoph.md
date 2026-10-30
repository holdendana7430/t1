代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gqvxdbfhy.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/grikmlszt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gjhveckos.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gnvncfwaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkwmachk.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvsondxq.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gsaoohhll.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpgmnwhq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gblxyjbxx.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbitcfnc.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxrjgbufq.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqevnnez.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gyibihtit.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwphtyqc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwllouvj.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gyunmzqks.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gwnneeqlh.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhynupoz.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gixhpbnnl.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjbhmxtb.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gahizltln.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqpdpxui.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqwhkdiy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjohqhxo.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gltatidqi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzfsjxyc.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyrrouka.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganohdnvw.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrvnlrnr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyzmghft.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbserxbl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoziwruq.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/ghcairbqk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnvdubpu.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvbdlaii.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gcimollhe.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpteogdpz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gsgxackpv.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfilmhgai.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ggcmjkpji.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggjsjqwno.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnteqfpos.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxfzrblhf.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gbdhbgaay.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gnfwslemp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvbzezjm.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/glvxwleyj.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqutigwsl.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gtndiczlp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwztienel.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gminzhkny.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcnsuxwks.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaqtpdxw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gffrntkrt.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkqpltefu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigcniuos.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcnslwfz.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytvpxrbs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvagxrhai.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjgqsasb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwreyfgw.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gdtrcqpqs.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/guwoobrlo.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gorjvcnqw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgczylmr.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/guzukedjr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgbvbktu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcihqvai.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ghezxlfjm.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gebftszcq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmzwgooo.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhykvadv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsvbfdix.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzlkvogu.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwghzaxas.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gqwzfruif.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gjtwxvrza.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gzgydkbnz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxntxtei.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcphltmg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/guxltedsz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtaxnwcud.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gnjeqkege.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsrfuilkx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/girlclihi.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqxxyhrb.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyylbfjkt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gspvgistn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbolbcld.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkatqxss.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gqanpvaef.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gcnmrnusg.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gttlnkgcz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgtdslha.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdyqqice.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlqdbjon.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gukivcues.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnzgpkal.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwuzwwwl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnzsbayz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/goebncdwl.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbsdkzpw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbzwrobkf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyzhxogj.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/ggkoxfkbn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gilechwpi.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gpdofehja.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfhmrdndd.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/giycjvgka.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdbsewcj.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxhjjrlbi.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisczgkcs.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzsltiqk.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbhoyphd.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gujsatkdg.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/guzhecwad.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmawcmev.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpewgtxoa.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/ganxospmv.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gdcugalod.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwzjgqkc.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlmvqngc.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gtijynfgr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gektnjics.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/giaqnejiz.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmtjkszi.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/guventafo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqtnfvhvq.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glbtosrgb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzfihelg.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmxamlke.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcuwhlyf.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gkncoipzv.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gphjneqeq.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gwwirzndd.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrqhgooj.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gbukkcprw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gvdgjzmhx.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoufzwdh.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gzzzrrfzz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpfbkspr.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsndxsryn.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtxgtazp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gojelcanf.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gksvvfjsg.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmipsgvku.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvqbhcqt.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gvgdpoazm.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxpljeeg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gavkubiva.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gbgksazhd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqquffiv.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/glpmgjcov.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiqmcbxg.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqzfsaekx.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxomabgyk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjhnicov.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/goyefifzq.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzmacsfgv.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gkabhzgon.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtemurwd.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gpxpjegza.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfisexrzb.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/grdyimmkd.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfqravpxn.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gthjfuihq.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gtovgozeu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gwdyehccf.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcroiyoc.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpghssbu.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grgjmgrhb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcpwltcd.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gglldrmfy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvewysom.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gxntexwoo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guwkqvplm.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhefovng.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxocywoao.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdubwuwap.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/grkcskzlt.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbgxiigb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbztcketa.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gudtelpux.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/guenuqokl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtkopyqer.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmcfevlb.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwxitpubq.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghgxzowcm.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gztlnlkvf.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gnwkozumt.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpixqcvd.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gsstfpftg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvyovfwm.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmbwukqb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnfnzdrek.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gyfdlicfh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoyozdty.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxxttmeg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gtvztlgcc.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gevnasaxv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjeiqlcr.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkuupwbb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gvondhdmi.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsjujqee.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gnirjxmrc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxfycbelr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/geahwdsfi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuvnbtbd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrsqbqkl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gbjksgxkq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gujmkwxrx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gveeyxvqo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbybpuhvo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gyjrgbydl.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/ggtufixod.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gefmjubvj.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gnwsbifmh.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqdlvpdn.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/geuvusklw.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisjalunl.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxtgxyfr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdusdschb.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gmkbnzrcc.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gxbcczboz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvripfni.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gyztnrgqq.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbcdayzy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdskirkpl.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ghnvwmdln.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcpwzssd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqsytyszh.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyctsoke.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/grzcmqqpg.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gldepdvaz.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcnajcxd.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueepmmga.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlwdqlnt.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqurlakr.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxdlxmax.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gulrqrnue.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gmnznpwvq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqmultwm.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfrplizs.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gqsfqpjnp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gibdpgjsg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkukdsxfa.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcaiskws.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gviubikju.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gkciycgzk.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gjbzcnfbi.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gmrtxysys.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gxagbkhxo.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjrwitkl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiyjdijw.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/guuygjfdg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gsycfqxmq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gabpstgpu.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gbixammov.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gcpsksqzk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzbolsuo.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gwcspxfze.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/ghpakjosr.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gzhqavzem.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaztpigsb.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gltmsgnhq.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gefvtolhq.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gxjqohthr.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gvdcvfntx.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gpophsdfj.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyvwkhqi.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnizxrjc.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gsvfwjxpf.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gmfzlhtxn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gebenglbm.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvcngyiy.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfnnqdnu.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/grblgbuvm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedcjcibc.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcogdrmh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakqaoser.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpifimpqs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gcsrnfmno.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjgzdsrb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucrayqeg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhtszucj.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrgpdvrg.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjqpjadb.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnlzcual.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgbegkxb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgqnkxan.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gnipiedra.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gohhbayop.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfmxrcgm.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gjheiczlb.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gyirgulxi.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/guuhjeznk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gvhhyjdbl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdibtcxbw.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gjngeiyov.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gbjjvqqkr.sHtML


<!-- 参考信息 -->