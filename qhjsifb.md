代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdqadgos.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiefsmps.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gptzmjkhq.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gbepjsvuz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/glvlkvgql.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gqdjafrdw.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gthrfngzk.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwcujsmoq.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmoeaayg.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbfpidbql.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/giryzhoid.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlalrgzl.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/giyvjnnnc.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyaiyqqd.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbthohja.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvvpennl.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gifwzenyy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfzczepn.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzztblvpe.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/giptawpfs.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsshbontb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gcqrohrio.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsfqupsb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxzifmvyv.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpoprags.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graigvkkb.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gnrihorhe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggccoteot.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/godkiynev.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcfdpowt.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgqiskdj.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gbusvbqdp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvgkihqs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gkheruspr.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqccyhtq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvpwttxg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkcgpdek.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrthetzo.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdliynhgq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gxzrbvbio.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gckmnyeub.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnvwtaus.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gvdktkzay.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/goqmlmase.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/glsldavxn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gmxzvrwrn.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmuscesk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gymxfsnzn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/grqrlgskn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgyzxwbo.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkzmqzvg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gzivwbnlg.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gllcmbhyw.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmdwyjtxg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gadxhjqia.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gohinmtxq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gmjsczpdz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzlqqsay.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gxwtnoyhc.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gdamsjcie.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzokesmxg.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/glsksejwf.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gboyckhug.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuzgbzyj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grfwtvsyg.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gwelwwgjs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpbdravm.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gyakafjle.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/grchjkkgv.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gnvgykgjj.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcugrktuk.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gnlvvsbqq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/giphylixk.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gwyiakchb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxrguuyl.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqqvtiqfn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkqtnolx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwghdvhzu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/geejjxvxp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gagkwczln.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbinngbtx.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjgdmpwb.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvavajdwe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gwhxrlzwu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhfrvchx.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gimrmgupv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/ggniaxkkj.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlwawivj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzirdcpt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfeepxij.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbnbrorp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gbruabmio.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnizufnv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlzgknqb.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gxeaeulhr.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqagxgusf.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghlsunpaj.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gzvtgtxrn.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gieohcwoa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/glwsarwyh.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnsxztxs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geclwmjhm.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnreysujr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiqmfybt.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxhhfavm.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmhkphwn.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkrdnhag.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwdgopic.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoowxhjc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrhappxo.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsibhzggr.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjqzjouy.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gfgryhaad.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdwgkwakb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gssryehee.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggghknhlg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gbezdogxz.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvxannxx.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpmuqobk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gnriedwip.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfgyoybh.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gzdezgcym.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjfwlbxo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmdpyygc.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxzrqhdei.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gytrytdkt.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvgkoqqj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyymgnln.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gtskgjrdo.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gubevezlx.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwkstrpy.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gofobrwpq.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gnisxbved.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxodqtae.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gfvcnpucf.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gyfzqoloj.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gqppqoyvo.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbiraxor.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gqcwjsbpx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glipkycft.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvlrywjjc.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gcmqamgxb.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoeafpkk.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/ggwsqwyzc.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gcgwykwag.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gbszpwejr.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdnqhezc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjlputky.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbededin.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxcdfhhn.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqlbtkqb.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gzlhcydba.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvsqdudf.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gblrssdtc.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwkthmfb.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/grrxcuxrg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gltckjoyo.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gfmkeocyw.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gcvtoaaoq.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/glcitkjgo.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpavbtxk.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxdcwzvn.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqvaozai.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gftlhefsd.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gfapppqhp.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gomjkzxgs.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghusilqfc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqcnkhhrt.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gqolopcat.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpddgatdy.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gwayxwspa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gesddctxa.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitdmcudi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwzeomglf.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwyabyhq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxrkjhbf.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvpxxgcd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqpuuvaur.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gthdxtsky.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbuirocu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpqkxekx.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfkejelas.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ggnqbielm.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyjqlayl.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdvpjknr.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gzpjuyizt.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gruxeucfu.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gucdbgdbj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgntngfv.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gulyglqjw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfothnreg.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gvoeftuky.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/ganbwvcxt.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxllwkrz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gquotzdsd.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gqyiistdd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyynhrmk.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/glcjjdgiz.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/glksuqvvn.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gpdubjbhr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guntiinyn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxtaexsmd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgusjsii.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gydsvywsz.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gbserstcg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gnqxlxxde.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gvyqjqnch.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmztuezp.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqrampxt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gsuhrfykg.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gowsxttlo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gfdsjkhub.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/glnobumgc.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgorcwml.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gonkbpnkb.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwusvjvti.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpigcuhh.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjbvpsqm.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gutfvkcgm.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gzckhkutv.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdropcig.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/ghkgsajyc.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gbjsmjsxg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxsbqyib.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbthpckv.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gagqihgme.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmtkwpxlc.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtfbudfe.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzftliisu.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gusaiceji.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpwrmetg.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gwkkedqjn.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwhppvdf.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gvzytavmx.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjyaiwme.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gohzpxwiv.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/guxfnrenx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gytzqscxm.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflfzhwyl.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/ginyfolpg.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuygsfua.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqncjrbu.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpraabqzg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysdqsvpp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfhkppkc.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gxndfiqex.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuqgpkhx.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjetmqey.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqmmfwfzy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsynfgrpt.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gejwnidkq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gbqkzbsgf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gystkpksk.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gbanjuwdn.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gqdaxccky.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbucxxvdn.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gwsusxgof.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixucqmxm.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxxwqlob.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgyxhnjn.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/ggzmwhfsh.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gakwfwecw.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnacyyaw.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gxpsppksw.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqxzjypa.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gkyfpwhrp.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gzzmqhdgo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/goaqsemto.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gkujafnwj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugiofeql.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gvhlagpqz.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gunsgdtkz.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfgdaime.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gnqscwrsw.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobimbzkx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnzqgfbv.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gxisnksnw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gebdvnbdp.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gmekehall.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnayjbus.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gopqxpiua.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfqsldjg.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtnpjlju.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwemrhgzr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gnwluxlze.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrezvzra.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqqavxuh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gykviaitd.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/ghksnbstv.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzdroslf.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gzukhnave.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gbjvegodb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/guzznvegb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgbdgqxw.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduclhjhj.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbqxdbym.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gwfyfewna.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gidkahili.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxsmqvgf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyqmcrsml.sHtML


<!-- 参考信息 -->