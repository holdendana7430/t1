代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjggrosw.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyacqmvef.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gywsenkzn.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gqglvaigs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/ghlzhxurp.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjauukvv.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouxknrmr.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gdbbgxvri.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwezrlnoq.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/godihxirh.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gaidpgfnb.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwggbcvh.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/godqvxzsf.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/grmxtqdlc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuieeybp.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gvltgrswj.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/glxqjceut.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxvyfssk.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/glvogztvj.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrpojmoy.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/guwbzbwnz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxbxjtpg.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnllntyyd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gjolgcasy.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gkbrwscdq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjruqfng.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gmutuessl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geywpqsfn.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gsrcstxpm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbuyrjwno.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gzkiiblkb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzwzghkz.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gnqokqlay.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gswnqgizc.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnyonjgp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrzlyfyr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gqgjmfcav.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gdcafznnl.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshohiswh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhsndkep.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmgjddhbo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtespokn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gksfypoid.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gxnetxvsc.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcnlgufm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdulppqb.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/guvshtpfj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggdtdpydf.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/ghfcizbgk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfbcpfgy.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvhmnifa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcbdwykyx.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gruszqnar.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnwntgbt.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbftyrjke.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnadwplwk.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckmfxjbe.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrbadctg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuvddypn.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gkygkjshl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkxxtimy.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ggcfaxmoq.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfuvugmv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelavbdwy.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gprcvswwb.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gmalwnlqm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgkqbvkl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghndgtqtp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaubjcfen.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/geykbochs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctfeffvc.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/guisdrlhn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsqthabp.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/grwvhxzek.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtezhzekm.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbepsrmg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnluktlhc.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoqsvdjt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqylymavf.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/glokwziye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gyaokohhn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqbkanjcg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gmuorhalh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guhbpkoie.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrcknqpv.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfodrrzpf.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/galzdhnes.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdavwrkg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwqhviqu.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrlzrall.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/guxvpjxpx.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjtbwnzx.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gcyavvppo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfunqrnl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfmwijtf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gdoegpycn.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrendkpr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gupfukolg.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gymykmjey.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gakxuaagw.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcanudzwl.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gptmhpxdx.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gzkhyjgnh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gejsnsgxh.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gvbkimmot.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gunmpyjkf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdhleiil.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlcygbsn.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gimykagjt.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gitxkhuyo.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/grmflvojr.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqemoakr.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gxshqgkrc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gspcvtzdv.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkphowioi.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gcjdvzfvl.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gftygkqdw.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoeonbzs.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghttadkqm.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxstrcex.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnarnjqd.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbhkpdana.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaupehuz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/guxiauooc.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwcwrazsg.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfnucmyi.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/geqicsplh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gphrkhdqr.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggspsdgln.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gmwycpsqp.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gzugxwgcn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/ggkgemvgc.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/guqmsfevz.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gglmhyybe.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gnhaqdzmr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhleytho.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gwqphbpfy.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/goodtozqc.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzpoxyce.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvorrsnph.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/ggedzwwqs.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gyyfdkadz.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gnlppppgr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gynyysxkn.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfmahzcr.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/guthielmj.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcljiyydl.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/geelaeekl.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gkuzgsavs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gydbmaobz.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxmkhqxv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdcngrrr.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcncapyh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmgwenzn.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvhvjrnvj.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gbxyyxgit.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatouwpiw.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gzrxddsfz.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtowlfkvq.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzezhmaq.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjshnofc.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjizmbdff.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlnkeahq.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxemslfrx.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjslepovp.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/giuiwvjzs.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gxurzprdc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gsplepijn.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslzairyi.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtfztziw.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gswoiefcv.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjqzzqwcz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmskejao.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gatllolxv.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gcpioyhua.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gehfrymkf.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/giibmatit.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gplerdfjg.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gveiavhfb.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbjnijan.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuhyszkh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxtvyyrb.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjyoegtt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbnouedd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkndompp.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgcxrtnn.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/guyvukgvd.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gitpvrqnk.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfpdoklv.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ggtwdegcu.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfadexex.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gqioukdil.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuvhcctu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkebyatfo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtleyqxxy.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcynqybg.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsdwtlkb.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/genidmlfr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxksqvgh.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gvzoguwku.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/grscuuzcd.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbughzrvp.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/govihxzbd.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgvfknko.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkhradmg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogqufmtk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gtlgkzqoj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcxdagzab.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/groizvbmu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzcyuxah.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvuihujs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkpoviyi.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqwdzjrb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcamkgwvr.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdkzfpei.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhdfzsus.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gmuloujoe.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnmsremd.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqayutyq.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokuqedkj.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gdgajoklz.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwsawbaf.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gaimtfvix.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gtucorsgj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggkmgkjb.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgtsivee.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnkmpjvw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gjcroxkhj.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicbetsxk.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gzuscotlb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gniwmpuxr.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gykkvdcxj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/grnrzpkef.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtnecfok.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyuqyfxw.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvisbwiv.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gvseqczeb.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gyzrcuwht.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gmllynapx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoqcdivp.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/getwudjej.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/getgpfbtr.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gfcokuvvk.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuwcjnvp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqtguvlj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrwugiaq.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gbyscfeas.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gxwnfaujz.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gwmmrnmfn.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gczznmktm.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyjdnhrt.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdjmwxxb.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvusinxdw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/glovalmlf.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gljnzhkjm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsotytsd.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/guznvypby.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbexdmjsg.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbhowaya.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaphqumck.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gnjliagqs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/glgmwuhpy.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/grqiavdbt.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gqorkwrpb.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/grdjekvri.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgkjeqfa.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdahvhbg.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gnydvbhvx.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/giviihjwh.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gofrgophe.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gqsqzddlc.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gskjbgjvs.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/grikkrxcp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gbcnopdns.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksjudixl.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gqselrnnt.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gzijwkctb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gniikxzjb.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gtaslagbe.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gekftqcpb.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/glkqcucwa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdaqtagx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprbthmim.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gpcbxhjyo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejunmmte.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gcayzqpfr.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/grsijbirv.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/guwczkrab.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/grleyhdhx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gjfxadnhp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gnxbmoakm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gjyfayxcs.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/giqstahdt.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlsojfit.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/grpcbwyhr.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gtyjnokwl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlwtaisj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpewqezh.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gtefzccvq.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbuqpmpu.sHtML


<!-- 参考信息 -->