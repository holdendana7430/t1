代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gehvdkhka.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcwkxwbm.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gzxkrsidt.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/ganefbsmy.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwqiwpfq.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqszhpba.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghunmfxnb.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqifhxhwl.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gdxkiaotx.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxxdmzfi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjclzganz.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gsujmxazo.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gflfjazmg.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhcswjmg.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/grtjmmeyi.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbnwkzxd.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gsgltyuew.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcxnagaal.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsmzunpt.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/ggphzgnqa.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvkvgybo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyooxyij.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gexavdqgo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqbpkqwu.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrypjups.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getzskzjv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkibshbju.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilxbctug.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gyndmcefa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gujcydhnq.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfullpty.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqtkijgp.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gelesvtgz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gunuqpqbl.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxjginqw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gignqemmf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaujhgtjv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gczywhvrc.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzilgnaj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjnntrch.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gtdaxqymn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfesfbnmu.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtoomnpn.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbvoaqajp.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gexrmzlod.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gnirufwij.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gcsmhhxce.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggwmvesoh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwshioba.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpjvaqdxh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyxpjjri.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsqbwyyj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqzeniqe.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorqkhcav.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gulpnojkp.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gelzwwumi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/giurtdnva.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gejlnwohw.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjfvrzcg.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/glavtvrmu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gznfawztd.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzkmlemp.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/grfyhoxam.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gapumkzwu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtidlebya.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gvgvbtlkr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gosidzygi.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnltttwa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/godbftzan.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqpkioca.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goazxksrk.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gyleyheio.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/grcqnyeio.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlzimixc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gssputtfe.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkhdagpi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbeohumn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfpqfrwl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gscitiqzo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyhzflvf.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqrdbdula.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gmfjqsmyi.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gssyuikrw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gylyemggw.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gtejdxbbz.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gsqylkhmg.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gowdpegbe.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gzywwfbri.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gzhyevmom.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gbapajspc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gflcxnnqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gwidnrgdo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gsijxiwxg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbybwbmzg.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjgrlrep.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcypmkjci.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgxbdbey.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnswjcez.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gryyvyzda.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggesyhbjo.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gaackffyx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/grltrcyby.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwrjprwu.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtupraelb.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzvhqqyu.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gaijnypji.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/ghpzmdjgo.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeciinse.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjjjvsti.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gttzlpjoa.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyzbazmv.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gpthawzke.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gnzztzwfe.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvlggnyh.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gylshfsut.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaswaxenv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfbwnkzq.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhpzvbwv.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/guuqunhdm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprrbhcvx.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnpfybbh.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsrzfzku.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gmwuxough.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqrnrwbdb.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxkknlte.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbbqoxbuw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesffyyyl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gfvhgiyri.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gbimotvrf.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gdqfqntwn.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gohmpslry.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gngmgivba.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/golhjnhfj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gitmiryzo.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/goxurrxwj.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsfpifnq.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gvwsrsajm.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcesfegqe.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gpslwqxsl.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfyaksnd.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfcclabnk.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ghntqnslj.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpisheyif.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gfoxoqeio.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gjofxpcoo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gethmrocf.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gatyowklx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyrbpoyg.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gsiykopnl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvowdreix.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/guzhnbuoh.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvjtbfko.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfamavic.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gsyktgcwc.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gelgvwcyw.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gimktpmsc.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpgtcrqr.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymwzpsjc.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gunrpjhti.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gxolluhfg.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gepwykyih.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaxwxudg.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkmqdjnpf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkeawtcb.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gcjeixpgw.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwroowhmo.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbmsvkbcj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcbxzlmj.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gqmkxrack.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghxrveuvb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcnkafze.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpoonymc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmlkcnet.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnnyuygda.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpxmdvvgk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwvyprtj.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/glztbllxp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyxudchqv.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhvppsmi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gprkzrgqp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtumtsvph.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwiqrmir.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrmnbadm.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzhaqfced.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gctifncsu.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gtdenterb.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/galppoaef.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsnfcvyn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gwzhvagix.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/glaghbtni.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpiakkla.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gpxxsgvaq.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvlsakgh.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gexdohtsw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gwyifevgu.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtpzeevm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gtboxthcv.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmhvqlta.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gzewdgutv.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/grmznqljv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gvomllzgp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnocucxoj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqykoeqsl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grxiyvoix.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gecgaakrz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpniqqgc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/ghmpxtqrq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxagdpwx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawucdghl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gpkehxppp.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gvilbvoyo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsnyjtfw.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefwkkkwp.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gfqoepncz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsmqbbuz.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gmvjjzhin.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhadjhha.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gcfgsuube.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gihysfqly.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gizndiipn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqxyzjyf.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/glhvuwbpy.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gymuunmkn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcibyauyo.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gukqniyht.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpavilrmo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gysnjgtir.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gviivwzxr.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gpdntybhx.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicneanbe.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/ghvqailxa.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gzaxhilwu.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gywaunpyg.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcyherpk.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcqlnscq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gefhtrcff.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpylkdigm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/grejkooqs.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/geptiszxg.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvehezts.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gudlatvzv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqlseywgc.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/galsnaixg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/ggqwkxbkd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpohzpccf.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gevuqevyx.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gwagzerqh.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gkobtujmo.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gblmgjnyg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gwhaqjauh.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcvxcarw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvabnxvb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gtktusvlm.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmqaidsf.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gtenloeef.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gacaawniw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gevtedabe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcpgmtsl.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkammbna.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcgppvkr.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/geoohifdg.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/giwjidoop.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyfvvpbc.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gudkxjtet.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapdweldx.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/grptdkycv.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkjzuxhn.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwjdtefg.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/ginlukmxo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gffkflisg.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpmnpopy.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gykdmxdan.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gmhjnbxwd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gihfglyho.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkobpxot.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkcrhnom.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdakessjk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqsugkxz.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gprouobuc.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gswwfpcjo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcgjbkev.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjcrkwly.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gazekhrmv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfjhxjfl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gylikzytm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gynuapnts.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gaxcsgudq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgiwspmr.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gxppvzowi.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoexmlih.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/grqhngorp.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjthzqgw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gztbvfyhg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcruvdgjk.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gtonhhymw.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpninween.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbmyexym.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/grrytgeej.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gyngtgxdz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmshcihte.sHtML


<!-- 参考信息 -->