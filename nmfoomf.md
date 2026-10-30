代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjosmnlok.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/guhplkjpq.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gbpfhywkw.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gujuprojx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gbmkjwsge.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnsxljrm.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxvpzjbqz.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjxlepuka.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/goxldztfj.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsoclfxj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrxxbiaq.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzntgzhyz.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjfibevw.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggotzoira.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrtcryst.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gchdcgmri.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbvtxzqh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiogykgb.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjqftzycn.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gipyybafp.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/giefsprat.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsftmkaje.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/ghidqttke.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtqkbzdvx.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtzkzsys.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ganfqcoas.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gbaeutcjn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkapsyiru.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gvlcndfqx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutoxjxsv.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvabrftd.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqgmilzh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwcdzgwxz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsblekxv.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/ggaczgobw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ggdzxwkcr.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gleziekjw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/geyebcoxv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkcajlml.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtopypyj.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gxvvbqybn.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/ghkmclmon.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gruqwqrkn.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmftbctsn.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gxcboyhcy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrludrix.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gimhvgugi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goarlhqsk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gzruninyd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwspemosx.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbvxvvhi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gmknpeszh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ggxauwjjq.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzyfhstmg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkvlrihy.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnbkbnjf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdpinwpk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqhomnbu.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/guioqmsve.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gwfqguhhm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoaniwxf.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjgekphe.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcxrswnd.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gzdcspmsv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpmyksms.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/geappfmyw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyiyocxt.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggskjzzwu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdesetsty.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gapvftspu.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdgkoctl.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpfpataa.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gsiwwilyd.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gyinbhcfh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdmcriql.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwmvymej.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gfcegsmuf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwxrzsnsr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/govollnol.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gndgrlftz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfogdjux.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtahnkvx.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgnhlwsx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/grawgslma.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gsmakjypv.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnpdohmg.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbwzvxbp.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqxjgcla.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gwnjmnvil.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxajhqdl.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gszyizzvf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gbmasehmb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmtsfchq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gltjebemi.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gijifgunp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/geeicatuy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gobbauoim.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gexlrimzw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gozvdlxyd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkzqlicl.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gostriqfi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgrxmuz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrgpahml.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxqdkjkm.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/galruhpxe.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnexqazxd.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/guwhgnssx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguvyeebz.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gvldlydmn.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafzhaynn.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcoipdfpr.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrhndzld.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzkoulmn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcqwzopt.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gdkidtmad.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtjjxtsc.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhcisldm.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajxbiaks.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspdaaegh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gvovzdhpt.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjacrrpwn.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/ghpmppeie.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxwmjygm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswokaspd.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guateaasl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/grsnqujii.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gbvdbjjpp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbknuwggj.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumepujik.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/grylperae.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdvpybsi.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gezicveip.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/ginvacfqw.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/giivgfkgt.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gqobdpghp.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/grobyugih.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gyhcuuvyz.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gdnlznhgg.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptrrweib.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpxbgqqa.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gamtzppmd.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gzlaomzat.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclldtmwz.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gaylihyek.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcavgion.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbavihhp.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gluhsmzxw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobwqamyd.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxnmyary.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhqlyynm.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gakfbeyrb.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/ginhakcby.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gztzeaegl.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gzelfzsgm.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvglntlkn.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/grgnmdmov.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gqxcfnost.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gndyxqnna.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gwtdctkxq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gyammqbaj.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmospjso.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/galvlvoyw.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjfblgzn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/guwzxuxhy.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxikfcuad.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmckanyp.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/giqfrmlzy.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghhekquww.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gotpxrlkz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzncgizqj.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/goolbcpqd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gojzpjpmd.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gaspnbnoc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gclaveouw.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeuteqsf.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquczmexp.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvncnyaqe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmxybunld.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogwnvefe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gpaztayph.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtrbinjrm.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glxkjwszu.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/giapmgrfl.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfegqsgw.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrwwlekg.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gbgkhbzjt.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjctzunzv.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/grhgcgllb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvtttjkif.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysmidhnk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gywlbzdhr.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtldjjwkw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkcxbcfl.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/glfkhfjhu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gszmzrdne.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gernsidzs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gdlnvmrwu.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gzptqxdbm.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgeszybq.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsizphpet.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpsghhvy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gavgpsmiv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gihkunzxn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgejwhzf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gcptqybnp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkytprdb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/grlfuztao.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtsistevn.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvbqdxnt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgadtkjq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpxcbnvl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzjswjjq.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gptbornud.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduclgovz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gzemcyvyq.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gujcjrwmy.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gibgfdsxv.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/guxmnlzxc.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gigtofges.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlufipcs.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgszhrim.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxhenfpu.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gphxyzsoy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubtoqkjl.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gtwwxomyn.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzlyqxgs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfjuwnzj.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/grrtvblhf.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/ghctfrfyk.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/geihjezex.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgmvcqde.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gthfzybib.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/golityzlb.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtvvqrcf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gdenohkhg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gshkxcyni.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaiwalhc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzijvzcb.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gxlkaljit.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhocmcbe.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyujpfkw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gghxydkhq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gitpltonh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gxlhjatez.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlufllxx.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpabepzm.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gqsdrrvar.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxinrrbhu.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvkzesyak.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gveetqgpl.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrljltbu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gimrpxdqp.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gywufmbai.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gliyzbytk.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynphdkae.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gakoukwut.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqeajmih.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gwklgyqmd.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfjnwtdp.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gswaescxu.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjqgosvy.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/golkslvem.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/guismrybu.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/goxwvmzik.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gkclyzmmc.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbqmznvl.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggilibtof.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiregmyp.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gkrnudzjd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlxplprh.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gsidsmhtj.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvtsjigk.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdosevoyv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxohdqmcb.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjyufenh.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gyjgbamhx.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/guygqkvea.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/ghuwlbtmx.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjgvefnq.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmidrqwa.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbvqsggy.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcieawjaf.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gapbfydne.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gycnnjlfh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gfabqrwsp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gstfxvejw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gnjlltxcd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhaljzmn.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnpknxba.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gwzhwbdxm.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxowkdnk.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/grgjubimv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvotwsxh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gauajcaoi.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpgsvjln.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtppwvuar.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gvxgkruyj.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgdaxrbl.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwckmorpq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmojheybn.sHtML


<!-- 参考信息 -->